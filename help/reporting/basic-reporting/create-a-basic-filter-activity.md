---
title: 기본 필터 활동 만들기
description: 이 활동에서는 "내가 소유한 프로젝트 중 이번 달 마감"이라는 프로젝트 필터를 만듭니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 기본 필터 활동 만들기

이 비디오에서는 &quot;내가 소유한 프로젝트 중 이번 달 종료하는 프로젝트&quot;라는 프로젝트 필터를 만듭니다. 많은 프로젝트를 주시하는 경우 이 필터를 사용하여 곧 닫을 프로젝트를 확대할 수 있습니다.

아래에 단계별 지침이 포함되어 있습니다.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## 답변

![새 필터를 만드는 화면 이미지](assets/basic-filter-activity-updated-6-15-21.png)

1. 다음 위치로 이동 [!UICONTROL 프로젝트] 에서 영역 [!UICONTROL 메인 메뉴]. 프로젝트 목록이 표시됩니다.
1. 다음을 클릭합니다. **[!UICONTROL 필터]** 메뉴 및 선택 **[!UICONTROL 새 필터]**.
1. 필터 이름을 &quot;이번 달에 끝나는 내가 소유한 프로젝트&quot;로 지정합니다.
1. 클릭 **[!UICONTROL 필터 규칙 추가]**.
1. 다음에서 [!UICONTROL 필드 이름을 입력하십시오.] 필드에 &quot;owner&quot;를 입력합니다. 그런 다음 을 선택합니다 [!UICONTROL 소유자 ID] 다음 아래에 [!UICONTROL 프로젝트] 필드 소스입니다.
1. 나가기 [!UICONTROL 같음] 그대로 연산자.
1. 이름 입력 시작 필드에 &quot;$$&quot;을(를) 입력합니다.
1. 선택 [!UICONTROL $$USER.ID]. 로그인한 사용자의 와일드카드입니다.
1. 클릭 [!UICONTROL 필터 규칙 추가] 다시.
1. 다음에서 [!UICONTROL 필드 이름을 입력하십시오.] 필드에 &quot;Is Complete&quot;를 입력합니다. 그런 다음 을 선택합니다 [!UICONTROL 완료됨] 을 클릭합니다.
1. 나가기 [!UICONTROL 같음] 그대로 연산자.
1. &quot;False&quot;를 선택합니다.
1. 클릭 [!UICONTROL 필터 규칙 추가] 다시.
1. 다음에서 [!UICONTROL 필드 이름을 입력하십시오.] 필드 유형 &quot;계획됨&quot;, 다음을 선택 [!UICONTROL 계획된 완료 일자] 다음 아래에 [!UICONTROL 프로젝트] 필드 소스입니다.
1. 변경 [!UICONTROL 같음] 연산자 - [!UICONTROL 이번 달].
1. 클릭 **[!UICONTROL 필터 저장]**
