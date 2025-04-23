---
title: 전역 기본 문제의 환경 설정 구성
description: 전환된 문제, 실제 일자 및 문제 액세스에 대한 문제 환경 설정을 지정하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 75%

---

# 전역 기본 문제의 환경 설정 구성

여러 시스템 전체 설정은 [!DNL Workfront]의 특정 상황에서 문제가 동작하는 방식에 대한 기본값을 설정합니다.

모범 사례는 전역 기본값을 그대로 두고 프로젝트 관리자가 프로젝트 수준 또는 프로젝트 템플릿에서 필요한 조정을 할 수 있도록 하는 것입니다.

전역 문제 환경 설정을 조정할 수 있지만 귀하와 [!DNL Workfront] 컨설턴트가 조직의 워크플로, 프로세스 및 보고 요구 사항에 필요한 설정을 논의하는 것이 좋습니다. 컨설턴트는 또한 특정 설정이 변경되면 어떻게 되는지 이해하는 데 도움을 줄 수 있습니다.

문제 환경 설정을 사용하면 문제가 작업 또는 프로젝트로 전환될 때 옵션, 실제 일자 계산 방법, 문제가 할당될 때 프로젝트에 액세스할 수 있는 사람을 시스템 관리자가 제어할 수 있습니다. 해당 설정이 [!DNL Workfront]에서 어디에 있는지 살펴보겠습니다.

## 전환된 문제 환경 설정

이러한 설정은 [!DNL Workfront]에서 작업 또는 프로젝트로 변환될 때 문제가 발생하는 상황을 제어합니다.

[!UICONTROL 문제] 섹션이 강조 표시된 ![[!UICONTROL 작업 및 문제] 환경 설정 창](assets/admin-fund-issue-prefs-converting.png)

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴 패널에서 **[!UICONTROL 프로젝트 환경 설정]** 섹션을 확장합니다.
1. **[!UICONTROL 작업 및 문제]**&#x200B;를 선택합니다.
1. **[!UICONTROL 문제]** 섹션으로 스크롤합니다.
1. 원하는 옵션을 클릭합니다.
1. 완료되면 저장합니다.

이 섹션의 옵션을 살펴보면서 조직에 적합한 옵션을 선택할 수 있습니다.

* **[!UICONTROL 해결 중 오브젝트의 상태가 변경되면 해결 가능한 문제 상태를 자동으로 업데이트]**

  이 설정을 사용하면 원래 문제의 해결을 새 오브젝트(작업 또는 프로젝트)의 해결과 연관시킬 수 있습니다.

  이 설정을 활성화(선택)하면 작업 또는 프로젝트 상태와 상태 키가 동일한 사용자 정의 문제 상태를 생성할 수 있습니다. 작업 또는 프로젝트(해결 가능한 오브젝트)가 사용자 정의 상태로 설정되면 변경 사항이 문제 상태에도 표시됩니다.

  비활성화하면 해결 중인 오브젝트 상태가 사용자 정의 상태가 아닌 기본 상태로 자동 설정됩니다.

  이 설정을 적용하려면 &quot;[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업에 연결]&quot; 옵션을 선택해야 합니다.

* **[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업/프로젝트에 연결]**

  문제가 전환되면 [!DNL Workfront]에서 기본적으로 원래 문제를 유지합니다. 작업 또는 프로젝트의 상태가 변경되면 문제의 상태가 변경됩니다. 작업 또는 프로젝트가 완료된 것으로 표시되면 문제가 해결된 것으로 표시됩니다.

  이 옵션을 선택하지 않으면 원래 문제가 삭제되며 전환된 작업 또는 프로젝트만 남습니다.

  이 설정은 원래 프로젝트에 기록된 문제 또는 [!DNL Workfront] 요청 대기열을 통해 발생한 문제에는 영향을 미치지 않습니다.

* **[!UICONTROL 기본 담당자가 작업/프로젝트에 액세스할 수 있도록 허용]**

  이렇게 하면 원본 문제를 만든 사람이 전환 중에 만들어진 작업 또는 프로젝트에 액세스할 수 있습니다. 작업을 검토하고, 업데이트하고, 진행 상황을 알 수 있습니다.

