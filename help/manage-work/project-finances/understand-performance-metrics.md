---
title: 성과 지표 이해
description: 성과 지표, 즉 [!UICONTROL 성과 지수 방식]([!UICONTROL PIM]) 및 [!UICONTROL 완료 시 추정치]([!UICONTROL EAC])를 사용하는 방법에 대해 알아봅니다.
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
workflow-type: ht
source-wordcount: '433'
ht-degree: 100%

---

# 성과 지표 이해

프로젝트 관리자가 사용하는 두 가지 성과 지표는 [!UICONTROL 성과 지수 방식]([!UICONTROL PIM]) 및 [!UICONTROL 완료 시 추정치]([!UICONTROL EAC])입니다. 시스템 전체 기본값은 [!DNL Workfront]에서 설정할 수 있으며 새로 만든 프로젝트에 적용됩니다. 그런 다음 개별 프로젝트에서 [!UICONTROL PIM]을 수정할 수 있습니다.

**[!UICONTROL PIM]**

[!UICONTROL PIM]의 설정은 [!DNL Workfront]에서 [!UICONTROL 비용 성과 지수]([!UICONTROL CPI]), [!UICONTROL 비용 일정 성과 지수]([!UICONTROL CSI]), [!UICONTROL 일정 성과 지수]([!UICONTROL SPI]), [!UICONTROL 완료 시 추정치]([!UICONTROL EAC]) 등 다른 프로젝트 성과 지표를 계산하는 방법을 제어합니다.

[!UICONTROL PIM]의 옵션은 시간 기반 및 비용 기반입니다.

* **시간 기반** - Workfront에서 프로젝트의 CPI 및 EAC를 계산할 때 계획된 시간을 사용합니다. 프로젝트의 EAC는 시간 단위의 숫자로 표시됩니다.
* **비용 기반** - Workfront에서 프로젝트의 CPI 및 EAC를 계산할 때 계획된 인건비를 사용합니다. EAC는 통화 값으로 나타납니다. 이 옵션을 사용할 때 작업 할당자(사용자 및/또는 직무 역할)가 비용 요금과 연결되어 있는지 확인하십시오.

**[!UICONTROL EAC]**

[!UICONTROL EAC]는 작업 또는 프로젝트가 완료되었을 때 예상되는 총 비용을 나타냅니다. 옵션은 프로젝트 수준에서 계산되며 작업/하위 작업에서 롤업됩니다.

* **프로젝트 수준에서 계산** - 상위 작업 및 프로젝트의 [!UICONTROL EAC]가 [!UICONTROL EAC] 공식에 실제 시간/실제 인건비를 사용하여 결정됩니다. 계산에 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 경비가 포함됩니다.
* **작업/하위 작업에서 롤업** - 상위 작업 및 프로젝트의 [!UICONTROL EAC]가 각 하위 작업의 [!UICONTROL EAC]를 합쳐 결정됩니다. 이 계산에서 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용은 제외됩니다.

[!UICONTROL EAC] 계산은 [완료 시 추정치 계산(EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=ko-KR)에 나열됩니다.

**성과 지표: 설정**

[!UICONTROL PIM] 및 [!UICONTROL EAC] 시스템 기본값을 설정하려면 다음 작업을 수행하십시오.

1. 메인 메뉴에서 **[!UICONTROL 설정]**&#x200B;을 선택합니다.
1. 왼쪽 패널 메뉴에서 **[!UICONTROL 프로젝트 환경 설정]**&#x200B;을 클릭한 다음 **[!UICONTROL 프로젝트]**&#x200B;를 클릭합니다.
1. [!UICONTROL 프로젝트 상태] 섹션에서 [!UICONTROL 성과 지수 방법]을 찾습니다. ‘시간 기반’ 또는 ‘비용 기반’을 선택합니다.
1. [!UICONTROL 완료 시 추정치]의 경우 ‘프로젝트 수준에서 계산’ 또는 ‘작업/하위 작업에서 롤업’을 선택합니다.
1. 창 하단의 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![[!UICONTROL 프로젝트 환경 설정] 화면의 이미지](assets/setting-up-finances-1.png)

**개별 프로젝트에서 [!UICONTROL PIM] 설정**

1. 프로젝트의 랜딩 페이지로 이동합니다.
1. 왼쪽 패널에서 **[!UICONTROL 프로젝트 세부 정보]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 재무]** 섹션을 엽니다.
1. **[!UICONTROL 성과 지수 방식]** 아래의 텍스트를 더블 클릭하여 편집합니다.
1. ‘시간 기반’ 또는 ‘비용 기반’을 선택합니다.
1. **[!UICONTROL 변경 사항 저장]**&#x200B;을 클릭하여 완료합니다.

![[!UICONTROL 프로젝트 세부 정보] 화면의 이미지](assets/setting-up-finances-2.png)

템플릿 세부 정보의 [!UICONTROL 재무] 섹션에 있는 프로젝트 템플릿에서 [!UICONTROL PIM]을 설정할 수 있습니다.
