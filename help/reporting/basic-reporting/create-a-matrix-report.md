---
title: 매트릭스 보고서 만들기
description: Workfront에서 매트릭스 보고서가 유용할 수 있는 경우 및 매트릭스 보고서를 만드는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
last-substantial-update: 2025-05-20T00:00:00Z
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 62%

---

# 매트릭스 보고서 만들기

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 매트릭스 보고서가 유용할 수 있는 경우
* 매트릭스 보고서를 만드는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on)

## 핵심 사항

* **매트릭스 보고서 구조:** 매트릭스 보고서는 자동 행 및 열 합계를 사용하여 행과 열로 데이터를 구성합니다. &#x200B; 근무 시간, 비용 및 매출과 같은 지표를 추적하는 데 이상적입니다. &#x200B;
* **필터 설정:** 필터를 사용하여 특정 홈 팀의 사용자가 지난 분기 동안 작업한 시간과 같은 특정 데이터에 집중합니다. &#x200B; 소유자 필드 소스는 관련 팀원을 식별하는 데 도움이 됩니다. &#x200B;
* **그룹화 옵션:** 이 예제에서 행은 &quot;소유자 이름&quot;(시간을 사용한 사용자)별로 그룹화되고 열은 &quot;시간 입력 날짜&quot;(월별 및 주별)별로 그룹화됩니다. &#x200B;
* **요약된 데이터:** 시간, 실제 비용 및 매출과 같은 열이 기본적으로 요약되어 합계가 매트릭스에 표시되도록 합니다. 원하는 경우 이러한 기본값을 해제할 수 있습니다. &#x200B;
* **차트 통합:** 매트릭스 보고서를 동일한 그룹화 정보를 사용하여 대체 데이터 시각화를 위한 차트로 보완할 수 있습니다. 매트릭스 탭이나 차트 탭을 기본 보기로 설정할 수 있습니다. &#x200B;

## “매트릭스 보고서 만들기” 활동

### 활동 1: 매트릭스 보고서 만들기

요청 대기열별로 정렬된 각 상태의 요청 수를 보여 주는 매트릭스 보고서를 만듭니다. 수신 작업량과 진행 상황에 대한 빠른 스냅샷을 제공합니다.

요청 대기열을 행 그룹화에 표시하고자 합니다. 상태는 열 그룹화로 나타납니다. 보고서 이름을 “상태 및 요청 대기열별 요청”으로 지정합니다.

### 답변 1

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

1. **[!UICONTROL 저장 및 닫기]**&#x200B;를 클릭합니다. 보고서 이름을 입력하라는 메시지가 표시되면 “상태 및 요청 대기열별 요청”을 입력합니다.

   ![새로운 문제 보고서 필터를 만드는 화면 이미지](assets/matrix-report-filters.png)
