---
title: 매트릭스 보고서 활동 만들기
description: 단계별 지침을 사용하여 매트릭스 보고서를 작성하는 방법을 연습합니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 66%

---

# 매트릭스 보고서 활동 만들기

단계별 지침을 사용하여 매트릭스 보고서를 작성하는 방법을 연습합니다.

## 활동 1: 매트릭스 보고서 만들기

요청 대기열별로 정렬된 각 상태의 요청 수를 보여 주는 매트릭스 보고서를 만듭니다. 이를 통해 들어오는 작업의 양과 이를 얼마나 잘 처리하고 있는지 신속하게 파악할 수 있습니다.

요청 대기열을 행 그룹화에 표시하고자 합니다. 상태는 열 그룹화로 나타납니다. 보고서 이름을 &quot;상태 및 요청 대기열별 요청&quot;으로 지정합니다.

## 답변 1

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 보고서]**&#x200B;를 선택합니다.
1. **[!UICONTROL 새 보고서]** 옵션을 클릭하고 **[!UICONTROL 문제]**&#x200B;를 선택합니다.
1. **[!UICONTROL 그룹화]** 탭으로 이동하여 **[!UICONTROL 매트릭스 그룹화로 전환]**&#x200B;을 클릭합니다.
1. [!UICONTROL 행 그룹화]의 경우, **[!UICONTROL 프로젝트]** > **[!UICONTROL 이름]**&#x200B;을 선택합니다.
1. [!UICONTROL 열 그룹화]의 경우, **[!UICONTROL 문제]** > **[!UICONTROL 상태]**&#x200B;를 선택합니다.

   ![새로운 문제 보고서 그룹화를 만드는 화면 이미지](assets/matrix-report-groupings.png)

1. **[!UICONTROL 필터]** 탭으로 이동합니다.
1. 활성 요청 대기열의 요청만 표시되도록 하려면 다음 필터 규칙을 추가합니다.

   * [!UICONTROL 프로젝트] > [!UICONTROL 동일시된 상태] > [!UICONTROL 같음] > [!UICONTROL 현재]
   * [!UICONTROL 대기열 정의] > [!UICONTROL 공개] > [!UICONTROL 같지 않음] > [!UICONTROL 없음] (공개 옵션 중 하나에 할당된 대기열 정의를 통해 프로젝트가 실제로 요청 대기열이라는 것을 알 수 있음)

1. **[!UICONTROL 저장 및 닫기]**&#x200B;를 클릭합니다. 보고서 이름을 묻는 메시지가 표시되면 &quot;상태 및 요청 대기열별 요청&quot;을 입력합니다.

   ![새로운 문제 보고서 필터를 만드는 화면 이미지](assets/matrix-report-filters.png)
