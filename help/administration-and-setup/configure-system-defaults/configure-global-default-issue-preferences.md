---
title: 글로벌 기본 문제 환경 설정 구성
description: 변환된 문제, 실제 날짜 및 문제 액세스에 대한 문제 환경 설정을 지정하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# 글로벌 기본 문제 환경 설정 구성

몇 가지 시스템 전체 설정은 [!DNL Workfront].

가장 좋은 방법은 전역 기본값을 그대로 두고 프로젝트 관리자가 프로젝트 수준이나 프로젝트 템플릿에서 필요한 조정을 수행하도록 하는 것입니다.

글로벌 문제 환경 설정을 조정할 수 있지만, 본인과 귀하가 [!DNL Workfront] 컨설턴트는 조직의 워크플로우, 프로세스 및 보고 요구 사항에 필요한 설정을 설명합니다. 특정 설정이 변경되면 컨설턴트가 어떤 상황이 발생하는지 이해하는 데 도움을 줄 수도 있습니다.

문제 환경 설정을 사용하면 시스템 관리자가 문제를 작업 또는 프로젝트로 변환할 때, 실제 날짜를 계산하는 방법과 문제가 할당될 때 프로젝트 액세스 권한을 받는 사람을 제어할 수 있습니다. 이러한 설정이 있는 위치를 살펴보겠습니다 [!DNL Workfront].

## 변환된 문제 환경 설정

이러한 설정은 [!DNL Workfront].

![[!UICONTROL 작업 및 문제] 기본 설정 창 [!UICONTROL 문제] 강조 표시된 섹션](assets/admin-fund-issue-prefs-converting.png)

1. 클릭 **[!UICONTROL 설정]** 에서 **[!UICONTROL 기본 메뉴]**.
1. 를 확장합니다. **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널의 섹션에 있는 섹션을 참조하십시오.
1. 선택 **[!UICONTROL 작업 및 문제]**.
1. 로 스크롤합니다. **[!UICONTROL 문제]** 섹션을 참조하십시오.
1. 원하는 옵션을 클릭합니다.
1. 완료되면 저장.

조직에 적합한 옵션을 선택할 수 있도록 이 섹션의 옵션을 살펴보겠습니다.

* **[!UICONTROL 객체 변경 해결 상태가 되면 해결 가능 문제 상태를 자동으로 업데이트합니다.]**

   이 설정을 사용하면 원래 문제의 해결 방법을 새 개체(작업 또는 프로젝트)의 해결에 상호 연관시킬 수 있습니다.

   이 설정을 활성화(선택)하면 작업 또는 프로젝트 상태와 동일한 상태 키를 갖는 사용자 지정 문제 상태를 만들 수 있습니다. 작업 또는 프로젝트(확인가능한 개체)가 사용자 지정 상태로 설정되면 변경 사항이 문제 상태에도 표시됩니다.

   비활성화하면 해결 객체 상태가 사용자 지정 객체 대신 기본 상태로 자동 설정됩니다.

   이 설정이 효과를 가지려면 &quot;[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업에 연결합니다]&quot; 옵션을 선택해야 합니다.

* **[!UICONTROL 원래 문제를 그대로 유지하여 작업/프로젝트에 대한 해결 방법을 제공합니다]**

   문제가 전환되면 다음과 같습니다 [!DNL Workfront] 원래 문제를 그대로 유지하려고 합니다. 작업 또는 프로젝트의 상태가 변경될 때 문제 상태가 변경됩니다. 작업 또는 프로젝트가 완료된 것으로 표시되면 문제가 해결된 것으로 표시됩니다.

   이 옵션을 선택하지 않으면 원래 문제가 삭제되고 변환된 작업이나 프로젝트만 유지됩니다.

   이 설정은 원래 프로젝트에 로그온했거나 [!DNL Workfront] 요청 큐.

* **[!UICONTROL 기본 연락처가 작업/프로젝트에 액세스할 수 있도록 허용]**

   이렇게 하면 원래 문제를 만든 사람이 변환 중에 만든 작업이나 프로젝트에 액세스할 수 있습니다. 그들은 그 일을 검토하고, 업데이트하며, 그 진행 상황을 계속 알 수 있다.

