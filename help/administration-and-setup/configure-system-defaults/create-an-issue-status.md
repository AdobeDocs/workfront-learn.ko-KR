---
title: 문제 상태 만들기
description: 조직 워크플로의 요구 사항을 충족하는 문제 상태를 만드는 방법을 알아봅니다.
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
ht-degree: 100%

---

# 문제 상태 만들기

[!DNL Workfront]는 새로운 상태를 만들기 전에 시스템의 기존 문제 상태를 수정할 것을 권장합니다. 이를 통해 유지해야 하는 상태 개수를 제한할 수 있습니다.

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴 패널에서 **[!UICONTROL 프로젝트 환경 설정]** 섹션을 확장합니다.
1. **[!UICONTROL 상태]**&#x200B;를 선택합니다.
1. **[!UICONTROL 문제]** 탭을 선택합니다.
1. 오른쪽 상단 필드가 [!UICONTROL 시스템 상태]로 설정되어 있는지 확인하십시오. 이렇게 하면 [!DNL Workfront] 인스턴스에서 전역적으로 새 상태를 사용할 수 있습니다.
1. 모든 문제 상태를 보려면 **[!UICONTROL 마스터 목록]**&#x200B;을 선택합니다. 여기에서 상태를 만들거나 수정합니다.
1. **[!UICONTROL 새 상태 추가]**&#x200B;를 클릭합니다.
1. 이름, 설명, 색상, 동일어, 키 등 조직에 필요한 필드를 완성합니다.
1. 이 상태를 사용할 수 있는 문제 유형의 확인란을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![[!UICONTROL 상태] 페이지의 새 상태 창](assets/admin-fund-create-issue-status.png)

## 문제 상태 및 그룹 관리자

그룹 관리자는 자신이 관리하는 그룹의 문제 상태를 만들고 사용자 정의할 수 있습니다. 그룹에 약간의 자율성을 제공하여 작업을 계속 진행하는 데 필요한 상태를 제공합니다. 또한 시스템 전체 상태의 긴 목록이 필요하지 않습니다.

시스템 관리자가 사용자 정의를 허용하도록 구성한 경우 그룹 관리자는 기존 상태를 편집할 수 있습니다.

시스템 관리자는 [!UICONTROL 상태] 창의 오른쪽 상단에서 그룹 이름을 선택하여 그룹 상태를 관리할 수 있습니다.

![[!UICONTROL 상태] 페이지의 그룹 목록 메뉴](assets/admin-fund-change-group-master-list.png)

그룹 관리자는 [!UICONTROL 설정] 영역의 [!UICONTROL 그룹] 섹션을 클릭하고 이름을 클릭한 다음 왼쪽 패널 메뉴에서 [!UICONTROL 상태]를 선택하여 그룹을 열 수 있습니다. 문제 탭을 선택하도록 합니다.

[!UICONTROL 그룹] 페이지](assets/admin-fund-group-issue-statuses.png)의 ![[!UICONTROL 상태] 섹션

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
