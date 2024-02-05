---
title: 차트로 보고서 만들기
description: Workfront에서 차트로 데이터 시각화를 향상하는 방법과 차트 도구를 사용하는 방법을 알아봅니다.
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
workflow-type: ht
source-wordcount: '327'
ht-degree: 100%

---

# 차트로 보고서 만들기

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 차트로 데이터 시각화를 향상하는 방법
* Workfront의 차트 도구를 사용하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## 활동: 보고서에 차트 추가

분기 말이 다가오고 있으며 최근에 완료된 프로젝트가 예산에 어떻게 고정되어 있는지 확인하려고 합니다. 계획된 비용 및 프로젝트의 실제 비용을 보여 주는 보고서를 만듭니다. 지난 분기에 완료된 프로젝트만 보려고 합니다. 사용자 정의 색상을 사용하여 조합 열 차트를 추가합니다.

## 답변

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
1. **[!UICONTROL 저장 및 닫기]**&#x200B;를 클릭합니다. 보고서 이름을 입력하라는 메시지가 표시되면 “지난 분기에 완료된 프로젝트별 계획된 비용과 실제 비용의 비교”라고 지정합니다.

   ![보고서에 차트를 추가하는 화면 이미지](assets/chart-report-chart.png)
