---
title: 기본 필터 활동 만들기
description: 이 활동에서는 "마케팅 포트폴리오의 모든 프로젝트"라는 프로젝트 필터와 "이번 달 마감하는 내가 소유한 프로젝트"라는 프로젝트 필터를 만듭니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
last-substantial-update: '2025-05-15T00:00:00.000Z'
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:23:25.803Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 462
ht-degree: 64%

---

# 기본 필터 활동 만들기


## 활동 1 - 마케팅 포트폴리오의 모든 프로젝트

이 활동에서는 “마케팅 포트폴리오의 모든 프로젝트”라는 [!UICONTROL 기존 필터] 환경의 프로젝트 필터를 만듭니다. 그러면 상태에 상관없이 “마케팅 포트폴리오”라는 포트폴리오의 모든 프로젝트가 표시됩니다.

단계별 지침은 아래에 포함되어 있습니다.

## 활동 1에 대한 답변

![새 필터를 생성하는 화면 이미지](assets/basic-filter-activity-1.png)

1. [!UICONTROL 메인 메뉴]에서 [!UICONTROL 프로젝트] 영역으로 이동합니다. 그러면 프로젝트 목록이 표시됩니다.
1. **[!UICONTROL 필터]** 메뉴를 클릭하고 아직 선택하지 않은 경우 [!UICONTROL 레거시 필터]을 선택하십시오.
1. **[!UICONTROL 새 필터]**&#x200B;를 선택합니다.
1. 필터 이름을 “마케팅 포트폴리오의 모든 프로젝트”로 지정합니다.
1. **[!UICONTROL 필터 규칙 추가]**&#x200B;를 클릭합니다.
1. **필드 선택** 필드를 클릭하고 &quot;[!UICONTROL 포트폴리오 이름]&quot;을(를) 입력하십시오. [!UICONTROL 포트폴리오] 필드 소스 아래의 [!UICONTROL 이름]을 선택합니다.
1. [!UICONTROL 같음] 연산자를 그대로 둡니다.
1. 검색 필드에 &quot;[!UICONTROL marketing]&quot;을(를) 입력하십시오.
1. 필터링할 해당 이름의 포트폴리오가 있다고 가정하고 [!UICONTROL 마케팅 포트폴리오]를 선택합니다. 그렇지 않은 경우 자동 완성 기능을 사용하여 원하는 포트폴리오를 찾습니다.
1. **[!UICONTROL 필터 저장]**&#x200B;을 클릭합니다.

## 활동 2 - 이번 달에 종료되는 내가 소유한 프로젝트

이 비디오에서는 “이번 달에 종료되는 내가 소유한 프로젝트”라는 [!UICONTROL 기존 필터] 환경의 프로젝트 필터를 만듭니다. 많은 프로젝트를 살펴보고 있다면 이 필터를 사용하여 곧 종료될 예정인 프로젝트를 확대할 수 있습니다.

단계별 지침은 아래에 포함되어 있습니다.

>[!VIDEO](https://video.tv.adobe.com/v/3443386/?captions=kor&quality=12&learn=on&enablevpops=1)

## 활동 2에 대한 답변

![새 필터를 생성하는 화면 이미지](assets/basic-filter-activity-2.png)

1. [!UICONTROL 메인 메뉴]에서 [!UICONTROL 프로젝트] 영역으로 이동합니다. 그러면 프로젝트 목록이 표시됩니다.
1. **[!UICONTROL 필터]** 메뉴를 클릭하고 아직 선택하지 않은 경우 [!UICONTROL 레거시 필터]을 선택하십시오.
1. **[!UICONTROL 새 필터]**&#x200B;를 선택합니다.
1. 필터 이름을 “이번 달에 종료되는 내가 소유한 프로젝트”로 지정합니다.
1. **[!UICONTROL 필터 규칙 추가]**&#x200B;를 클릭합니다.
1. **필드 선택** 필드를 클릭하고 &quot;소유자&quot;라는 단어를 입력하세요. 이제 [!UICONTROL 프로젝트] 필드 원본에서 소유자 ID를 클릭합니다.
1. [!UICONTROL 같음] 연산자를 그대로 둡니다.
1. 검색 필드에 &quot;$$&quot;을(를) 입력합니다.
1. [!UICONTROL $$USER.ID]를 선택합니다. 로그인한 사용자의 와일드카드입니다.
1. 다른 필터 규칙 추가를 클릭합니다.
1. **필드 선택** 필드를 클릭하고 &quot;완료됨&quot;이라는 단어를 입력하세요. 이제 [!UICONTROL 프로젝트] 필드 원본에서 &quot;완료됨&quot;을 클릭합니다.
1. [!UICONTROL 같음] 연산자를 그대로 둡니다.
1. “False”를 선택합니다.
1. 다른 필터 규칙 추가를 다시 클릭합니다.
1. **필드 선택** 필드를 클릭하고 &quot;계획됨&quot;이라는 단어를 입력하세요. 이제 [!UICONTROL 프로젝트] 필드 원본에서 &quot;계획된 완료 일자&quot;를 클릭하십시오.
1. [!UICONTROL 같음] 연산자를 [!UICONTROL 이번 달]로 변경합니다.
1. **[!UICONTROL 필터 저장]**&#x200B;을 클릭합니다.
