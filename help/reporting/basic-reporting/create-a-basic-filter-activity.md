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
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 32%

---

# 기본 필터 활동 만들기

## 활동 1 - 마케팅 포트폴리오의 모든 프로젝트

이 활동에서는 의 &quot;마케팅 포트폴리오의 모든 프로젝트&quot;라는 프로젝트 필터를 만듭니다. [!UICONTROL 레거시 필터] 경험. 포트폴리오에 있는 &quot;마케팅 Portfolio&quot;이라는 모든 프로젝트가 상태에 관계없이 표시됩니다.

단계별 지침은 아래에 포함되어 있습니다.

### 활동 1에 대한 답변

![새 필터를 생성하는 화면 이미지](assets/basic-filter-activity-1.png)

1. [!UICONTROL 메인 메뉴]에서 [!UICONTROL 프로젝트] 영역으로 이동합니다. 그러면 프로젝트 목록이 표시됩니다.
1. 다음을 클릭합니다. **[!UICONTROL 필터]** 메뉴 및 선택 [!UICONTROL 레거시 필터].
1. 선택 **[!UICONTROL 새 필터]**.
1. 필터 이름을 &quot;마케팅 포트폴리오의 모든 프로젝트&quot;로 지정합니다.
1. **[!UICONTROL 필터 규칙 추가]**&#x200B;를 클릭합니다.
1. 다음에서 [!UICONTROL 필드 이름을 입력하십시오.] 필드, 유형 &quot;[!UICONTROL 포트폴리오 이름]&quot;. 그런 다음 을 선택합니다 [!UICONTROL 이름] 다음 아래에 [!UICONTROL Portfolio] 필드 소스입니다.
1. [!UICONTROL 같음] 연산자를 그대로 둡니다.
1. 유형 &quot;[!UICONTROL 마케팅]의 &quot; [!UICONTROL 이름을 입력하십시오.] 필드.
1. 선택 [!UICONTROL 마케팅 Portfolio] 필터링할 해당 이름의 포트폴리오가 있다고 가정합니다. 그렇지 않은 경우 바로 앞에 입력 기능을 사용하여 원하는 포트폴리오를 찾을 수 있습니다.
1. 클릭 **[!UICONTROL 필터 저장]**.

## 활동 2 - 내가 소유한 이달 마감 프로젝트

이 비디오는 다음에서 &quot;이번 달에 끝나는 내가 소유한 프로젝트&quot;라는 프로젝트 필터를 만듭니다. [!UICONTROL 레거시 필터] 경험. 많은 프로젝트를 주시하는 경우 이 필터를 사용하여 곧 닫을 프로젝트를 확대할 수 있습니다.

단계별 지침은 아래에 포함되어 있습니다.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### 활동 2에 대한 답변

![새 필터를 생성하는 화면 이미지](assets/basic-filter-activity-updated-6-15-21.png)

1. [!UICONTROL 메인 메뉴]에서 [!UICONTROL 프로젝트] 영역으로 이동합니다. 그러면 프로젝트 목록이 표시됩니다.
1. 다음을 클릭합니다. **[!UICONTROL 필터]** 메뉴 및 선택 [!UICONTROL 레거시 필터].
1. 선택 **[!UICONTROL 새 필터]**.
1. 필터 이름을 &quot;이번 달에 내가 소유한 프로젝트&quot;로 지정합니다.
1. **[!UICONTROL 필터 규칙 추가]**&#x200B;를 클릭합니다.
1. 다음에서 [!UICONTROL 필드 이름을 입력하십시오.] 필드에 &quot;owner&quot;를 입력합니다. [!UICONTROL 프로젝트] 필드 소스 아래의 [!UICONTROL 소유자 ID]를 선택합니다.
1. [!UICONTROL 같음] 연산자를 그대로 둡니다.
1. 다음에 &quot;$$&quot; 입력 [!UICONTROL 이름을 입력하십시오.] 필드.
1. [!UICONTROL $$USER.ID]를 선택합니다. 로그인한 사용자의 와일드카드입니다.
1. 다시 [!UICONTROL 필터 규칙 추가]를 클릭합니다.
1. 다음에서 [!UICONTROL 필드 이름을 입력하십시오.] 필드에 &quot;Is Complete&quot;를 입력하십시오. 그런 다음 프로젝트 필드 소스 아래의 [!UICONTROL 완료됨]을 선택합니다.
1. [!UICONTROL 같음] 연산자를 그대로 둡니다.
1. &quot;False&quot;를 선택합니다.
1. 다시 [!UICONTROL 필터 규칙 추가]를 클릭합니다.
1. 다음에서 [!UICONTROL 필드 이름을 입력하십시오.] 필드 유형 &quot;계획됨&quot;, 다음을 선택 [!UICONTROL 계획된 완료 일자] 다음 아래에 [!UICONTROL 프로젝트] 필드 소스입니다.
1. [!UICONTROL 같음] 연산자를 [!UICONTROL 이번 달]로 변경합니다.
1. 클릭 **[!UICONTROL 필터 저장]**.
