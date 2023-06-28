---
title: 시스템 전체 문제 상태 사용자 지정
description: 문제 상태 이름을 변경하고, 상태가 사용되는 문제 유형을 제어하고, 그룹 수준 사용자 지정에 대한 상태를 잠금/잠금 해제하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 시스템 전체 상태 사용자 정의

[!DNL Workfront] 는 조직의 문제 관리 워크플로우를 수용할 수 있는 다양한 기본 설정을 제공합니다. 이러한 상태는 조직의 용어와 일치하도록 이름을 변경할 수 있습니다. 및 상태를 특정 문제 유형에 할당할 수 있습니다.

필요한 경우 추가 상태를 생성할 수 있습니다. 시스템 관리자만 시스템 전체 상태를 만들 수 있습니다. 또한 시스템 관리자는 그룹 관리자가 편집할 수 있는 상태를 제어합니다.

![[!UICONTROL 문제] 탭 [!UICONTROL 조각상] 페이지 위치 [!UICONTROL 설정]](assets/admin-fund-all-issue-statuses.png)

## 기존 상태 수정

[!DNL Workfront] 은(는) 최소 상태 수를 권장합니다. 이렇게 하면 사용자가 올바른 상태를 더 쉽게 선택할 수 있으며 유지 관리할 상태 목록이 더 짧아집니다.

기존 상태를 편집하여 이름, 할당된 문제 유형, 관련 색상 등을 변경할 수 있습니다.

![문제 상태 목록 [!UICONTROL 편집] 강조 표시된 옵션](assets/admin-fund-edit-issue-status.png)

1. 클릭 **[!UICONTROL 설정]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 확장 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널에서 섹션으로 이동하십시오.
1. 선택 **[!UICONTROL 상태]**.
1. 다음 항목 선택 **[!UICONTROL 문제]** tab을 사용하여 [!UICONTROL 시스템 상태] 오른쪽 위 모서리에 표시됩니다.
1. 선택 **[!UICONTROL 기본 목록]** 모든 문제 유형에 대한 상태를 봅니다. 여기에서 문제 상태를 만들거나 수정합니다.
1. 이름을 바꿀 상태의 오른쪽에 마우스를 가져다 대고 을 클릭합니다 **[!UICONTROL 편집]**.
1. 원하는 대로 상태에 새 이름을 지정하거나 다른 정보를 변경합니다.
1. 이 설정이 의 모든 사용자에게 적용되어야 하는 경우 상태를 잠급니다. [!DNL Workfront] 인스턴스.
1. 그룹 관리자가 그룹에 대해서만 상태를 편집할 수 있도록 상태 잠금을 해제합니다.
1. 상태를 적용할 문제 유형의 상자를 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![새 상태를 만들기 위한 창](assets/admin-fund-edit-issue-status-2.png)

### 상태 할당

모든 상태가 모든 문제 유형에 지정되지는 않을 수 있습니다. 다음 [!UICONTROL 상태] 페이지에는 각 상태를 사용할 수 있는 문제 유형을 보여주는 열이 있습니다.

![상태 페이지의 문제 탭에서 강조 표시된 순서 변경](assets/admin-fund-issue-type-statuses.png)


특정 문제 유형에 지정된 상태만 보려면 창 상단의 문제 유형 이름을 클릭하면 됩니다.

![[!UICONTROL 문제] 탭 / [!UICONTROL 상태] 강조 표시된 열이 있는 페이지](assets/admin-fund-statuses-issue-type.png)

여기에서 문제를 다음에 표시할 순서로 끌어다 놓을 수 있습니다. [!UICONTROL 상태] 드롭다운 메뉴.

상태를 편집하려면 다음으로 돌아가야 합니다. [!UICONTROL 기본 목록].
