---
title: 이벤트 알림 설정
description: 이벤트 알림을 관리하여 사용자가 받는 이메일 및 인앱 알림을 제어하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
kt: 10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 4%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# 이벤트 알림 설정

>[!NOTE]
>
>단계적 롤아웃으로 인해 시스템 및 그룹 관리자가 이벤트 알림을 관리할 수 있는 기능은 일부 사용자는 일시적으로 사용할 수 없습니다 [!DNL Workfront] 고객. 릴리스에 대한 업데이트를 보려면 이 문서를 따르십시오. 그룹에 대한 이벤트 알림 구성을 잠금 해제합니다.

시스템 관리자는 사용자가 수신해야 하는 알림을 결정합니다 [!DNL Workfront].

![[!UICONTROL 이메일 알림] 창 [!UICONTROL 설정] 영역](assets/admin-fund-notifications-1.png)

다음 [!UICONTROL 이벤트 알림] 목록은 유형별로 그룹화됩니다. 나열된 각 이벤트 알림에 대해 5가지 정보가 표시됩니다.

* **[!UICONTROL 활성] —** 다음 [!UICONTROL 활성] 열에서 시스템 수준의 알림을 켜거나 끌 수 있습니다.
* **[!UICONTROL 이름] —** 내 알림의 이름입니다 [!DNL Workfront].
* **[!UICONTROL 설명] —** 설명은 알림을 트리거하기 위해 발생한 작업 또는 알림 수신에 응답하여 수행해야 하는 작업에 대한 간단한 설명을 제공합니다.
* **[!UICONTROL 이메일 제목] —** 사용자에게 이메일을 보낼 때 제목 줄에 있는 사용자에게 표시되는 내용.
* **[!UICONTROL 그룹 액세스] —** 그룹 관리자가 관리할 수 있도록 알림 잠금을 해제합니다.

## 알림 켜기

전역 시스템 수준에서 알림을 관리하려면 검색 창에 가 표시되는지 확인합니다. [!UICONTROL 시스템 이벤트 알림].

파란색이 표시되도록 전환 단추를 클릭하여 모든 사용자가 사용할 수 있도록 특정 알림을 설정하십시오. 파란색이 숨겨져 있으면 알림이 꺼져 있습니다.

![[!UICONTROL 활성] 열 [!UICONTROL 이메일 알림] 페이지](assets/admin-fund-notifications-2.png)

이벤트 알림을 설정하면 이벤트가 발생할 때 메시지가 즉시 전송됩니다.

## 그룹 관리자 컨트롤 허용

그룹 관리자에게는 시스템 관리자가 그룹 및 하위 그룹이 작동하는 방식과 워크플로우가 무엇인지 여부에 따라 알림 목록을 추가로 사용자 지정할 수 있는 권한이 부여될 수 있습니다.

![[!UICONTROL 그룹 액세스] 열 [!UICONTROL 이메일 알림] 페이지](assets/ganotifications_01.png)

그룹 관리자에게 그룹 및 하위 그룹에 대한 알림을 관리할 수 있는 권한을 제공하려면 시스템 수준 알림 잠금을 해제해야 합니다.

* 이메일 알림 페이지의 이벤트 알림 탭으로 이동합니다.

* 검색 창에 시스템 이벤트 알림이 표시되는지 확인합니다.

* 그룹 액세스 열에서 토글 을 클릭하여 모든 그룹 관리자에 대한 단일 알림 잠금을 해제하면 파란색이 나타납니다.

* 각 알림 왼쪽에 있는 상자를 선택하고 목록 위의 도구 모음에서 잠금 해제 아이콘을 클릭하여 한 번에 여러 개의 알림을 잠금 해제합니다.

![[!UICONTROL 그룹 액세스] 열 [!UICONTROL 이메일 알림] 페이지](assets/ganotifications_02.png)

회색으로 표시되도록 토글을 클릭하여 잠금 해제된 알림을 잠급니다. 확인란을 선택하고 도구 모음에서 잠금 해제 아이콘을 클릭하여 여러 알림을 동시에 잠급니다.

![[!UICONTROL 그룹 액세스] 열 [!UICONTROL 이메일 알림] 페이지](assets/ganotifications_03.png)

잠금 해제된 알림은 최상위 그룹 관리자가 해당 그룹 및 하위 그룹에 이 알림이 필요한지 여부를 확인하는 데 나타납니다. 하위 그룹은 상위 상위 상위 그룹에서 알림 구성을 상속합니다. ﻿


## 그룹 알림 관리

시스템 관리자가 알림 옵션 잠금을 해제하면 그룹 관리자는 왼쪽 패널 메뉴에서 이벤트 알림을 클릭하여 개별 그룹 페이지에서 그룹 알림을 관리할 수 있습니다. 그런 다음 알림 옵션을 활성화하거나 비활성화할 수 있습니다.

![[!UICONTROL 그룹 액세스] 열 [!UICONTROL 이메일 알림] 페이지](assets/managegroupnotifications_01.png)

필요한 경우 시스템 관리자는 창 상단의 검색 표시줄에 그룹 이름을 입력하여 알림 페이지에서 그룹 알림을 관리할 수 있습니다.

![[!UICONTROL 그룹 액세스] 열 [!UICONTROL 이메일 알림] 페이지](assets/managegroupnotifications_02.png)

## 프로 팁

몇 가지 알림이 있습니다 [!DNL Workfront] 는 사용자가 사용할 수 있도록 설정하는 것이 좋습니다.

대부분의 사용자의 경우:

* [!UICONTROL 내 작업 중 하나의 전임 작업이 완료되었습니다.]
* [!UICONTROL 누군가가 지시된 업데이트에 나를 포함시킵니다.]
* [!UICONTROL 내 작업 항목에 대한 댓글]
* [!UICONTROL 지정한 작업의 기한 변경]


프로젝트 관리자 전용:

* [!UICONTROL 현재 진행 중인 프로젝트가 활성화됨]
* [!UICONTROL 내가 소유한 프로젝트가 늦어지고 있습니다.]
* [!UICONTROL 내가 소유한 프로젝트에 문제가 추가됨]
* [!UICONTROL 이정표 작업은 내가 소유한 프로젝트에서 완료됩니다]

<!---
learn more URLs
--->
