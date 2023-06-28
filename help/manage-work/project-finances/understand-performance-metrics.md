---
title: 성능 지표 이해
description: 성능 지표 사용 방법 알아보기 - [!UICONTROL 성과 지표 메서드] ([!UICONTROL PIM]) 및 [!UICONTROL 완료 시 견적] ([!UICONTROL EAC]).
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 성능 지표 이해

프로젝트 관리자가 사용하는 두 가지 성능 지표에는 [!UICONTROL 성과 지표 메서드] ([!UICONTROL PIM]) 및 [!UICONTROL 완료 시 견적] ([!UICONTROL EAC]). 시스템 전체 기본값을 설정할 수 있는 위치: [!DNL Workfront] 및 을 새로 만든 프로젝트에 적용합니다. [!UICONTROL PIM] 그런 다음 개별 프로젝트에서 수정할 수 있습니다.

**[!UICONTROL PIM]**

에 대한 설정 [!UICONTROL PIM] 제어 방법 [!DNL Workfront] 는 과 같은 기타 프로젝트 성능 지표를 계산합니다. [!UICONTROL 원가 성과 지수] ([!UICONTROL CPI]), [!UICONTROL 원가 일정 성과 지수] ([!UICONTROL CSI]), [!UICONTROL 일정 성과 지수] ([!UICONTROL SPI]), 및 [!UICONTROL 완료 시 견적] ([!UICONTROL EAC]).

옵션 [!UICONTROL PIM] 은 시간 기반이며 비용 기반입니다.

* **시간 기반** — Workfront은 계획된 시간을 사용하여 프로젝트의 CPI와 EAC를 계산합니다. 프로젝트의 EAC가 시간 단위로 숫자로 표시됩니다.
* **비용 기반** — Workfront은 프로젝트의 CPI와 EAC를 계산할 때 계획된 인건비를 사용합니다. EAC는 통화 값으로 표시됩니다. 이 옵션을 사용하는 경우 작업 담당자(사용자 및/또는 작업 역할)가 비용 비율과 연결되어 있는지 확인하십시오.

**[!UICONTROL EAC]**

[!UICONTROL EAC] 작업 또는 프로젝트가 완료될 때의 예상 총 비용을 나타냅니다. 옵션은 프로젝트 수준에서 계산되며 작업/하위 작업에서 롤업됩니다.

* **프로젝트 수준에서 계산** — [!UICONTROL EAC] 상위 작업 및 프로젝트의 경우 의 실제 시간/실제 인건비를 사용하여 결정됩니다. [!UICONTROL EAC] 공식. 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 비용이 포함됩니다.
* R **작업/하위 작업에서 올림** — [!UICONTROL EAC] 상위 작업 및 프로젝트에 대한 은(는) [!UICONTROL EAC] 각 하위 작업에 대해. 이 계산에서는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용은 제외됩니다.

다음 [!UICONTROL EAC] 계산은에 나열되어 있습니다 [EAC(완료 시 추정 비용) 계산](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**성능 지표: 설정**

설정 [!UICONTROL PIM] 및 [!UICONTROL EAC] 시스템 기본값:

1. 선택 **[!UICONTROL 설정]** 기본 메뉴에서.
1. 클릭 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 패널 메뉴에서 **[!UICONTROL 프로젝트]**
1. 다음에서 [!UICONTROL 프로젝트 상태] 섹션, 찾기 [!UICONTROL 성과 지표 메서드]. 시간 기반 또는 비용 기반 을 선택합니다.
1. 대상 [!UICONTROL 완료 시 견적]프로젝트 수준에서 계산 또는 작업/하위 작업에서 롤업을 선택합니다.
1. 클릭 **[!UICONTROL 저장]** 창 아래에요.

![의 이미지 [!UICONTROL 프로젝트 환경 설정] 화면](assets/setting-up-finances-1.png)

**설정 [!UICONTROL PIM] 개별 프로젝트에서**

1. 프로젝트의 랜딩 페이지로 이동합니다.
1. 클릭 **[!UICONTROL 프로젝트 세부 정보]** 왼쪽 패널에서 가져옵니다.
1. 를 엽니다. **[!UICONTROL 재무]** 섹션.
1. 아래 텍스트를 두 번 클릭합니다 **[!UICONTROL 성과 지표 메서드]** 을 클릭하여 편집합니다.
1. 시간 기반 또는 비용 기반 을 선택합니다.
1. 클릭 **[!UICONTROL 저장]** 완료할 변경 사항.

![의 이미지 [!UICONTROL 프로젝트 세부 정보] 화면](assets/setting-up-finances-2.png)

[!UICONTROL PIM] 의 프로젝트 템플릿에 설정할 수 있습니다. [!UICONTROL 재무] 섹션에 자세히 설명되어 있습니다.
