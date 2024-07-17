---
title: '[!UICONTROL 포트폴리오 최적화 도구]를 사용하여 업무 우선 순위 지정 및 업무 관리'
description: '[!UICONTROL 포트폴리오 최적화 도구]를 사용하여 포트폴리오 내에서 프로젝트의 우선 순위를 지정하고 프로젝트를 관리하는 방법을 알아봅니다.'
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: prioritize-and-manage-work-with-portfolios.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13835
role: User
level: Intermediate
exl-id: b8b91ae8-f0e1-4cab-bf2c-6b8ca9746ea3
source-git-commit: 64789af613bd6b38e58bd2c15df622729b883b22
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 100%

---

# [!UICONTROL 포트폴리오 최적화 도구]를 사용하여 업무 우선 순위 지정 및 업무 관리

포트폴리오에서 각 프로젝트의 [!UICONTROL 비즈니스 사례]에 입력된 정보는 포트폴리오로 롤업되고 [!UICONTROL 포트폴리오 최적화] 섹션의 제목으로 유입됩니다.

[!UICONTROL 비즈니스 사례]](assets/10-portfolio-management9.png)의 정보가 있는 ![[!UICONTROL 포트폴리오 최적화 도구] 영역의 이미지

이제 이 정보를 사용하여 어떤 프로젝트를 빨리 프로덕션에 착수시켜야 하고 어떤 프로젝트는 다음 라운드까지 보류할 수 있는지 분석할 때입니다. 이때 [!UICONTROL 포트폴리오 최적화] 도구가 큰 도움이 됩니다.

[!UICONTROL 포트폴리오 최적화 도구]는 다음과 같은 경우 가장 완벽하게 사용자를 지원할 수 있습니다.

* [!UICONTROL 비즈니스 사례]가 완료되어 모든 프로젝트에 제출되었습니다.
* [!UICONTROL 비즈니스 사례]의 [!UICONTROL 제출] 버튼을 클릭하여 Workfront에서 프로젝트 점수를 계산하도록 합니다.
* 사용자는 선택한 프로젝트의 총 재무 상한을 나타내는 예산을 제공합니다.

## 최적화 기준

[!UICONTROL 포트폴리오 최적화 도구]는 표준 기준 세트를 사용하여 프로젝트를 비교하고 우선 순위를 지정합니다.

그 기준은 다음과 같습니다.

* 저비용
* 높게 정렬
* 높은 값
* 이익 대비 낮은 위험
* 높은 ROI

최적화 아이콘을 클릭하면 각 기준 중 하나와 연결된 슬라이더 막대 세트가 열립니다. 슬라이더를 오른쪽으로 이동하여 우선 순위가 높은 기준을 설정하거나 슬라이더를 왼쪽으로 밀어 우선 순위가 낮은 기준을 설정할 수 있습니다.

[!UICONTROL 비즈니스 사례]](assets/11-portfolio-management10.png)의 정보가 있는 ![[!UICONTROL 포트폴리오 최적화 도구] 영역의 이미지

[!DNL Workfront]에서는 이러한 기준을 사용하여 1에서 100 사이의 프로젝트 점수를 생성합니다. 숫자가 높은 프로젝트는 원하는 포트폴리오 방향과 더 잘 일치함을 나타냅니다.

![프로젝트 점수에 대한 정보가 있는 [!UICONTROL 포트폴리오 최적화 도구]영역의 이미지](assets/12-portfolio-management14.png)

>[!NOTE]
>
>[!UICONTROL 비즈니스 사례]의 모든 섹션을 작성했더라도 반드시 [!DNL Workfront]를 통해 포트폴리오에 [!UICONTROL 비즈니스 사례]를 제출해야 [!UICONTROL 포트폴리오 최적화 도구]에서 프로젝트에 점수를 매깁니다. 제출하지 않은 경우 [!UICONTROL 포트폴리오 최적화 도구]의 [!UICONTROL 점수] 열에 점수 대신 경고 기호가 표시됩니다. 프로젝트 채점에 대한 자세한 내용을 보려면 경고 기호 위로 마우스 커서를 이동합니다.

![[!UICONTROL 포트폴리오 최적화 도구]의 [!UICONTROL 점수] 열에 있는 경고 기호의 이미지.](assets/13-portfolio-management12.png)

## 프로젝트 우선 순위 지정

이제 프로젝트 점수가 매겨졌으므로 목록을 쉽고 빠르게 재구성할 수 있습니다.

[!UICONTROL 점수] 열 헤더를 클릭하면 프로젝트가 다시 정렬되어 최고 점수순 또는 최저 점수순으로 나열됩니다. 번호 왼쪽에 있는 막대 아이콘을 클릭하고 원하는 순서대로 프로젝트를 끌어 놓아 프로젝트의 순서를 수동으로 지정할 수 있습니다.

경우에 따라 비교하고 싶지 않은 프로젝트가 목록에 있을 수 있습니다. 목록에 있는 항목을 보고 싶지 않은 경우 먼저 선택을 취소한 다음 토글을 오른쪽으로 밀어 버튼의 배경이 파란색이 되도록 하면 숨겨집니다. 이러한 프로젝트를 포함시키려면 토글을 왼쪽으로 밀어 회색이 표시되도록 합니다.

![[!UICONTROL 포트폴리오 최적화 도구]에서 선택되지 않은 프로젝트의 이미지.](assets/14-portfolio-management13.png)

이렇게 하면 서로 비교하고자 하는 프로젝트만 볼 수 있습니다. 프로젝트 점수, 필터링 및 정렬을 통해 이제 프로젝트의 우선 순위 기준을 변경해야 하는지 여부에 대해 정보에 입각한 결정을 내릴 수 있습니다.

[!DNL Workfront]에 포트폴리오 및 최적화 도구가 마련되어 있는 이유는 프로젝트의 우선 순위를 지정하는 프로세스를 원활하게 하기 위함입니다. 그러나 제안된 기준을 반드시 사용할 필요는 없습니다. 작업을 시작하거나 기반을 제공하는 정도의 용도로만 도구를 사용해도 괜찮습니다.

그러나 프로젝트가 우선 순위순으로 정리되었고 [!DNL Workfront]에서 우선 순위를 확정할 준비가 된 경우 왼쪽 상단의 **[!UICONTROL 우선 순위 설정]** 버튼을 클릭하면 시스템에서 1부터 프로젝트 번호를 매기고 해당 번호를 사용하여 각 프로젝트의 [!UICONTROL 포트폴리오 우선 순위] 필드를 설정합니다.

해당 숫자를 유지하려면 하단의 **[!UICONTROL 저장]** 버튼을 클릭합니다.

![[!UICONTROL 포트폴리오 최적화 도구]에서 [!UICONTROL 우선 순위 설정] 버튼을 사용하여 프로젝트의 우선 순위를 지정하는 경우의 이미지.](assets/15-portfolio-management15.png)

<!-- 
Pro-tips graphic
-->

* [!UICONTROL 포트폴리오 최적화 도구]를 통해 설정된 프로젝트의 우선 순위를 [!UICONTROL 리소스 플래너]에 표시할 수 있습니다. **[!UICONTROL 설정]** 아이콘을 클릭하고 **[!UICONTROL 포트폴리오 우선 순위 표시]** 옵션을 켭니다. 화면이 새로 고쳐지고 왼쪽 열에 포트폴리오 우선 순위가 표시됩니다. 열 상단의 **[!UICONTROL 순서]** 옵션을 클릭하여 [!UICONTROL 리소스 플래너] 우선 순위와 포트폴리오 우선 순위를 일치시킵니다. 완료되면 반드시 저장하십시오.

  ![[!UICONTROL 리소스 플래너]에 있는 [!UICONTROL 포트폴리오 우선 순위] 열의 이미지.](assets/16-portfolio-management17.png)

## 변경 사항 관리

물론 포트폴리오가 완벽한 해답은 아니지만 우선 순위가 바뀔 때의 고충은 줄여 줄 수 있습니다. 한때 며칠이 걸렸던 일을 이제는 몇 시간 또는 몇 분이면 끝낼 수 있습니다.

새 프로젝트가 포트폴리오에 추가되면 여전히 해당 프로젝트를 분석하고 우선 순위를 지정해야 합니다. [!UICONTROL 비즈니스 사례] 및 최적화 점수를 사용하면 요청된 프로젝트, 계획된 프로젝트 및 현재 프로젝트와 새 프로젝트를 쉽게 비교할 수 있습니다.

![[!UICONTROL 포트폴리오 최적화 도구]에 있는 프로젝트 [!UICONTROL 상태] 열의 이미지.](assets/17-project-management16.png)

비교하는 과정에서 새 프로젝트의 우선 순위가 더 높아야 하는 경우 최적화 점수를 기준으로 목록을 다시 정렬하거나 목록에서 더 높은 위치로 끌어다 놓을 수 있습니다. 완료한 후 **[!UICONTROL 우선 순위 설정]** 버튼을 클릭하고 저장하면 작업이 마무리됩니다.

<!-- Learn more graphic and documentation article links

* Portfolio Optimizer overview 
* Optimize projects in the Portfolio Optimizer 
* Overview of the Portfolio Optimizer score 
* Prioritizing projects in the Portfolio Optimizer

-->
