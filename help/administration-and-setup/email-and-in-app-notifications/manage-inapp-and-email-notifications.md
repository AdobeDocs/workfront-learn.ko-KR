---
title: 인앱 및 이메일 이벤트 알림 관리
description: 사용자가 수신하는 인앱 및 이메일 알림을 제어하여 작업에 관한 유용한 이메일을 수신하는 방법에 대해 알아보십시오.
short-description: 사용자가 수신하는 인앱 및 이메일 알림을 제어하는 방법에 대해 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10095.jpeg
jira: KT-10095
exl-id: 831646d2-ecf8-4fe6-8d4e-8c5fc233ed56
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 13%

---

# 인앱 및 이메일 이벤트 알림 관리

이메일은 일상 생활의 일부이며, 어떤 날에는 받는 이메일의 양이 압도적입니다. 그러나 와 [!DNL Workfront], 시스템 관리자는 모든 사람이 관련된 작업과 관련된 관련성이 있고 유용한 이메일을 수신하는지 확인할 수 있습니다.

Workfront에서 사용자에게 보낼 수 있는 알림에는 몇 가지 유형이 있습니다. 이러한 알림 중 일부는 시스템 수준에서 제어되며 모든 사용자에게 영향을 줍니다. 일부 알림은 일별 요약에서 이메일을 즉시 생성하도록 설정할 수 있습니다. 또는 Workfront 내부에서만 알림을 생성하려면 이메일을 끕니다.

## 이벤트 알림

이벤트는 상태 변경, 댓글 게시 또는 지정과 같은 것으로, 에서는 인앱 알림을 트리거할 수 있습니다. [!DNL Workfront].

![알림 목록](assets/admin-fund-user-notifications-01.png)

그러나 환경 설정에서 옵션을 선택하거나 선택 해제하여 이메일 알림을 받을 이벤트를 결정할 수 있습니다.

이러한 변경 작업을 수행하려면 [!UICONTROL 메인 메뉴].

![의 사용자 이름 [!UICONTROL 메인 메뉴]](assets/admin-fund-user-notifications-02.png)

클릭 [!UICONTROL 편집] 다음에서 [!UICONTROL 자세히] 메뉴 아래의 제품에서 사용할 수 있습니다.

![사용자 프로필 페이지의 메뉴](assets/admin-fund-user-notifications-03.png)

클릭 [!UICONTROL 알림] 다음에서 [!UICONTROL 사용자 편집] 팝업 상자입니다.

![[!UICONTROL 사용자 편집] 창](assets/admin-fund-user-notifications-04.png)

여기에서 즉시, 매일 또는 전혀 수신하지 않을 알림을 결정할 수 있습니다. 여기서 변경한 사항은 사용자에게만 적용되며 Workfront의 다른 사용자에게는 영향을 주지 않습니다.

**[!UICONTROL 일별]**

기본적으로 이메일은 즉시 전송되도록 설정되어 있습니다. 하지만 이메일 알림 빈도를 전환할 수 있습니다. [!UICONTROL 인스턴트] 끝 [!UICONTROL 매일]필요한 정보를 언제 가져오는지 확인할 수 있습니다.

![[!UICONTROL 알림] 섹션 / [!UICONTROL 사용자 편집] 창](assets/admin-fund-user-notifications-05.png)

일별 옵션은 한 이메일에 그날의 이벤트 요약본을 보냅니다. 사용자는에 표시되는 그룹화마다 하나의 이메일을 받습니다. [!UICONTROL 알림] 섹션.

예를 들어 [!UICONTROL 내가 소유한 프로젝트 정보] 섹션에는 매일 이메일 1개가 생성됩니다. [!UICONTROL 조치 필요] 섹션에는 매일 1개의 이메일 등이 생성됩니다.

![[!UICONTROL 일별 요약] 다음에 대한 이메일 [!UICONTROL 내가 소유한 프로젝트 정보]](assets/admin-fund-user-notifications-06.png)

![[!UICONTROL 일별 요약] 다음에 대한 이메일 [!UICONTROL 조치 필요]](assets/admin-fund-user-notifications-07.png)

일별 옵션을 선택하는 것 외에도, 이러한 이메일을 보낼 시간을 설정합니다. 가장 적합한 작업에 따라 다이제스트 이메일은 아침에 출근하기 전 또는 퇴근하기 직전에 전송될 수 있습니다.

![[!UICONTROL 다음 이후 이메일 일일 요약:] 드롭다운 메뉴 [!UICONTROL 사용자 편집] 창](assets/admin-fund-user-notifications-08.png)

**전혀 아님**

마지막 옵션은 이메일 알림을 완전히 끄는 것입니다.

![선택한 알림이 다음으로 꺼짐 [!UICONTROL 사용자 편집] 창](assets/admin-fund-user-notifications-09.png)

이렇게 하려는 경우 이메일을 받지 못하더라도 작업은 여전히 내에서 할당, 주석 처리 및 업데이트되고 있음을 알고 있습니다 [!DNL Workfront]. 모든 알림을 해제하면 알아야 하는 중요한 정보가 누락될 수 있습니다.

다음과 같은 경우가 있습니다. [!DNL Workfront] 사용자가 이메일 알림을 해제하는 것을 보았습니다. 예를 들어 작업의 대부분을 [!DNL Workfront] 모바일 앱에서는 이메일 알림을 끄고 앱을 통해서만 알림을 받을 수 있습니다.

에 관계없이 [!UICONTROL 이벤트 알림] 알림을 수신하기로 결정하는 경우, 알림은 조직의 목표를 위해 수행되는 작업의 성공에 중요합니다.


## Recommendations

다음과 같은 두 가지 알림이 있습니다. [!DNL Workfront] 인스턴트 이메일이든 일별 요약이든 모두 선택된 상태로 두는 것이 좋습니다.

대부분의 사용자의 경우:

* [!UICONTROL 내 작업 중 하나의 전임 작업이 완료되었습니다.]
* [!UICONTROL 누군가가 지시된 업데이트에 나를 포함시킵니다.]
* [!UICONTROL 누군가 내 작업 항목에 주석을 남김]
* [!UICONTROL 나에게 할당된 작업의 기한 변경]


특히 프로젝트 관리자의 경우:

* [!UICONTROL 내가 진행 중인 프로젝트가 활성화됩니다.]
* [!UICONTROL 내가 소유한 프로젝트가 늦어지고 있습니다.]
* [!UICONTROL 내가 소유한 프로젝트에 문제가 추가됨]
* [!UICONTROL 내가 소유한 프로젝트에서 마일스톤 작업이 완료되었습니다.]


<!---
learn more URLs
Email notifications
guide: manage your notifications
--->
