---
title: 매트릭스 보고서 만들기
description: 매트릭스 보고서가 유용할 수 있는 시기와 Workfront에서 매트릭스 보고서를 만드는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 매트릭스 보고서 만들기

이 비디오에서는 다음을 학습합니다.

* 매트릭스 보고서가 유용할 때
* 매트릭스 보고서를 만드는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on)

## 활동: 매트릭스 보고서 만들기

요청 큐별로 정렬된 각 상태에 있는 요청의 수를 보여주는 매트릭스 보고서를 만듭니다. 이렇게 하면 들어오는 작업의 양과 그에 따라 얼마나 잘 대처하고 있는지에 대한 빠른 스냅숏이 제공됩니다.

요청 큐를 행 그룹에 표시할 수 있습니다. 상태는 열 그룹으로 나타납니다. 보고서 이름을 &quot;상태별 요청 및 요청 큐&quot;로 지정합니다.

## 답변

1. 선택 **[!UICONTROL 보고서]** 에서 **[!UICONTROL 기본 메뉴]**.
1. 을(를) 클릭합니다. **[!UICONTROL 새 보고서]** 옵션을 선택하고 **[!UICONTROL 문제]**.
1. 로 이동합니다. **[!UICONTROL 그룹화]** 탭을 클릭하고 **[!UICONTROL Matrix Grouping으로 전환]**.
1. 대상 [!UICONTROL 행 그룹화], 선택 **[!UICONTROL 프로젝트]** > **[!UICONTROL 이름]**.
1. 대상 [!UICONTROL 열 그룹화], 선택 **[!UICONTROL 문제]** > **[!UICONTROL 상태]**.

   ![새 문제 보고서 그룹을 만드는 화면의 이미지입니다](assets/matrix-report-groupings.png)

1. 로 이동합니다. **[!UICONTROL 필터]** 탭.
1. 활성 요청 큐에 요청만 표시되도록 하려면 다음 필터 규칙을 추가하십시오.

   * [!UICONTROL 프로젝트] > [!UICONTROL 상태] > [!UICONTROL Equal] > [!UICONTROL 현재]
   * [!UICONTROL 큐 정의] > [!UICONTROL 공용] > [!UICONTROL 같지 않음] > [!UICONTROL 없음] (이것은 공개 옵션 중 하나에 할당되는 큐 정의에 의해 프로젝트가 실제로 요청 큐임을 아는 방법입니다.)

1. 클릭 **[!UICONTROL 저장 + 닫기]**. 보고서 이름을 묻는 메시지가 표시되면 &quot;Requests by Status and Request Queue&quot;를 입력합니다.

   ![새 문제 보고서 필터를 만드는 화면의 이미지입니다](assets/matrix-report-filters.png)
