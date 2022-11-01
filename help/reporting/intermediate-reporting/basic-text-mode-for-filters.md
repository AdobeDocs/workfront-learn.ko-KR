---
title: 필터에 대한 기본 텍스트 모드 이해
description: 텍스트 모드, 카멜 표기법 및 의 보고서 필터에서 사용할 수 있는 몇 가지 기본 "플러그 앤 플레이" 텍스트 모드를 알아봅니다 [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 필터에 대한 기본 텍스트 모드 이해

>[!IMPORTANT]
>
>전제 조건:
>
>* 보고 요소 이해
>* 보고 구성 요소 이해
>* 기본 필터 만들기


이 비디오에서는 다음을 학습합니다.

* 텍스트 모드는 무엇입니까?
* 낙타의 예는 무엇인가요
* 보고서 필터에서 사용할 수 있는 몇 가지 기본 &quot;플러그인 및 재생&quot; 텍스트 모드

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

다음 텍스트 모드에서는 사용자가 &quot;Done with My Part&quot;로 표시된 작업을 제외합니다. 작업 필터를 만들고 원하는 필터 규칙을 추가한 다음 텍스트 모드로 전환한 다음 필터에 표시되는 텍스트 모드 뒤에 아래 코드를 붙여 넣으면 됩니다.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## 추가적인 플러그인 및 재생 텍스트 모드 필터

### 작업 - 승인 대기 중인 모든 작업 표시

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### 작업 - 내가 승인한 모든 작업 표시

원하는 필터를 사용하여 작업 보고서를 만든 다음 필터 탭으로 이동하여 텍스트 모드로 전환을 클릭합니다. 이미 있는 항목에 이 코드를 추가합니다.

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### 작업 - 프로젝트 간 선행 작업이 하나 이상 있는 모든 작업 표시

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### 작업 - 다른 사용자에게 할당한 모든 작업 표시

원하는 필터를 사용하여 작업 보고서를 만든 다음 필터 탭으로 이동하여 텍스트 모드로 전환을 클릭합니다. 이미 있는 항목에 이 코드를 추가합니다.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

로그인한 사용자가 현재 담당자 중 하나 이상을 할당한 모든 작업을 표시합니다. 여러 사람에 의해 할당자가 지정된 경우 처음 할당받은 사람의 이름만 작업 랜딩 페이지에 &quot;요청자&quot;로 표시됩니다.

## 활동: 텍스트 모드 질문

1. &quot;ID로 입력됨&quot;이라는 제목의 필드에 대한 낙타사례를 어떻게 쓰실 건가요?
1. 문제 보고서에서 닫힌 것으로 표시되었지만 승인 보류 중인 문제를 표시하는 필터를 만듭니다.

### 답변

1. &quot;Entered By ID&quot; 필드에 대한 카멜 대소스는 다음과 같이 기록해야 합니다. enteredByID
1. 텍스트 모드는 문제 보고서 필터의 다음과 같습니다.

   ![텍스트 모드에서 새 필터를 만드는 화면의 이미지입니다](assets/btm-answer.png)
