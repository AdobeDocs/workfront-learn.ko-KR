---
title: 사용자 기반의 와일드카드로 필터 만들기
description: 사용자 기반의 와일드카드를 사용하는 방법 및 로그인한 사용자를 기반으로 필터를 빌드하는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 48%

---

# 사용자 기반의 와일드카드로 필터 만들기

이 비디오에서는 다음 방법을 배우게 됩니다.

* 와일드카드를 사용하는 이유 이해
* 사용자 기반의 와일드카드로 필터 빌드

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>작업 또는 문제 할당 정보를 조회하는 필터를 빌드할 때 할당 사용자 >> ID 필드 소스 및 이름을 사용합니다.  이 옵션은   &quot;소유자&quot; 또는 기본 할당자뿐만 아니라 작업 또는 문제에 할당된 사용자입니다.

>[!TIP]
>
>필터를 직접 빌드할 때도 $$USER.ID(이름 대신)를 사용합니다. 이렇게 하면 누군가가 사용자가 실행 중인 필터를 보고 &quot;나와 공유&quot;라고 말하면 필터를 이미 설정하므로 이 필터를 사용하는 각 사람이 자신의 정보를 볼 수 있습니다.

>[!TIP]
>
>사용자 기반의 와일드카드를 사용할 때는 항상 Equal 필터 한정자를 사용해야 합니다.


## 사용자 기반 와일드카드 활동을 사용하여 필터 만들기

이 페이지의 PDF를 다운로드하려면 [여기를 클릭](/help/assets/create-filters-with-user-based-wildcards-activities.pdf)하십시오.

### 학습활동 1

이번 주에 약간의 추가 시간이 있어서, 귀하의 팀에 그들의 과제에 도움을 사용할 수 있는 사람이 있는지 확인하고 싶습니다. 작업 필터를 만들어 이번 주 만료 예정인 완료되지 않은 작업을 찾습니다.

### 답변 1

팀원들을 도와줘서 정말 고마워! 아래 이미지와 같이 필터가 설정되면 다음 작업을 찾을 수 있습니다.

* 완료되지 않았습니다(즉, [!UICONTROL 완료] 상태 또는 [!UICONTROL 완료]와 같은 상태가 없음).
* [!UICONTROL 현재] 상태의 프로젝트에 있습니다(아직 시작되지 않은 프로젝트에 대한 작업을 찾지 않으려는 경우).
* Workfront 팀 설정에 의해 정의된 대로 홈 팀의 사용자에게 할당된 작업
* 그리고 이 주의 완료 날짜는 이번 주 언젠가 입니다(이 규칙은 사전 작성된 날짜 필터를 사용하여 &quot;이번 주&quot;를 정의함).

![사용자 기반의 와일드카드로 작업 필터를 만드는 화면 이미지](assets/user-wildcard-exercise-answer.png)

목록을 좀 더 제한해야 하는 경우, 몇 가지 추가 필터를 추가해야 할 수도 있습니다. 예를 들어 팀에서 작업하는 특정 프로그램이나 포트폴리오를 보는 필터 규칙을 추가할 수 있습니다.
