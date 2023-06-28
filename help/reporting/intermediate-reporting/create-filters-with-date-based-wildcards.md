---
title: 날짜 기반 와일드카드로 필터 만들기
description: 날짜 기반 와일드카드를 사용하는 방법 및 시기와 현재 날짜를 기반으로 필터를 작성하는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 날짜 기반 와일드카드로 필터 만들기

이 비디오에서는 다음 방법을 알아봅니다.

* 날짜 기반 와일드카드 사용 시점 파악
* Workfront의 두 날짜 기반 와일드카드 간의 차이점 이해
* 날짜 기반 와일드카드를 필터에 추가
* 와일드카드, 속성, 연산자 및 수정자를 사용하여 사용자 정의 날짜를 만듭니다
* 와일드카드를 사용하여 사용자 정의 날짜 범위 만들기

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on)

## 활동 질문

1. 기한이 어제 또는 오늘인 문제를 원하는 경우 필터 규칙을 어떻게 작성합니까?
1. 지난 주에 마감된 프로젝트를 찾기 위해 필터 규칙을 어떻게 작성합니까?
1. 다음 필터 규칙은 정기적으로 사용하는 작업 보고서의 일부입니다. 이 보고서에서 얻을 수 있는 결과 유형은 무엇입니까?

![날짜 기반 와일드카드로 작업 필터를 만드는 화면 이미지](assets/date-wildcard-answer-1.png)

## 답변

1. 다음 기간 사이의 문제 계획된 완료 일자 필터링 [!UICONTROL $$TODAY-1d] 및 [!UICONTROL $$오늘].
1. 다음 기간 사이의 프로젝트 계획 완료 일자 필터링 [!UICONTROL $$TODAYb-1w] 및 [!UICONTROL $$TODAYe-1w].
1. 이 보고서는 아직 완료되지 않았고(즉, 완료율이 100 미만인 경우), 기한이 지났거나 오늘 기한이 지난 작업을 찾습니다. 작업의 계획된 완료 일자에 대한 필터 규칙에서는 기한이 오늘 일자와 같거나 이전인 작업을 확인하도록 되어 있습니다.
