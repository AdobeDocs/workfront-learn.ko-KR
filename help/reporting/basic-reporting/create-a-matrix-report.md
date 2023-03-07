---
title: 매트릭스 보고서 만들기
description: 매트릭스 보고서가 유용한 경우와 Workfront에서 매트릭스 보고서를 만드는 방법을 알아봅니다.
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
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 매트릭스 보고서 만들기

이 비디오에서는 다음 사항에 대해 알아봅니다.

* 매트릭스 보고서가 유용한 경우
* 매트릭스 보고서를 만드는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## 활동: 매트릭스 보고서 만들기

각 상태에 있는 요청 수를 요청 대기열별로 정렬하여 보여 주는 매트릭스 보고서를 만듭니다. 이를 통해 들어오는 작업의 양과 이를 얼마나 잘 처리하고 있는지에 대한 빠른 스냅샷을 얻을 수 있습니다.

행 그룹화에 요청 대기열을 표시합니다. 상태는 열 그룹화로 나타납니다. 보고서 이름을 &quot;상태 및 요청 대기열별 요청&quot;로 지정합니다.

## 답변

1. 선택 **[!UICONTROL 보고서]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 다음을 클릭합니다. **[!UICONTROL 새 보고서]** 옵션 및 선택 **[!UICONTROL 문제]**.
1. 로 이동 **[!UICONTROL 그룹화]** tab 키를 누른 다음 클릭 **[!UICONTROL 매트릭스 그룹화로 전환]**.
1. 대상 [!UICONTROL 행 그룹화], 선택 **[!UICONTROL 프로젝트]** > **[!UICONTROL 이름]**.
1. 대상 [!UICONTROL 열 그룹화], 선택 **[!UICONTROL 문제]** > **[!UICONTROL 상태]**.

   ![새 문제 보고서 그룹화를 만드는 화면 이미지](assets/matrix-report-groupings.png)

1. 로 이동 **[!UICONTROL 필터]** 탭.
1. 활성 요청 대기열에 요청만 표시되도록 하려면 다음 필터 규칙을 추가합니다.

   * [!UICONTROL 프로젝트] > [!UICONTROL 상태가 다음과 같음] > [!UICONTROL 같음] > [!UICONTROL 현재]
   * [!UICONTROL 대기열 정의] > [!UICONTROL 공개] > [!UICONTROL 같지 않음] > [!UICONTROL 없음] (대기열 정의가 공개 옵션 중 하나에 할당되어 프로젝트가 실제로 요청 대기열임을 아는 방법입니다.)

1. 클릭 **[!UICONTROL 저장 + 닫기]**. 보고서 이름을 묻는 메시지가 표시되면 &quot;상태 및 요청 대기열별 요청&quot;을 입력합니다.

   ![새 문제 보고서 필터를 만드는 화면 이미지](assets/matrix-report-filters.png)
