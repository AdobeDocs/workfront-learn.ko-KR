---
title: 필터의 기본 텍스트 모드 이해
description: 텍스트 모드가 무엇인지, 카멜 표기법이 무엇인지, Workfront의 보고서 필터에서 사용할 수 있는 몇 가지 기본 “플러그 앤 플레이” 텍스트 모드에 대해 알아봅니다.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: e17c8cafba5b0829c4bed987a5dad14ecbcb7eaf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 98%

---

# 필터의 기본 텍스트 모드 이해

>[!IMPORTANT]
>
>전제 조건:
>
>* 보고 요소 이해
>* 보고 구성 요소 이해
>* 기본 필터 만들기

>[!TIP]
>
>* 텍스트 모드에 대해 자세히 알아보려면 한 시간 길이의 녹화된 웨비나 이벤트인 [전문가에게 질문하기 - 텍스트 모드 보고 소개](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=ko-KR)를 시청하는 것이 좋습니다.
>* 텍스트 모드에 대해 자세히 알아보려면 총 5시간 30분 길이의 [고급 보고](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=ko-KR) 튜토리얼을 시청하는 것이 좋습니다.
>* 액세스하려면 여기를 클릭하십시오. [[!UICONTROL API 탐색기]](https://developer.adobe.com/workfront/api-explorer/)


이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 텍스트 모드의 정의
* 카멜 표기법의 정의
* 보고서 필터에서 사용할 수 있는 몇 가지 기본 “플러그 앤 플레이” 텍스트 모드

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## 작업 - “내 부분 완료”로 표시한 작업 필터링

다음 텍스트 모드는 사용자가 “내 부분 완료”라고 표시한 작업을 제외합니다. 작업 필터를 만들고 원하는 필터 규칙을 추가한 다음, 텍스트 모드로 전환하고 필터에 표시되는 텍스트 모드 뒤에 아래 코드를 붙여넣기만 하면 됩니다.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## 작업 - 승인 대기 중인 모든 작업 표시

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## 작업 - 내가 승인한 모든 작업 표시

원하는 필터로 작업 보고서를 만든 다음, 필터 탭으로 이동하여 텍스트 모드로 전환을 클릭합니다. 이미 있는 코드에 다음 코드를 추가합니다.

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## 작업 - 프로젝트 간 전임 작업이 하나 이상 있는 모든 작업 표시

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## 작업 - 다른 사람에게 할당한 모든 작업 표시

원하는 필터로 작업 보고서를 만든 다음, 필터 탭으로 이동하여 텍스트 모드로 전환을 클릭합니다. 이미 있는 코드에 다음 코드를 추가합니다.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

로그인한 사용자가 현재 할당자 중 적어도 한 명을 할당한 모든 작업을 보여 줍니다. 여러 사람이 할당자를 할당된 경우, 할당한 첫 번째 사람의 이름만 작업 랜딩 페이지에 “요청자”로 표시됩니다.

## 작업 - 완료된 모든 작업 표시 - 승인 보류 중

```
status=CPL:A
status_Mod=in
```


## 문제 - 완료된 모든 문제 표시 - 승인 보류 중

```
status=CPL:A
status_Mod=in
```


## 프로젝트 - 완료된 모든 프로젝트 표시 - 승인 보류 중

```
status=CPL:A
status_Mod=in
```


## 메모 - 내가 태그된 모든 댓글 표시

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## 매개변수/사용자 정의 필드 보고서 - 사용자 정의 양식에 첨부되지 않은 사용자 정의 필드 표시(정리 작업에 매우 유용함)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
