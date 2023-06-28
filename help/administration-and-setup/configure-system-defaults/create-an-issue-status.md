---
title: 문제 상태 만들기
description: 조직 워크플로의 요구 사항을 충족하기 위해 문제 상태를 만드는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# 문제 상태 만들기

[!DNL Workfront] 는 새 상태를 만들기 전에 시스템의 기존 문제 상태를 수정할 것을 권장합니다. 이렇게 하면 유지 관리해야 하는 상태의 수를 제한하는 데 도움이 됩니다.

1. 클릭 **[!UICONTROL 설정]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 확장 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널에서 섹션으로 이동하십시오.
1. 선택 **[!UICONTROL 상태]**.
1. 다음 항목 선택 **[!UICONTROL 문제]** 탭.
1. 오른쪽 위의 필드가 로 설정되어 있는지 확인합니다. [!UICONTROL 시스템 상태]. 이렇게 하면 새 상태를 전체적으로 사용할 수 있습니다. [!DNL Workfront] 인스턴스.
1. 선택 **[!UICONTROL 기본 목록]** 모든 문제 상태를 봅니다. 여기서 상태를 만들거나 수정합니다.
1. 클릭 **[!UICONTROL 새 상태 추가]**.
1. 이름, 설명, 색상, 같음, 키 등 조직에 필요한 필드를 작성합니다.
1. 이 상태에서 사용할 수 있는 문제 유형의 확인란을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![의 새 상태 창 [!UICONTROL 상태] 페이지](assets/admin-fund-create-issue-status.png)

## 문제 상태 및 그룹 관리자

그룹 관리자는 자신이 관리하는 그룹에 대한 문제 상태를 만들고 사용자 지정할 수 있습니다. 이를 통해 그룹에 자율성을 부여하여 작업을 계속 진행해야 하는 상태를 제공할 수 있습니다. 또한 시스템 전체 상태에 대한 긴 목록이 필요하지 않습니다.

시스템 관리자가 사용자 지정을 허용하도록 구성한 경우 그룹 관리자는 기존 상태를 편집할 수 있습니다.

시스템 관리자는 의 오른쪽 상단에서 그룹 이름을 선택하여 그룹의 상태를 관리할 수 있습니다. [!UICONTROL 상태] 창.

![그룹 목록 메뉴 [!UICONTROL 상태] 페이지](assets/admin-fund-change-group-master-list.png)

그룹 관리자는 [!UICONTROL 그룹] 의 섹션 [!UICONTROL 설정] 영역을 클릭하고 이름을 클릭한 다음 을 선택하여 그룹을 엽니다. [!UICONTROL 상태] 왼쪽 패널 메뉴에서 을 클릭합니다. 문제 탭을 선택해야 합니다.

![[!UICONTROL 상태] 섹션 / [!UICONTROL 그룹] 페이지](assets/admin-fund-group-issue-statuses.png)

<!---
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
--->

<!---
learn more URLs
Issue statuses
Create and customize system-wide statuses
--->
