---
title: 시스템 전체 문제 상태 사용자 지정
description: 문제 상태 이름을 변경하고, 상태에 사용되는 문제 유형을 제어하고, 그룹 수준 사용자 지정을 위해 잠금/잠금 해제 상태를 설정하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 시스템 전체 상태 사용자 지정

[!DNL Workfront] 는 조직의 문제 관리 워크플로우를 수용할 수 있는 다양한 기본 법령을 제공합니다. 이러한 상태의 이름은 조직의 용어와 일치하도록 변경할 수 있습니다. 및 상태를 특정 문제 유형에 지정할 수 있습니다.

필요한 경우 추가 상태를 만들 수 있습니다. 시스템 관리자만 시스템 전체 상태를 만들 수 있습니다. 또한 시스템 관리자는 그룹 관리자가 편집할 수 있는 상태를 제어합니다.

![[!UICONTROL 문제] 탭 [!UICONTROL 동상] 페이지 [!UICONTROL 설정]](assets/admin-fund-all-issue-statuses.png)

## 기존 상태 수정

[!DNL Workfront] 에서는 최소 상태 수를 권장합니다. 따라서 사용자가 적합한 상태를 쉽게 선택하고 더 짧은 상태 목록이 유지되므로

기존 상태를 편집하여 이름, 할당된 문제 유형, 관련 색상 등을 변경할 수 있습니다.

![문제 상태 목록 [!UICONTROL 편집] 강조 표시된 옵션](assets/admin-fund-edit-issue-status.png)

1. 클릭 **[!UICONTROL 설정]** 에서 **[!UICONTROL 기본 메뉴]**.
1. 를 확장합니다. **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널의 섹션에 있는 섹션을 참조하십시오.
1. 선택 **[!UICONTROL 상태]**.
1. 을(를) 선택합니다 **[!UICONTROL 문제]** 탭을 사용하여 [!UICONTROL 시스템 상태] 오른쪽 위 모서리에 표시됩니다.
1. 선택 **[!UICONTROL 기본 목록]** 모든 문제 유형에 대한 상태를 확인합니다. 여기에서 문제 상태를 만들거나 수정합니다.
1. 이름을 바꿀 상태 오른쪽을 마우스로 가리킨 다음 을 클릭합니다 **[!UICONTROL 편집]**.
1. 원하는 대로 상태에 새 이름을 지정하거나 다른 정보를 변경합니다.
1. 이러한 설정이 [!DNL Workfront] 인스턴스.
1. 그룹 관리자가 그룹의 상태만 편집할 수 있도록 하려면 상태를 잠금 해제하십시오.
1. 상태를 적용해야 하는 문제 유형에 대한 확인란을 선택합니다.
1. 클릭 **[!UICONTROL 저장]**.

![새 상태를 만드는 창](assets/admin-fund-edit-issue-status-2.png)

### 상태 지정

일부 상태가 모든 문제 유형에 지정되지는 않을 수 있습니다. 다음 [!UICONTROL 상태] 페이지에는 각 상태를 사용할 수 있는 문제 유형을 보여주는 열이 있습니다.

![상태 페이지의 문제 탭에 강조 표시된 변경 순서](assets/admin-fund-issue-type-statuses.png)


특정 문제 유형에 지정된 상태를 보려면 창 상단에 있는 문제 유형 이름을 클릭하면 됩니다.

![[!UICONTROL 문제] 탭 [!UICONTROL 상태] 강조 표시된 열이 있는 페이지](assets/admin-fund-statuses-issue-type.png)

여기에서 문제를 원하는 순서대로 끌어다 놓을 수 있습니다 [!UICONTROL 상태] 드롭다운 메뉴

상태를 편집하려면 페이지로 돌아가야 합니다 [!UICONTROL 기본 목록].
