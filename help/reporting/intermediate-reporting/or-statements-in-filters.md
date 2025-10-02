---
title: 필터에 OR 구문 만들기
description: Workfront의 유연한 필터 논리를 통해 사용자는 기본 "AND" 규칙, 선택적 "OR" 조건 및 복잡한 기준에 대한 구성된 필터 그룹을 사용하여 보고 보기를 구체화할 수 있습니다.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 31%

---

# 필터에 OR 구문 만들기

이 비디오에서는 Workfront에서 여러 규칙을 사용하여 필터를 만들고 사용하는 방법을 설명합니다. &#x200B; 기본적으로 Workfront은 필터 규칙 사이에 &quot;AND&quot;를 사용합니다. 즉, 항목이 목록에 표시되려면 모든 조건이 true여야 합니다.
또는 필터 논리를 &quot;OR&quot;로 변경하여 조건을 충족하는 항목을 표시할 수 있습니다.
이 비디오에서는 필터 그룹을 사용하여 작업을 위한 필터를 만드는 방법도 보여 줍니다. &#x200B; 예를 들어 늦은 크리에이티브 팀에 할당된 미완료 작업에 대한 그룹과 미할당 크리에이티브 팀에 할당된 미완료 작업에 대한 그룹, 이렇게 두 개의 그룹을 만들 수 있습니다. &#x200B; 각 그룹 내에서 &quot;AND&quot; 논리가 적용되며, 이는 그룹의 모든 조건이 충족되어야 함을 의미합니다. &#x200B; 그룹 간의 &quot;OR&quot; 논리는 두 그룹의 조건에 맞는 작업이 표시되도록 합니다.

>[!VIDEO](https://video.tv.adobe.com/v/3470692/?quality=12&amp;learn=on&amp;enablevpops=0

## OR 필터 활동

사용자에게 할당되었거나 아무에게도 할당되지 않은 미완료 작업을 찾으려 합니다. 아래와 같이 필터를 설정합니다. 이 필터가 원하는 결과를 제공합니까? 그 이유는 무엇입니까?

![부적절하게 생성된 OR 구문 이미지 [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### 답변

아니요. 이 필터는 작업 완결성에 대한 필터 규칙이 OR의 한쪽에만 있으므로 완료되지 않았거나 아무도 할당하지 않은 작업 등 원하는 결과를 제공하지 않습니다.

대신 이 필터는 다음을 표시하는 목록을 생성합니다.

* 완료되지 않은 나에게 할당된 작업.
* **플러스(OR)**
* 상태에 관계없이 할당되지 않은 모든 작업.

필터는 아래와 같아야 합니다. 이 필터에는 OR의 양쪽에 작업 완전성에 대한 필터 규칙이 있습니다.

![적절하게 생성된 OR 구문 이미지 [!DNL Workfront]](assets/or-statement-your-turn-2.png)
