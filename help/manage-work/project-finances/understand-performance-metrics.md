---
title: 성능 지표 이해
description: 성능 지표는 다음과 같습니다 [!UICONTROL 성능 인덱스 메서드] ([!UICONTROL PIM]) 및 [!UICONTROL 완료 시 예상] ([!UICONTROL EAC]).
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 성능 지표 이해

프로젝트 관리자가 사용하는 두 개의 성능 지표는 다음과 같습니다 [!UICONTROL 성능 인덱스 메서드] ([!UICONTROL PIM]) 및 [!UICONTROL 완료 시 예상] ([!UICONTROL EAC]). 시스템 전체 기본값은 [!DNL Workfront] 새로 만든 프로젝트에 적용합니다. [!UICONTROL PIM] 그런 다음 개별 프로젝트에서 수정할 수 있습니다.

**[!UICONTROL PIM]**

에 대한 설정 [!UICONTROL PIM] 제어 방법 [!DNL Workfront] 과 같은 다른 프로젝트 성과 지표를 계산합니다. [!UICONTROL 비용 성과 인덱스] ([!UICONTROL CPI]), [!UICONTROL 원가 스케줄 성과 인덱스] ([!UICONTROL CSI]), [!UICONTROL 일정 성능 인덱스] ([!UICONTROL SPI]) 및 [!UICONTROL 완료 시 예상] ([!UICONTROL EAC]).

옵션 [!UICONTROL PIM] 는 시간 기반 및 비용을 기반으로 합니다.

* **시간 기반** — Workfront은 계획된 시간을 사용하여 프로젝트의 CPI 및 EAC를 계산합니다. 프로젝트의 EAC는 시간 단위로 표시됩니다.
* **비용 기반** — Workfront은 프로젝트의 CPI 및 EAC를 계산하는 데 계획된 인건비 비용을 사용합니다. EAC가 통화 값으로 나타납니다. 이 옵션을 사용하는 경우 작업 담당자(사용자 및/또는 작업 역할)가 원가율과 연결되어 있는지 확인합니다.

**[!UICONTROL EAC]**

[!UICONTROL EAC] 작업 또는 프로젝트가 완료될 때 예상되는 총 비용을 나타냅니다. 옵션은 프로젝트 수준에서 계산되며 작업/하위 작업에서 롤업됩니다.

* **프로젝트 수준에서 계산** — [!UICONTROL EAC] 상위 태스크 및 프로젝트의 경우 [!UICONTROL EAC] 공식. 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 비용이 포함됩니다.
* R **작업/하위 작업에서 제거** — [!UICONTROL EAC] 상위 작업 및 프로젝트의 경우 [!UICONTROL EAC] 각 하위 작업에 대해 고려할 수 있습니다. 이 계산은 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용을 제외합니다.

다음 [!UICONTROL EAC] 계산은 &quot;EAC(완료 시 예상 계산)&quot;에 나열되어 있습니다. <!-- link to article -->문서 [!UICONTROL [!DNL Workfront] 1개].

**성능 지표: 설정**

설정하려면 [!UICONTROL PIM] 및 [!UICONTROL EAC] 시스템 기본값:

1. 선택 **[!UICONTROL 설정]** 기본 메뉴에서 사용할 수 있습니다.
1. 클릭 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 패널 메뉴에서 **[!UICONTROL 프로젝트]**
1. 에서 [!UICONTROL 프로젝트 상태] 섹션, 찾기 [!UICONTROL 성능 인덱스 메서드]. 시간 기반 또는 비용 기반 을 선택합니다.
1. 대상 [!UICONTROL 완료 시 예상]을 눌러 프로젝트 레벨에서 계산 또는 작업/하위 작업에서 롤업을 선택합니다.
1. 클릭 **[!UICONTROL 저장]** 창 하단에 있습니다.

![의 이미지 [!UICONTROL 프로젝트 환경 설정] screen](assets/setting-up-finances-1.png)

**설정 [!UICONTROL PIM] 개별 프로젝트**

1. 프로젝트의 랜딩 페이지로 이동합니다.
1. 클릭 **[!UICONTROL 프로젝트 세부 사항]** 왼쪽 패널에서 생성합니다.
1. 를 엽니다. **[!UICONTROL 재무]** 섹션을 참조하십시오.
1. 아래 텍스트를 두 번 클릭합니다 **[!UICONTROL 성능 인덱스 메서드]** 편집
1. 시간 기반 또는 비용 기반 을 선택합니다.
1. 클릭 **[!UICONTROL 저장]** 완료 변경.

![의 이미지 [!UICONTROL 프로젝트 세부 사항] screen](assets/setting-up-finances-2.png)

[!UICONTROL PIM] 프로젝트 템플릿의 [!UICONTROL 재무] 템플릿 세부 정보의 섹션.
