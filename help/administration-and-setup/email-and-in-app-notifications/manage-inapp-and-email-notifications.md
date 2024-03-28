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
ht-degree: 100%

---

# 인앱 및 이메일 이벤트 알림 관리

이메일은 일상 업무의 일부이며 때로는 많은 양의 이메일을 받게 됩니다. 그러나 시스템 관리자는 [!DNL Workfront]을 통해 모든 사람이 해당 작업과 관련된 유용한 이메일을 받을 수 있도록 합니다.

Workfront에서 사용자에게 보낼 수 있는 여러 유형의 알림이 있습니다. 이러한 알림 중 일부는 시스템 수준에서 제어되며 모든 사용자에게 영향을 미칩니다. 일부 알림은 일 단위 요약에서 즉시 이메일을 생성하도록 설정할 수 있습니다. 또는 Workfront 내에서 알림만 생성하려면 이메일을 끕니다.

## 이벤트 알림

이벤트는 상태 변경, 게시된 댓글 또는 할당과 같은 것으로 [!DNL Workfront]의 인앱 알림을 트리거할 수 있습니다.

![알림 목록](assets/admin-fund-user-notifications-01.png)

그러나 환경 설정에서 옵션을 선택하거나 선택 취소하여 이메일 알림을 받을 이벤트를 결정할 수 있습니다.

변경하려면 [!UICONTROL 메인 메뉴]에서 이름을 클릭합니다.

![[!UICONTROL 메인 메뉴]](assets/admin-fund-user-notifications-02.png)의 사용자 이름

[!UICONTROL 더 보기] 메뉴에서 [!UICONTROL 편집]을 클릭합니다.

![사용자 프로필 페이지의 메뉴](assets/admin-fund-user-notifications-03.png)

[!UICONTROL 사용자 편집]의 팝업 상자에서 [!UICONTROL 알림]을 클릭합니다.

![[!UICONTROL 사용자 편집] 창](assets/admin-fund-user-notifications-04.png)

여기에서 즉시, 일별 또는 전혀 받지 않을 알림을 결정할 수 있습니다. 여기에서 수행하는 모든 변경 사항은 귀하에게만 적용되며 Workfront의 다른 사용자에게 영향을 주지 않습니다.

**[!UICONTROL 일별]**

기본적으로 이메일은 즉시 전송되도록 설정되어 있습니다. 단, 이메일 알림 빈도를 [!UICONTROL 즉시]에서 [!UICONTROL 일별]로 전환하여 필요한 정보를 언제든지 얻을 수 있습니다.

[!UICONTROL 사용자 편집] 창의 ![[!UICONTROL 알림] 섹션](assets/admin-fund-user-notifications-05.png)

일별 옵션은 일별 이벤트 요약을 하나의 이메일로 보냅니다. 사용자는 [!UICONTROL 알림] 섹션에 표시되는 각 그룹화에 대해 하나의 이메일을 받습니다.

예를 들어 [!UICONTROL 내가 소유한 프로젝트에 대한 정보] 섹션에서는 매일 하나의 이메일을 생성하고, [!UICONTROL 필요한 조치] 섹션에서는 매일 하나의 이메일 등을 생성합니다.

[!UICONTROL 내가 소유한 프로젝트에 대한 정보]](assets/admin-fund-user-notifications-06.png)에 대한 ![[!UICONTROL 일별 요약] 이메일

[!UICONTROL 필요한 조치]](assets/admin-fund-user-notifications-07.png)에 대한 ![[!UICONTROL 일별 요약] 이메일

일별 옵션을 선택하는 것 외에도 해당 이메일을 보낼 시간을 설정합니다. 적합성에 따라 요약 이메일은 아침 출근 전이나 퇴근 직전에 전송될 수 있습니다.

[!UICONTROL 사용자 편집] 창의 ![[!UICONTROL 다음 시간 이후에 일별 요약 이메일 보내기] 드롭다운 메뉴](assets/admin-fund-user-notifications-08.png)

**전혀 받지 않음**

마지막 옵션은 이메일 알림을 완전히 끄는 것입니다.

![[!UICONTROL 사용자 편집] 창의 선택한 알림 끄기](assets/admin-fund-user-notifications-09.png)

이 작업을 수행하기로 결정한 경우, 이메일을 받지 않더라도 [!DNL Workfront] 내에서 작업이 계속 할당되고 댓글이 추가되고 업데이트됩니다. 모든 알림을 끄면 알아야 할 중요 정보가 누락될 수 있습니다.

[!DNL Workfront]에서 사용자가 이메일 알림을 끄는 몇 가지 경우가 있습니다. 예를 들어 [!DNL Workfront] 모바일 애플리케이션을 통해 대부분의 작업을 수행하는 경우, 이메일 알림을 끄고 앱을 통해서만 알림을 받을 수 있습니다.

수신하기로 결정한 [!UICONTROL 이벤트 알림]과 상관없이 알림은 조직의 목표를 위해 수행되는 작업의 성공에 중요합니다.


## 추천 항목

[!DNL Workfront]에서 인스턴트 이메일 또는 일별 요약에 대해 선택한 상태로 두는 것을 권장하는 몇 가지 알림이 있습니다.

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
Email notifications
guide: manage your notifications
--->
