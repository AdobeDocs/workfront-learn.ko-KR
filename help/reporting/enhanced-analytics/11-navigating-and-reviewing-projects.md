---
title: 프로젝트 탐색 및 검토 이해
description: '[!UICONTROL 향상된 분석]에서 플라이트 플랜 차트를 읽는 방법을 알아봅니다.'
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8729
recommendations: noDisplay,noCatalog
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
doc-type: video
source-git-commit: 92dd1cf0db8c6ea785cba2f524133273240a6d10
workflow-type: ht
source-wordcount: '459'
ht-degree: 100%

---

# 프로젝트 탐색 및 검토 이해

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 플라이트 플랜 차트를 읽는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on)

## 플라이트 플랜 차트

![An image of a flight plan chart with numbers matching bullets below](assets/section-2-1.png)

차트에는 다음이 표시됩니다.

1. 왼쪽에 표시된 프로젝트 이름.
1. 하단에 표시된 이름.
1. 파란색 세로선은 마우스 커서로 가리키고 있는 특정 일자를 나타냅니다.
1. 파란색 가로선은 프로젝트의 계획된 시작 일자와 종료 일자를 나타냅니다.
1. 녹색 선은 프로젝트가 ‘목표 충족’ 상태임을 나타냅니다.
1. 주황색 선은 프로젝트가 ‘위험 상태’ 상태임을 나타냅니다.
1. 빨간색 선은 프로젝트가 ‘문제 발생’ 상태임을 나타냅니다.

프로젝트에 대한 이 정보를 확인하면 다음과 같은 사항을 결정하는 데 도움이 됩니다.

* 계획된 완료 일자를 초과하여 프로젝트가 연장되도록 하는 이벤트.
* 프로젝트에 문제가 발생하기 시작하는 시점.
* 동일한 기간 동안 진행되는 프로젝트의 수.
* 활성 프로젝트의 수.
* 특별한 관심이나 지원이 필요한 프로젝트.

## 상태는 진행 상태를 기반으로 합니다.

프로젝트 상태는 프로젝트 진행 현황을 시각적으로 표시한 것입니다. Workfront에서는 프로젝트 내 작업의 진행 상태에 따라 상태를 결정합니다.

![An image of possible progress statuses](assets/section-2-2.png)

프로젝트 상태는 다음과 같이 설정될 수 있습니다.

* 프로젝트의 상태 유형이 수동으로 설정된 경우 프로젝트를 관리할 수 있는 액세스 권한이 있는 사용자가 **수동**&#x200B;으로 설정합니다. 이 경우 사용자가 중요 경로와 독립적으로 프로젝트의 상태를 설정할 수 있습니다.
* Workfront에서 프로젝트의 상태 유형이 ‘진행 상태’로 설정된 경우 **자동**&#x200B;으로 설정됩니다.

Workfront에서는 상태 유형을 ‘진행 상태’로 설정하여 작업 진행 상황을 기반으로 프로젝트의 실제 진행 상황을 명확하게 표시할 것을 권장합니다.

![An image of possible progress statuses](assets/section-2-3.png)

‘진행 상태’로 설정하면 프로젝트 상태는 다음과 같을 수 있습니다.

* **목표 충족**—중요 경로에 있는 마지막 작업의 진행 상태가 ‘정시’이면 프로젝트의 상태는 ‘목표 충족’이 됩니다. 프로젝트가 예정대로 완료될 예정입니다.
* **위험 상태**—중요 경로에 있는 마지막 작업의 진행 상태가 ‘늦어짐’ 또는 ‘위험 상태’이면 프로젝트 상태는 ‘위험 상태’입니다. 프로젝트가 늦게 완료될 예정이지만 아직 실제로 늦지는 않았습니다.
* **문제 발생**—중요 경로에 있는 마지막 작업의 진행 상태가 ‘지연’이면 프로젝트 상태는 ‘문제 발생’입니다. 기한이 과거 일자이며 프로젝트가 현재 지연되었습니다.

>[!NOTE]
>
>환경에 맞게 상태를 사용자 정의할 수 있으므로 옵션이 세 가지 이상이거나 옵션의 이름이 위와 다를 수 있습니다. 상태 사용자 정의에 대한 자세한 내용은 [사용자 정의 상태 만들기 또는 편집](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-conditions/create-edit-custom-conditions.html?lang=ko) 문서를 참조하십시오.
