---
title: 차트 활동을 사용하여 보고서 만들기
description: 단계별 지침을 사용하여 차트를 사용하여 보고서를 작성하는 방법을 연습합니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 81%

---

# 차트 활동을 사용하여 보고서 만들기

단계별 지침을 사용하여 차트를 사용하여 보고서를 작성하는 방법을 연습합니다.

## 활동 1: 보고서에 차트 추가

분기 말이 다가오고 있으며 최근에 완료된 프로젝트가 예산에 어떻게 고정되어 있는지 확인하려고 합니다. 계획된 비용 및 프로젝트의 실제 비용을 보여 주는 보고서를 만듭니다. 지난 분기에 완료된 프로젝트만 보려고 합니다. 사용자 정의 색상을 사용하여 조합 열 차트를 추가합니다.

## 답변 1

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 보고서]**&#x200B;를 선택합니다.
1. **[!UICONTROL 새 보고서]** 메뉴를 클릭하고 **[!UICONTROL 프로젝트]**&#x200B;를 선택합니다.
1. **[!UICONTROL 열(보기)]** 탭에서 **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 프로젝트] > [!UICONTROL 계획된 비용]을 선택하고 이 열을 **[!UICONTROL 합계]**&#x200B;별로 요약합니다.
1. 다시 **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 프로젝트] > [!UICONTROL 실제 비용]을 선택하고 이 열을 **[!UICONTROL 합계]**&#x200B;별로 요약합니다.

   ![보고서에 열을 추가하는 화면 이미지](assets/chart-report-columns.png)

1. **[!UICONTROL 그룹화]** 탭에서 보고서를 [!UICONTROL 프로젝트] > [!UICONTROL 이름]별로 그룹화하도록 설정합니다.

   ![보고서에 그룹화를 추가하는 화면 이미지](assets/chart-report-groupings.png)

1. **[!UICONTROL 필터]** 탭에서 두 개의 필터 규칙을 추가합니다.

   * [!UICONTROL 프로젝트] > [!UICONTROL 동일시된 상태] > [!UICONTROL 완료]
   * [!UICONTROL 프로젝트] >[!UICONTROL  실제 완료 일자] > [!UICONTROL 지난 분기]

   ![보고서에 필터를 추가하는 화면 이미지](assets/chart-report-filters.png)

1. **[!UICONTROL 차트]** 탭에서 차트 유형에 대한 **[!UICONTROL 열]**&#x200B;을 선택합니다.
1. [!UICONTROL 왼쪽 (Y) 축]의 경우, [!UICONTROL 프로젝트] > [!UICONTROL 계획된 비용]을 선택합니다.
1. [!UICONTROL 하단 (X) 축]의 경우, [!UICONTROL 프로젝트] > [!UICONTROL 이름]을 선택합니다.
1. **[!UICONTROL 조합 차트]** 버튼을 클릭하고 **[!UICONTROL 값]** 필드에서 [!UICONTROL 프로젝트] > [!UICONTROL 실제 비용]을 선택합니다.
1. 색상 상자 옆에 있는 화살표를 클릭하여 [!UICONTROL 실제 비용] 색상을 변경합니다. 표시되는 색상 중 하나를 선택하거나 오른쪽 하단에 있는 상자를 클릭하여 색상 팔레트를 불러옵니다.
1. **[!UICONTROL 저장 및 닫기]**&#x200B;를 클릭합니다. 보고서 이름을 묻는 메시지가 표시되면 이를 &quot;지난 분기에 완료된 프로젝트별 계획된 비용 대 실제 비용&quot;이라고 합니다.

   ![보고서에 차트를 추가하는 화면 이미지](assets/chart-report-chart.png)
