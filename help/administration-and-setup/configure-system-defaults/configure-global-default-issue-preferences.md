---
title: 글로벌 기본 문제 환경 설정 구성
description: 전환된 문제, 실제 날짜 및 문제 액세스에 대한 문제 환경 설정을 지정하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# 글로벌 기본 문제 환경 설정 구성

몇 가지 시스템 전체 설정은 의 특정 상황에서 문제가 작동하는 방식에 대한 기본값을 설정합니다. [!DNL Workfront].

가장 좋은 방법은 글로벌 기본값을 그대로 두고 프로젝트 관리자가 프로젝트 수준 또는 프로젝트 템플릿에서 필요한 조정을 할 수 있도록 하는 것입니다.

글로벌 문제 환경 설정은 조정할 수 있지만, 당신과 당신이 [!DNL Workfront] 컨설턴트는 조직의 워크플로, 프로세스 및 보고 요구 사항에 필요한 설정을 설명합니다. 컨설턴트는 특정 설정이 변경되면 발생하는 상황을 이해하는 데 도움을 줄 수도 있습니다.

문제 환경 설정을 통해 시스템 관리자는 문제를 작업 또는 프로젝트로 전환할 때 옵션, 실제 날짜가 계산되는 방법 및 문제가 할당될 때 프로젝트 액세스 권한을 받는 사용자를 제어할 수 있습니다. 이러한 설정이 어디에 있는지 살펴보겠습니다 [!DNL Workfront].

## 전환된 문제 환경 설정

이러한 설정은에서 작업 또는 프로젝트로 변환될 때 문제가 발생하는 상황을 제어합니다 [!DNL Workfront].

![[!UICONTROL 작업 및 문제] 기본 설정 창 [!UICONTROL 문제] 강조 표시된 섹션](assets/admin-fund-issue-prefs-converting.png)

1. 클릭 **[!UICONTROL 설정]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 확장 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널에서 섹션으로 이동하십시오.
1. 선택 **[!UICONTROL 작업 및 문제]**.
1. 다음으로 스크롤 **[!UICONTROL 문제]** 섹션.
1. 원하는 옵션을 클릭합니다.
1. 완료되면 저장합니다.

이 섹션에서 조직에 적합한 옵션을 선택할 수 있는 옵션을 살펴보겠습니다.

* **[!UICONTROL 해결 중 오브젝트의 상태가 변경되면 해결 가능한 문제 상태를 자동으로 업데이트]**

  이 설정을 사용하면 원래 문제의 해결 방법을 새 개체(작업 또는 프로젝트)의 해결 방법과 상호 연관시킬 수 있습니다.

  이 설정을 활성화(선택)하면 작업 또는 프로젝트 상태와 동일한 상태 키를 가진 사용자 정의 문제 상태를 만들 수 있습니다. 작업 또는 프로젝트(해결 가능한 개체)가 사용자 지정 상태로 설정되면 변경 사항이 문제 상태에도 표시됩니다.

  비활성화되면 해결 중 오브젝트 상태가 사용자 지정 상태가 아닌 기본 상태로 자동 설정됩니다.

  이 설정을 적용하려면 &quot;[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업에 연결]&quot; 옵션을 선택해야 합니다.

* **[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업/프로젝트에 연결]**

  문제가 전환되면 다음이 표시됩니다. [!DNL Workfront] 원래 문제를 유지합니다. 작업 또는 프로젝트의 상태가 변경됨에 따라 문제의 상태가 변경됩니다. 작업 또는 프로젝트가 완료된 것으로 표시되면 문제가 해결된 것으로 표시됩니다.

  이 옵션을 선택하지 않으면 원래 문제는 삭제되고 변환된 작업 또는 프로젝트만 유지됩니다.

  이 설정은 원래 프로젝트에 기록되었거나 을 통해 발생한 문제에 대한 보고에 영향을 줍니다. [!DNL Workfront] 요청 큐.

* **[!UICONTROL 기본 담당자가 작업/프로젝트에 액세스할 수 있도록 허용]**

  이렇게 하면 원래 문제를 만든 사람에게 전환 중에 만든 작업 또는 프로젝트에 액세스할 수 있습니다. 또한 작업을 검토하고 업데이트를 수행한 후 진행 상황을 계속 알 수 있습니다.

