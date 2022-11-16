---
title: 날짜 기반 와일드카드를 사용하여 필터 만들기
description: 날짜 기반 와일드카드를 사용하는 방법 및 시기 및 현재 날짜를 기반으로 필터를 만드는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 날짜 기반 와일드카드를 사용하여 필터 만들기

이 비디오에서는 다음 방법을 배웁니다.

* 날짜 기반 와일드카드를 사용할 시기 파악
* Workfront의 두 날짜 기반 와일드카드 간의 차이를 이해합니다
* 필터에 날짜 기반 와일드카드 추가
* 와일드카드, 속성, 연산자 및 한정자를 사용하여 사용자 지정 날짜를 만듭니다
* 와일드카드를 사용하여 사용자 지정 날짜 범위 만들기

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12)

## 활동 질문

1. 기한 날짜가 어제나 오늘인 문제가 필요한 경우 필터 규칙을 어떻게 작성합니까?
1. 지난 주에 예정되었던 프로젝트를 찾기 위해 필터 규칙을 어떻게 구축합니까?
1. 다음 필터 규칙은 정기적으로 사용하는 작업 보고서의 일부입니다. 이 보고서에서는 어떤 유형의 결과를 얻을 수 있습니까?

![날짜 기반 와일드카드를 사용하여 작업 필터를 만드는 화면의 이미지입니다](assets/date-wildcard-answer-1.png)

## 답변

1. 다음 사이의 문제 계획된 완료 날짜를 필터링합니다. [!UICONTROL $TODAY-1d] 및 [!UICONTROL $$오늘].
1. 프로젝트 계획 완료 날짜 사이에 필터링 [!UICONTROL $TODAYb-1w] 및 [!UICONTROL $$TODAYe-1w].
1. 이 보고서는 아직 완료되지 않은 작업(즉, 완료율이 100보다 작음)을 찾아서 기한 초과 또는 오늘 기한 초과 작업을 찾습니다. 작업의 계획된 완료 날짜에 대한 필터 규칙은 기한 일자가 오늘 날짜와 같거나 이전인 작업을 확인하도록 합니다.
