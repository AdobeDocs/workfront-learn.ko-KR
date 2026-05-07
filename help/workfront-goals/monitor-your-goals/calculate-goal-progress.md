---
title: 목표에 대한 진행률 계산
description: ' [!DNL Workfront Goals]에서 목표에 대한 진행률을 계산하는 방법에 대해 알아봅니다.'
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10119
exl-id: fa7aba9b-503e-4fad-93ee-9b709a839e11
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:12:43.441Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 285
ht-degree: 100%

---

# 목표에 대한 진행률 계산

[!DNL Workfront Goals]는 목표 진행률을 계산하고 다음 정보를 표시합니다.

* **실제 완료율**- 지금까지 실제로 달성된 목표의 완료율입니다. 이 값은 목표와 관련된 모든 진행률 표시기의 평균 완료율입니다.
* **예상 완료율**- 목표를 정시에 완료하기 위해 현재 시점에서 달성해야 하는 목표의 완료율입니다. 이 값은 목표 기간(총 일 수)과 현재 시점(목표 시작 일자 이후 경과된 총 일 수)으로 계산됩니다.
* **진행 상황**- 진행 상황은 목표가 제 시간에 완료될 목표에 도달했는지, 완료되지 않을 위험이 있거나 문제가 있는지를 나타내는 레이블입니다.

![[!DNL Workfront Goals]](assets/13-workfront-goals-percent-complete.png)의 목표 진행 상황의 스크린샷

다음 차트는 목표 진행 상황 레이블과 진행률 사이의 관계를 보여 줍니다.

![목표 진행률 레이블과 진행률 간의 관계를 보여 주는 차트](assets/14-workfront-goals-progress-statuses.jpeg)

목표의 진행 상황은 시스템에 입력한 업데이트를 기반으로 완료에 도달하는 측면에서 목표가 어디에 있는지 파악하는 좋은 방법입니다. 목표에서 활동과 결과를 업데이트하는 것이 매우 중요한 이유입니다. 진행 상황 레이블로 표준화된 상태를 나머지 조직에 전달할 수 있습니다.

![[!DNL Workfront Goals]](assets/15-workfront-goals-progress-bar-code.png)의 다양한 진행 상황 레이블을 다루는 그래픽


>[!TIP]
>
>목표 진행 상황을 계산하는 데 사용되는 공식에 대한 자세한 내용은 [Adobe Workfront Goals의 목표 진행 상황 및 상태 개요](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-goals/goal-management/calculate-goal-progress.html?lang=ko-KR#overview-of-goal-progress-and-threshold)를 참조하십시오.

