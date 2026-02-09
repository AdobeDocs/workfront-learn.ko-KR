---
title: 복잡한 보고를 위해 EXISTS 필터 만들기
description: EXISTS 필터가 무엇인지, 어떤 역할을 하는지, 그리고 처음부터 어떻게 빌드할 수 있는지 알아봅니다. 또한 EXISTS 필터의 많은 유용한 예를 살펴봅니다.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
source-git-commit: 66bab1a0b2316a31cb99916220500303e49797ad
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 4%

---

# 복잡한 보고를 위해 EXISTS 필터 만들기

EXISTS 필터는 표준 Report Builder에서 2 테이블/필드 이동 제한을 해결할 수 있는 고급 텍스트 모드 필터입니다. 또는 NOTEXISTS를 통해 특정 관계 조건이 부족한 시스템 내 오브젝트를 식별하는 데 사용할 수 있습니다.

이 비디오에서는 EXISTS 필터를 만들어 증명 승인 보고서에서 &quot;현재 프로젝트에 대한 증명 승인&quot;을 보는 방법에 대해 알아봅니다.

EXISTS 함수에 대한 자세한 설명은 [EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기](https://experienceleague.adobe.com/ko/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements) 설명서를 참조하십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3471210/?captions=kor&quality=12&learn=on&enablevpops=1)

## 존재함 필터 예

### 프로젝트 보고서 존재함

작업 수준에서 찾은 projectID를 비교하여 프로젝트 수준 ID 필드와 일치시켜 작업을 연결 개체로 사용합니다. 그러면 작업의 할당 사용자를 $$USER.ID 와일드카드와 비교할 수 있습니다. 그러면 조회하는 사용자가 할당된 프로젝트만 반환됩니다
기본 피할당자 여부와 상관없이 작업.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


또한 문제(optask) 수준에서 찾은 projectID를 비교하고 이를 프로젝트 수준 ID 필드와 일치시켜 문제(optask)를 연결 개체로 사용합니다. 그런 다음 해당 문제(optasks) 중 지정된 범위 내에 입력 일자가 있는지 확인합니다. 이 경우 가 있는 모든 프로젝트가 반환됩니다.
notexists로 인해 지난 30일 동안 rolling에 기록된 문제(optask)가 없습니다.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### 템플릿 보고서 있음

이 필터는 프로젝트를 만드는 데 사용되지 않았거나 지난 1년 동안 프로젝트에 첨부된 모든 템플릿을 표시합니다. 한 가지 주의 사항은 템플릿이 첨부 파일로 사용되었는지 여부를 파악하기 위해 작업이 포함된 템플릿에 따라 달라진다는 것입니다.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### 작업 보고서 존재함

할당 taskID 및 작업 ID로 연결하여 사용자 테이블을 연결 개체로 사용합니다. 그러면 팀 컬렉션 ID를 사용자 팀 ID로 검사하여 할당자가 보는 사용자와 동일한 팀에 있는 경우 작업을 반환합니다.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### 사용자 보고서 있음

이렇게 하면 지난 3주 동안 업데이트를 게시하지 않은 모든 사용자가 반환됩니다. 참고 개체를 사용하여 간격을 연결하고 ownerID를 사용자 ID와 비교합니다. 는 자신이 소유한 노트의 입력 일자가 3주 전보다 크지 않은 경우 해당 사용자를 반환합니다.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

지난 주에 시간을 기록하지 않은 모든 사용자가 반환됩니다. 이 메서드는 위의 예제와 매우 유사한 메서드를 사용하지만, 대신 시간 소유자 정보와 시간 입력 날짜를 사용하여 반환되는 사용자를 기반으로 합니다.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

사용자 보고서에서 프로젝트의 사람 탭과 일치하는 사용자 목록을 표시합니다.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### 범주(사용자 정의 양식) 보고서 존재함

이 텍스트는 프로젝트에서 전혀 사용되지 않은 모든 프로젝트 양식 목록을 제공합니다. 이 옵션은 초점을 맞추는 양식의 개체 유형을 지정하는 것과 함께 사용해야 합니다. 따라서 이 경우 포커스는 PROJ이므로 objTypes 행에 콜아웃을 포함해야 합니다. 사용할 수 있습니다.
다른 객체 유형의 경우 객체 코드 관련 부분을 변경하면 됩니다. 프로젝트 첨부 양식 컬렉션을 나열된 양식으로 확인하고 일치하는 양식이 없으면 을 반환합니다.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### 매개변수(사용자 정의 필드) 보고서 존재함

현재 시스템의 사용자 정의 양식에 첨부되지 않은 모든 사용자 정의 필드가 반환됩니다.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### 보고서 있음

그러면 필터에서 특정 값을 사용하는 보고서가 반환됩니다.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

대시보드에 첨부된 모든 보고서가 반환됩니다.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### 증명 승인 보고서 존재함

이 경우 현재 상태의 프로젝트에만 증명 승인이 반환됩니다. 이 작업은 Document 개체를 사용하여 currentVersionID를 documentVersionID로 확인하여 증명 승인에서 프로젝트로의 간격을 메웁니다. 여기서 프로젝트 상태로 이동합니다.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
