---
title: 차트를 사용하여 보고서 만들기
description: 차트를 통해 데이터의 시각화를 개선하고 Workfront에서 차트 도구를 사용하는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
kt: 8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 차트를 사용하여 보고서 만들기

이 비디오에서는 다음을 학습합니다.

* 차트를 통해 데이터 시각화를 향상시키는 방법
* Workfront의 차트 도구를 사용하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12)

## 활동: 보고서에 차트 추가

분기 말이 가까워지고 있으며, 최근 완료된 프로젝트가 해당 예산에 맞게 어떻게 완료되었는지 확인할 수 있습니다. 프로젝트에 대한 계획 원가와 실제 원가를 보여 주는 보고서를 생성합니다. 지난 분기에 완료된 프로젝트만 표시하려고 합니다. 사용자 정의 색상을 사용하여 조합 열 차트를 추가합니다.

## 답변

1. 선택 **[!UICONTROL 보고서]** 에서 **[!UICONTROL 기본 메뉴]**.
1. 을(를) 클릭합니다. **[!UICONTROL 새 보고서]** 메뉴 및 선택 **[!UICONTROL 프로젝트]**.
1. 에서 **[!UICONTROL 열(보기)]** 탭, **[!UICONTROL 열 추가]**.
1. 선택 [!UICONTROL 프로젝트] > [!UICONTROL 계획 비용] 이 열을 **[!UICONTROL 합계]**.
1. 클릭 **[!UICONTROL 열 추가]** 다시 한 번
1. 선택 [!UICONTROL 프로젝트] > [!UICONTROL 실제 비용] 이 열을 **[!UICONTROL 합계]**.

   ![보고서에 열을 추가할 화면의 이미지입니다](assets/chart-report-columns.png)

1. 에서 **[!UICONTROL 그룹화]** 탭에서 보고서를 그룹화 기준으로 설정합니다 [!UICONTROL 프로젝트] > [!UICONTROL 이름].

   ![보고서에 그룹화를 추가할 화면의 이미지입니다](assets/chart-report-groupings.png)

1. 에서 **[!UICONTROL 필터]** 탭에서 두 개의 필터 규칙을 추가합니다.

   * [!UICONTROL 프로젝트] > [!UICONTROL 상태] > [!UICONTROL 완료]
   * [!UICONTROL 프로젝트] >[!UICONTROL  실제 완료 날짜] > [!UICONTROL 지난 분기]

   ![보고서에 필터를 추가할 화면의 이미지입니다](assets/chart-report-filters.png)

1. 에서 **[!UICONTROL 차트]** 탭, **[!UICONTROL 열]** 차트 유형입니다.
1. 대상 [!UICONTROL 왼쪽(Y) 축], 선택 [!UICONTROL 프로젝트] > [!UICONTROL 계획 비용].
1. 대상 [!UICONTROL 아래쪽(X) 축], 선택 [!UICONTROL 프로젝트] > [!UICONTROL 이름].
1. 을(를) 클릭합니다. **[!UICONTROL 조합 차트]** 단추를 누르고 선택합니다. [!UICONTROL 프로젝트] > [!UICONTROL 실제 비용] 에서 **[!UICONTROL 값]** 필드.
1. 색상 상자 옆의 화살표를 클릭하여 [!UICONTROL 실제 비용] 색상. 나타나는 색상 중 하나를 선택하거나 오른쪽 아래 모서리의 상자를 클릭하여 색상 팔레트를 표시합니다.
1. 클릭 **[!UICONTROL 저장 + 닫기]**. 보고서 이름을 묻는 메시지가 표시되면 &quot;Planning vs Actual Cost by Project Completed Last Quarter&quot;라고 합니다.

   ![보고서에 차트를 추가할 화면의 이미지입니다](assets/chart-report-chart.png)