* **[!UICONTROL 전환 시 변경되도록 이 설정 허용]**

  이 옵션을 선택하면 의 기본 설정이 사용됩니다.[!UICONTROL 원래 문제 유지]&quot; 및 &quot;[!UICONTROL 기본 담당자 허용]&quot;은 사용자가 문제를 전환하여 변경할 수 있습니다. 기본값을 그대로 유지하려면 이 옵션을 선택 취소합니다.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## 실제 날짜 환경 설정

에는 여러 유형의 날짜가 사용됩니다 [!DNL Workfront]. 실제 날짜는 다음과 같은 &quot;타임스탬프&quot;입니다. [!DNL Workfront] 는 특정 상태가 변경될 때 를 생성합니다.

다음 [!UICONTROL 실제 시작 일자] 타임스탬프는 문제 상태가 신규에서 다른 상태로 변경될 때 생성됩니다. 다음 [!UICONTROL 실제 완료 일자] timestamp는 문제 상태가 마감되었음을 나타내는 상태로 변경되는 경우입니다.

이 환경 설정은 작업과 문제에 대한 실제 날짜 설정을 제어합니다.

![[!UICONTROL 작업 및 문제] 기본 설정 창 [!UICONTROL 실제 일자] 강조 표시된 섹션](assets/admin-fund-issue-prefs-actual-dates.png)

1. 클릭 **[!UICONTROL 설정]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 확장 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널에서 섹션으로 이동하십시오.
1. 선택 **[!UICONTROL 작업 및 문제]**.
1. 다음으로 스크롤 **[!UICONTROL 실제 일자]** 섹션.
1. 에 대해 원하는 옵션을 선택합니다. **[!UICONTROL 실제 시작 일자]** — [!UICONTROL 지금] (현재 날짜 및 시간) 또는 [!UICONTROL 계획된 시작 일자] (다음 [!UICONTROL 실제 시작 일자] 는 문제 세부 정보에 설정된 시작 날짜와 일치합니다.
1. 이제 다음에 대한 옵션을 선택합니다. **[!UICONTROL 실제 완료 일자]** — [!UICONTROL 지금] (현재 날짜 및 시간) 또는 [!UICONTROL 계획된 완료 일자] (다음 [!UICONTROL 실제 시작 일자] 는 문제 세부 정보에 설정된 날짜와 일치합니다.
1. 완료되면 저장합니다.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## 문제 액세스

다음 [!UICONTROL 액세스] 문제 설정은 Workfront에서 문제가 할당되면 사용자에게 부여되는 액세스 권한을 제어합니다. 이러한 설정은 문제가 연결된 프로젝트에 대한 액세스 권한 외에도 문제 자체에 대한 액세스를 제어합니다.

이러한 설정을 변경하기 전에 워크플로우 또는 프로세스 요구 사항에 대해 [!DNL Workfront] 컨설턴트 및 내부 거버넌스 팀

![[!UICONTROL 작업 및 문제] 기본 설정 창 [!UICONTROL 누군가 문제에 할당되었을 때] 강조 표시된 섹션](assets/admin-fund-issue-prefs-access-1.png)

1. 클릭 **[!UICONTROL 설정]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 확장 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널에서 섹션으로 이동하십시오.
1. 선택 **[!UICONTROL 작업 및 문제]**.
1. 다음으로 스크롤 **[!UICONTROL 액세스]** 섹션 및 찾기[!UICONTROL 누군가 문제에 할당되었을 때]&quot; 옵션.
1. 문제 자체에 대한 공유 액세스 권한 설정 — [!UICONTROL 보기], [!UICONTROL 참여], 또는 [!UICONTROL 관리]. [!DNL Workfront] 는 고급 옵션을 그대로 둘 것을 권장합니다.
1. 문제 피할당자도 프로젝트에 액세스할 수 있어야 하는 경우 상자를 선택합니다
1. 그런 다음 프로젝트에 대한 공유 액세스 권한 을 선택합니다. [!UICONTROL 보기], [!UICONTROL 참여], 또는 [!UICONTROL 관리]. 을(를) 설정할 때 [!UICONTROL 고급 옵션], 조직의 워크플로 및 액세스 요구 사항을 염두에 두십시오.
1. 완료되면 저장합니다.

![[!UICONTROL 액세스] 창 표시 [!UICONTROL 참여] 옵션](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
