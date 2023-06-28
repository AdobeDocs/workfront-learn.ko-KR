---
title: 차트로 보고서 만들기
description: 차트가 데이터의 시각화를 개선하는 방법과 Workfront에서 차트 도구를 사용하는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 차트로 보고서 만들기

이 비디오에서는 다음 사항에 대해 알아봅니다.

* 차트가 데이터의 시각화를 개선하는 방법
* Workfront의 차트 도구 사용 방법

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## 활동: 보고서에 차트 추가

분기의 끝이 가까워지고 있으며, 최근에 완료된 프로젝트가 예산에 얼마나 부합하는지 확인하고자 합니다. 프로젝트의 계획된 비용과 실제 비용을 보여주는 보고서를 만듭니다. 지난 분기에 완료된 프로젝트만 표시하려고 합니다. 사용자 정의 색상을 사용하여 조합 열 차트를 추가합니다.

## 답변

1. 선택 **[!UICONTROL 보고서]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 다음을 클릭합니다. **[!UICONTROL 새 보고서]** 메뉴 및 선택 **[!UICONTROL 프로젝트]**.
1. 다음에서 **[!UICONTROL 열(보기)]** 탭을 클릭하고 **[!UICONTROL 열 추가]**.
1. 선택 [!UICONTROL 프로젝트] > [!UICONTROL 계획된 비용] 다음 기준에 따라 이 열 요약 **[!UICONTROL 합계]**.
1. 클릭 **[!UICONTROL 열 추가]** 다시.
1. 선택 [!UICONTROL 프로젝트] > [!UICONTROL 실제 비용] 다음 기준에 따라 이 열 요약 **[!UICONTROL 합계]**.

   ![보고서에 열을 추가하는 화면 이미지](assets/chart-report-columns.png)

1. 다음에서 **[!UICONTROL 그룹화]** 탭, 보고서를 그룹화 기준으로 설정 [!UICONTROL 프로젝트] > [!UICONTROL 이름].

   ![보고서에 그룹화를 추가하는 화면 이미지](assets/chart-report-groupings.png)

1. 다음에서 **[!UICONTROL 필터]** 탭에서 두 개의 필터 규칙을 추가합니다.

   * [!UICONTROL 프로젝트] > [!UICONTROL 상태가 다음과 같음] > [!UICONTROL 완료]
   * [!UICONTROL 프로젝트] >[!UICONTROL  실제 완료 일자] > [!UICONTROL 지난 분기]

   ![보고서에 필터를 추가하는 화면 이미지](assets/chart-report-filters.png)

1. 다음에서 **[!UICONTROL 차트]** 탭, 선택 **[!UICONTROL 열]** 을 참조하십시오.
1. 의 경우 [!UICONTROL 왼쪽(Y) 축], 선택 [!UICONTROL 프로젝트] > [!UICONTROL 계획된 비용].
1. 의 경우 [!UICONTROL 하단(X) 축], 선택 [!UICONTROL 프로젝트] > [!UICONTROL 이름].
1. 다음을 클릭합니다. **[!UICONTROL 혼합형 차트]** 단추 및 선택 [!UICONTROL 프로젝트] > [!UICONTROL 실제 비용] 다음에서 **[!UICONTROL 값]** 필드.
1. 색상 상자 옆에 있는 화살표를 클릭하여 [!UICONTROL 실제 비용] 색상. 나타나는 색상 중 하나를 선택하거나 오른쪽 아래 모서리에 있는 상자를 클릭하여 색상 팔레트를 표시합니다.
1. 클릭 **[!UICONTROL 저장 + 닫기]**. 보고서 이름을 묻는 메시지가 표시되면 &quot;지난 분기에 완료된 프로젝트별 계획된 비용 대 실제 비용&quot;이라고 합니다.

   ![보고서에 차트를 추가하는 화면 이미지](assets/chart-report-chart.png)