* **[!UICONTROL 전환 시 변경되도록 이 설정 허용]**

  이 옵션을 선택하면 문제를 전환하는 사용자가 &quot;[!UICONTROL 원래 문제 유지]&quot; 및 &quot;[!UICONTROL 기본 연락처 허용]&quot;에 대한 기본 설정을 변경할 수 있습니다. 기본값을 변경하지 않고 유지하려면 이 옵션을 선택 취소하십시오.

<!--
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
-->

## 실제 일자 환경 설정

[!DNL Workfront] 전체에서 여러 유형의 일자가 사용됩니다. 실제 날짜는 특정 상태가 변경될 때 [!DNL Workfront]에서 생성하는 &quot;타임스탬프&quot;입니다.

문제 상태가 ‘신규’에서 다른 상태로 변경되면 [!UICONTROL 실제 시작 일자] 타임스탬프가 만들어집니다. [!UICONTROL 실제 완료 일자] 타임스탬프는 문제 상태가 종료를 나타내는 상태로 변경된 때입니다.

이 환경 설정은 작업과 문제에 대한 실제 날짜 설정을 제어합니다.

[!UICONTROL 실제 일자] 섹션이 강조 표시된 ![[!UICONTROL 작업 및 문제] 환경 설정 창](assets/admin-fund-issue-prefs-actual-dates.png)

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴 패널에서 **[!UICONTROL 프로젝트 환경 설정]** 섹션을 확장합니다.
1. **[!UICONTROL 작업 및 문제]**&#x200B;를 선택합니다.
1. **[!UICONTROL 실제 일자]** 섹션으로 스크롤합니다.
1. **[!UICONTROL 실제 시작 일자]**&#x200B;에 대해 [!UICONTROL 지금] (현재 일자 및 시간) 또는 [!UICONTROL 계획된 시작 일자] 중 원하는 옵션을 선택합니다([!UICONTROL 실제 시작 일자]는 문제 세부 정보에 설정된 시작 일자와 일치).
1. 그리고 **[!UICONTROL 실제 완료 일자]**&#x200B;에 대해 [!UICONTROL 지금] (현재 일자 및 시간) 또는 [!UICONTROL 계획된 완료 일자] 중 옵션을 선택합니다([!UICONTROL 실제 시작 일자]는 문제 세부 정보에 설정된 시작 일자와 일치).
1. 완료되면 저장합니다.


<!--
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
-->

## 문제 액세스

문제에 대한 [!UICONTROL 액세스] 설정은 Workfront에서 문제를 할당할 때 사용자에게 부여되는 액세스 권한을 제어합니다. 이러한 설정은 문제와 연결된 프로젝트에 대한 액세스 외에도 문제 자체에 대한 액세스를 제어합니다.

이러한 설정을 변경하기 전에 워크플로 또는 프로세스 요구 사항에 대해 [!DNL Workfront] 컨설턴트 및 내부 거버넌스 팀과 논의하십시오.

[!UICONTROL 사용자가 문제에 할당될 때] 섹션이 강조 표시된 ![[!UICONTROL 작업 및 문제] 환경 설정 창](assets/admin-fund-issue-prefs-access-1.png)

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴 패널에서 **[!UICONTROL 프로젝트 환경 설정]** 섹션을 확장합니다.
1. **[!UICONTROL 작업 및 문제]**&#x200B;를 선택합니다.
1. **[!UICONTROL 액세스]** 섹션으로 스크롤하여 &quot;[!UICONTROL 누군가 문제에 할당되었을 때]&quot; 옵션을 찾습니다.
1. 문제 자체에 대한 공유 액세스 권한을 [!UICONTROL 보기], [!UICONTROL 기여] 또는 [!UICONTROL 관리] 중에서 선택합니다. [!DNL Workfront]의 권장 사항은 고급 옵션을 그대로 두는 것입니다.
1. 문제 할당자도 프로젝트에 액세스할 수 있어야 하는 경우 확인란을 선택합니다.
1. 그런 다음 프로젝트에 대한 공유 액세스 권한을 [!UICONTROL 보기], [!UICONTROL 기여] 또는 [!UICONTROL 관리] 중에서 선택합니다. [!UICONTROL 고급 옵션]을 설정할 때 조직의 워크플로 및 액세스 요구 사항을 염두에 두십시오.
1. 완료되면 저장합니다.

[!UICONTROL 기여] 옵션을 보여 주는 ![[!UICONTROL 액세스] 창](assets/admin-fund-issue-prefs-access-2.png)

<!--
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
-->