* **[!UICONTROL 전환 시 변경되도록 이 설정 허용]**

   이 옵션을 선택하면 &quot;에 대한 기본 설정이 됩니다.[!UICONTROL 원래 문제 유지]&quot; 및 &quot;[!UICONTROL 기본 연락처 허용]문제를 변환하는 사용자가 &quot;를 변경할 수 있습니다. 기본값을 그대로 유지하려면 이 옵션을 선택 취소합니다.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## 실제 날짜 환경 설정

에는 여러 가지 유형의 날짜가 사용됩니다 [!DNL Workfront]. 실제 날짜는 [!DNL Workfront] 특정 상태가 변경될 때 생성됩니다.

다음 [!UICONTROL 실제 시작 날짜] 문제 상태가 새로 작성에서 다른 상태로 변경되면 타임스탬프가 만들어집니다. 다음 [!UICONTROL 실제 완료 날짜] timestamp는 문제 상태가 닫혀 있음을 나타내는 상태로 변경되는 경우입니다.

이 기본 설정은 작업과 문제 모두에 대한 실제 날짜 설정을 제어합니다.

![[!UICONTROL 작업 및 문제] 기본 설정 창 [!UICONTROL 실제 날짜] 강조 표시된 섹션](assets/admin-fund-issue-prefs-actual-dates.png)

1. 클릭 **[!UICONTROL 설정]** 에서 **[!UICONTROL 기본 메뉴]**.
1. 를 확장합니다. **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널의 섹션에 있는 섹션을 참조하십시오.
1. 선택 **[!UICONTROL 작업 및 문제]**.
1. 로 스크롤합니다. **[!UICONTROL 실제 날짜]** 섹션을 참조하십시오.
1. 에 대해 원하는 옵션을 선택합니다 **[!UICONTROL 실제 시작 날짜]** — [!UICONTROL 지금] (현재 날짜 및 시간) 또는 [!UICONTROL 계획 시작 일자] ( [!UICONTROL 실제 시작 날짜] 문제 세부 정보에 설정된 시작 날짜와 일치합니다.)
1. 이제 **[!UICONTROL 실제 완료 날짜]** — [!UICONTROL 지금] (현재 날짜 및 시간) 또는 [!UICONTROL 계획 완료 일자] ( [!UICONTROL 실제 시작 날짜] 문제 세부 정보에 설정된 날짜와 일치합니다.)
1. 완료되면 저장.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## 문제 액세스

다음 [!UICONTROL 액세스] 문제에 대한 설정은 Workfront에서 문제를 지정할 때 사용자에게 부여된 액세스 권한을 제어합니다. 이러한 설정은 문제가 연결된 프로젝트에 액세스할 수 있을 뿐만 아니라 문제 자체에 대한 액세스를 제어합니다.

이러한 설정을 변경하기 전에 [!DNL Workfront] 컨설턴트와 내부 거버넌스 팀

![[!UICONTROL 작업 및 문제] 기본 설정 창 [!UICONTROL ISSUE에 누군가 할당되는 경우] 강조 표시된 섹션](assets/admin-fund-issue-prefs-access-1.png)

1. 클릭 **[!UICONTROL 설정]** 에서 **[!UICONTROL 기본 메뉴]**.
1. 를 확장합니다. **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널의 섹션에 있는 섹션을 참조하십시오.
1. 선택 **[!UICONTROL 작업 및 문제]**.
1. 로 스크롤합니다. **[!UICONTROL 액세스]** 섹션에서 &quot;[!UICONTROL ISSUE에 누군가 할당되는 경우]&quot; 옵션을 선택합니다.
1. 문제 자체에 대한 공유 액세스 설정 — [!UICONTROL 보기], [!UICONTROL Contribute], 또는 [!UICONTROL 관리]. [!DNL Workfront] 고급 옵션을 그대로 둘 것을 권장합니다.
1. 문제 할당자가 프로젝트에 액세스할 수 있어야 하는 경우 상자를 선택합니다
1. 그런 다음 프로젝트에 대한 공유 액세스 를 선택합니다. [!UICONTROL 보기], [!UICONTROL Contribute], 또는 [!UICONTROL 관리]. 를 설정할 때 [!UICONTROL 고급 옵션]조직의 워크플로우 및 액세스 요구 사항을 기억하십시오.
1. 완료되면 저장.

![[!UICONTROL 액세스] 창 표시 [!UICONTROL Contribute] 옵션](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
