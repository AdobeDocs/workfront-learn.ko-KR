---
title: 요청 대기열에 문제 승인 프로세스 적용
description: 기본 승인 프로세스를 구현하여 요청 워크플로를 간소화함으로써 승인된 요청의 상태가 "새로 만들기"로 적절하게 변경되도록 합니다. "해결되지 않음"으로 상태 변경을 선택하여 거부된 요청에 대한 혼동을 해결합니다.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: 3fc3a58c829769ca06ffb93971ac75516dfbd5f2
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 6%

---

# 요청 대기열에 문제 승인 프로세스 적용

>[!PREREQUISITES]
>
>* [요청 흐름 만들기](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [전역 및 일회용 승인 프로세스 만들기](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


이 비디오에서는 요청 대기열을 만들 때 기본 승인 프로세스를 적용하는 프로세스에 대해 설명합니다. &#x200B; 요청이 만들어지면 &quot;신규 - 승인 보류 중&quot; 상태로 시작되고 지정된 승인자에게 승인 알림이 전송됩니다. &#x200B; 승인되면 상태가 &quot;신규&quot;로 변경되어 할당된 개인이 작업을 시작할 수 있습니다. &#x200B; 거부된 경우 승인 프로세스 설정의 일반적인 실수로 인해 상태가 &quot;신규&quot;로 잘못 되돌릴 수 있습니다. &#x200B;
이 비디오에서는 상태가 새 요청의 기본값인 &quot;새로 만들기&quot;로 설정되면 승인 프로세스가 트리거됨을 강조합니다. &#x200B; 거부되면 시스템은 기본적으로 상태를 이전 상태로 다시 변경하는 것으로 설정되며, 이는 새 요청에 이상적이지 않습니다. &#x200B; 대신 &quot;해결되지 않음&quot;과 같은 다른 상태를 선택해야 합니다. &#x200B; 또한 기본적으로 제공되는 &quot;거부됨&quot; 상태는 없지만 시스템 관리자가 필요한 경우 만들 수 있습니다. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops)

## 핵심 사항

* **기본 승인 프로세스:** 요청 대기열을 만들 때 각 요청에 자동으로 승인 워크플로를 할당하는 기본 승인 프로세스를 적용할 수 있습니다.
* **승인 시 상태 변경:** 승인된 요청의 상태가 &quot;새로 만들기 - 승인 보류 중&quot;에서 &quot;새로 만들기&quot;로 변경되어 할당된 개인이 작업을 시작할 수 있습니다.
* **거부 처리에 일반적인 오류:** 요청이 거부되면 승인 프로세스의 기본 시스템 설정으로 인해 상태가 &quot;새로 만들기&quot;로 되돌아갑니다.
* **거부된 요청에 대한 권장 상태:** 이전 상태(&quot;새로 만들기&quot;)로 되돌리지 않고, 혼동을 방지하기 위해 &quot;해결되지 않음&quot;과 같은 다른 상태를 선택하는 것이 좋습니다.
* **사용자 지정 상태 옵션:** 기본적으로 제공되는 &quot;거부됨&quot; 상태가 없지만, 승인 프로세스를 더 명확하게 하기 위해 필요한 경우 시스템 관리자가 만들 수 있습니다.


## 이 주제와 관련된 추천 튜토리얼

* [작업, 문제 및 승인 위임](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [그룹별 승인 프로세스 이해](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [요청 흐름 만들기](/help/manage-work/request-queues/create-a-request-flow.md)
* [전역 및 일회용 승인 프로세스 만들기](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
