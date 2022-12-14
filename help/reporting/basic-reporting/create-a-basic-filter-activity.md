---
title: 기본 필터 활동 만들기
description: 이 활동에서는 "Projects I Own This Month Closing"이라는 프로젝트 필터를 만듭니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 기본 필터 활동 만들기

이 비디오에서는 &quot;Projects I Own This Month Closing&quot;이라는 프로젝트 필터를 만듭니다. 많은 프로젝트를 계속 보고 있다면 이 필터를 통해 곧 닫을 예정인 프로젝트를 확대할 수 있습니다.

단계별 지침은 아래에 나와 있습니다.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## 답변

![새 필터를 만드는 화면의 이미지입니다.](assets/basic-filter-activity-updated-6-15-21.png)

1. 로 이동합니다 [!UICONTROL 프로젝트] 지역 [!UICONTROL 기본 메뉴]. 프로젝트 목록이 표시됩니다.
1. 을(를) 클릭합니다. **[!UICONTROL 필터]** 메뉴 및 선택 **[!UICONTROL 새 필터]**.
1. 필터의 이름을 &quot;Projects I Own This Month Closing&quot;으로 지정합니다.
1. 클릭 **[!UICONTROL 필터 규칙 추가]**.
1. 에서 [!UICONTROL 필드 이름 입력 시작] 필드에 &quot;owner&quot;를 입력합니다. 그런 다음 을(를) 선택합니다 [!UICONTROL 소유자 ID] 아래에 [!UICONTROL 프로젝트] 필드 소스.
1. 을(를) 종료하십시오. [!UICONTROL Equal] 연산자를 있는 그대로 사용합니다.
1. 이름 입력 시작 필드에 &quot;$$&quot;을 입력합니다.
1. 선택 [!UICONTROL $$USER.ID]. 로그인한 사용자의 와일드카드입니다.
1. 클릭 [!UICONTROL 필터 규칙 추가] 다시 한 번
1. 에서 [!UICONTROL 필드 이름 입력 시작] 필드에서 &quot;Is Complete&quot;를 입력합니다. 그런 다음 을(를) 선택합니다 [!UICONTROL 완료됨] 프로젝트 필드 소스 아래에 표시됩니다.
1. 을(를) 종료하십시오. [!UICONTROL Equal] 연산자를 있는 그대로 사용합니다.
1. &quot;False&quot;를 선택합니다.
1. 클릭 [!UICONTROL 필터 규칙 추가] 다시 한 번
1. 에서 [!UICONTROL 필드 이름 입력 시작] 필드 유형 &quot;계획됨&quot;을 선택한 다음 [!UICONTROL 계획 완료 일자] 아래에 [!UICONTROL 프로젝트] 필드 소스.
1. 변경 [!UICONTROL Equal] 연산자 대상 [!UICONTROL 이번 달].
1. 클릭 **[!UICONTROL 필터 저장]**
