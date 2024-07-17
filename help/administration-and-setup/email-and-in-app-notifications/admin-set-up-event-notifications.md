---
title: 이벤트 알림 설정
description: 이벤트 알림을 관리하여 사용자가 수신하는 이메일 및 인앱 알림을 제어하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 100%

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
>단계적 롤아웃으로 인해 일부 [!DNL Workfront] 고객은 시스템 및 그룹 관리자가 이벤트 알림을 관리할 수 있는 기능을 일시적으로 사용할 수 없습니다. 릴리스에 대한 업데이트는 해당 문서(그룹에 대한 이벤트 알림 구성을 잠금 해제)를 참조하십시오.

시스템 관리자는 [!DNL Workfront]를 통해 사용자가 어떤 알림을 받아야 하는지 확인합니다.

[!UICONTROL 설정] 영역의 ![[!UICONTROL 이메일 알림] 창](assets/admin-fund-notifications-1.png)

[!UICONTROL 이벤트 알림] 목록은 유형별로 그룹화됩니다. 나열된 각 이벤트 알림에 대한 다섯 가지 정보가 다음과 같이 표시됩니다.

* **[!UICONTROL 기본] -** [!UICONTROL Active] 열을 사용하면 시스템 전체 수준에서 알림을 켜거나 끌 수 있습니다.
* **[!UICONTROL 이름] -** [!DNL Workfront] 내의 알림 이름입니다.
* **[!UICONTROL 설명] -** 설명에서는 알림을 트리거하기 위해 트리거하는 작업 또는 알림 수신에 대한 응답으로 수행해야 하는 작업에 대한 간략한 설명을 제공합니다.
* **[!UICONTROL 이메일 제목] -** 이메일이 사용자에게 전송될 때 제목 줄에 사용자에게 표시되는 내용입니다.
* **[!UICONTROL 그룹 액세스] -** 그룹 관리자가 관리할 수 있도록 알림 잠금을 해제합니다.

## 알림 켜기

전역 시스템 수준에서 알림을 관리하려면 검색 창에 [!UICONTROL 시스템 이벤트 알림]이 표시되어 있는지 확인합니다

파란색이 표시되도록 전환 버튼을 클릭하여 모든 사용자가 사용할 수 있도록 특정 알림을 켭니다. 파란색이 숨겨져 있으면 알림이 꺼진 것입니다.

[!UICONTROL 이메일 알림] 페이지의 ![[!UICONTROL 활성] 열](assets/admin-fund-notifications-2.png)

이벤트 알림을 켜면 이벤트가 발생하는 즉시 메시지가 전송됩니다.

## 그룹 관리자 제어 허용

시스템 관리자는 그룹 관리자가 부여하는 권한을 사용하여 그룹 및 하위 그룹의 기능과 워크플로에 따라 알림 목록을 추가로 사용자 정의할 수 있습니다.

[!UICONTROL 이메일 알림] 페이지의 ![[!UICONTROL 그룹 액세스] 열](assets/ganotifications_01.png)

그룹 관리자에게 그룹 및 하위 그룹에 대한 알림을 관리할 수 있는 기능을 제공하려면 시스템 수준 알림을 잠금 해제해야 합니다.

* 이메일 알림 페이지의 이벤트 알림 탭으로 이동합니다.

* 검색 창에 시스템 이벤트 알림이 표시되는지 확인합니다.

* 그룹 액세스 열의 토글을 클릭하여 파란색이 표시되도록 모든 그룹 관리자에 대한 단일 알림을 잠금 해제합니다.

* 각 알림 왼쪽에 있는 상자를 선택하고 목록 위의 도구 모음에서 잠금 해제 아이콘을 클릭하여 여러 알림을 한 번에 잠금 해제합니다.

[!UICONTROL 이메일 알림] 페이지의 ![[!UICONTROL 그룹 액세스] 열](assets/ganotifications_02.png)

회색이 표시되도록 토글을 클릭하여 잠금 해제된 알림을 잠급니다. 확인란을 선택하고 도구 모음에서 잠금 해제 아이콘을 클릭하여 동시에 여러 알림을 잠급니다.

[!UICONTROL 이메일 알림] 페이지의 ![[!UICONTROL 그룹 액세스] 열](assets/ganotifications_03.png)

잠금 해제된 알림은 그룹 및 하위 그룹에 해당 알림이 필요한지 여부를 확인할 수 있도록 최상위 그룹 관리자에게 표시됩니다. 하위 그룹은 최상위 그룹에서 알림 구성을 상속합니다. ﻿


## 그룹 알림 관리

시스템 관리자가 알림 옵션을 잠금 해제하면 그룹 관리자는 왼쪽 패널 메뉴에 있는 이벤트 알림을 클릭하여 개별 그룹 페이지에서 그룹 알림을 관리할 수 있습니다. 그런 다음 알림 옵션을 활성화하거나 비활성화할 수 있습니다.

[!UICONTROL 이메일 알림] 페이지의 ![[!UICONTROL 그룹 액세스] 열](assets/managegroupnotifications_01.png)

필요한 경우, 시스템 관리자는 창 상단의 검색 창에 그룹 이름을 입력하여 알림 페이지에서 그룹 알림을 관리할 수 있습니다.

[!UICONTROL 이메일 알림] 페이지의 ![[!UICONTROL 그룹 액세스] 열](assets/managegroupnotifications_02.png)

## 전문가 팁

사용자가 사용할 수 있도록 [!DNL Workfront]에서 권장하는 몇 가지 알림이 있습니다.

대부분의 사용자:

* [!UICONTROL 내 작업 중 하나의 전임 작업이 완료되었습니다.]
* [!UICONTROL 누군가가 지시된 업데이트에 나를 포함시킵니다.]
* [!UICONTROL 누군가 내 작업 항목에 댓글을 남김]
* [!UICONTROL 나에게 할당된 작업의 기한 변경]


프로젝트 관리자:

* [!UICONTROL 내가 진행 중인 프로젝트가 활성화됨]
* [!UICONTROL 내가 소유한 프로젝트가 늦어지고 있습니다.]
* [!UICONTROL 내가 소유한 프로젝트에 문제가 추가됨]
* [!UICONTROL 내가 소유한 프로젝트에서 마일스톤 작업이 완료됨]

<!---
learn more URLs
--->
