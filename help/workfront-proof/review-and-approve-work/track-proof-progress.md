---
title: 증명 진행 추적
description: 사용 방법 알아보기 [!UICONTROL SOCD] 의 증명 진행 상황을 추적하기 위한 지표, 증명 진행 상황 및 보고서 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# 증명 진행 추적

프로젝트 관리자, 증명 관리자 또는 검토 및 승인 프로세스의 다른 이해 당사자는 증명의 진행 상황을 추적할 수 있습니다. 다음을 사용하여 이 작업 수행 [!DNL Workfront’s] 기본 **증명 진행 표시기** 다음에 있음 [!UICONTROL 문서] 페이지를 만들거나 사용자 지정 보고서를 작성하십시오.

증명 진행 상황을 보려면 [!DNL Workfront], 플랜, 작업 또는 검토 라이선스가 있어야 하며 증명 사용자여야 합니다. 다음을 확인할 수 없는 경우 [!DNL Workfront] 프로필이 이러한 요구 사항을 충족하면 조직의 증명 시스템 관리자에게 문의하십시오.

## 증명 진행 상황 추적 [!UICONTROL SOCD] 지표 및 증명 상태

을(를) 사용하여 검토 및 승인 프로세스를 통해 증명이 어떻게 진행되는지 높은 수준으로 봅니다. [!UICONTROL SOCD] 의 아이콘 [!UICONTROL 문서] 목록을 표시합니다. 이 아이콘은 증명에서 수행한 특정 작업을 나타냅니다.

![의 이미지 [!UICONTROL 문서] 의 목록 [!DNL  Workfront] 이 포함된 프로젝트 [!UICONTROL SOCD] 강조 표시된 아이콘.](assets/manage-proofs-socd.png)

아이콘은 수신자에게 증명을 보낸 시점부터 증명에 대한 결정을 내리는 시점까지 증명에 대한 작업을 나타냅니다.

* **S —** 증명이 수신자에게 전송되었습니다.
* **O —** 증명이 열렸습니다.
* **C —** 증명에 대한 댓글이 작성되었습니다.
* **D —** 증명(승인, 거부 등)에 대한 결정이 내려졌습니다.

색상은 작업이 완료되었는지 여부를 나타냅니다.

* **흰색 —** 단계가 아직 발생하지 않았습니다.
* **녹색 —** 단계가 완료되었습니다.
* **주황 —** 증명 기한은 24시간 이내이며 단계가 발생하지 않았습니다.
* **빨강 —** 증명 기한이 지났고 단계가 발생하지 않았습니다.

다음 [!UICONTROL SOCD] 다음에 있음 [!UICONTROL 문서] 목록, 요약 패널 또는 [!UICONTROL 문서 세부 정보]는 증명 진행 상황에 대한 높은 수준의 요약입니다. [!DNL Workfront] 는 증명 프로세스에서 &quot;가장 뒤쳐진&quot; 수신자를 기준으로 이 작업을 구성합니다.

예를 들어 검토자/승인자가 3명이고 이 중 2명만 증명을 보고 댓글을 단 경우 [!UICONTROL SOCD] 아이콘은 증명이 전송되었음을 나타냅니다([!UICONTROL S]) 및 열림([!UICONTROL O]) 그러나 해당 의견은 허용되지 않습니다([!UICONTROL C]).

각 개별 증명 수신자의 활동 방식을 확인하려면 증명 워크플로를 여십시오. 전반적인 증명 진행률이 창 맨 위에 있습니다. 각 단계에는 회색 막대에 자체 진행률 표시기가 있습니다.  그리고 각 사용자 옆에는 개인의 진행률이 있습니다.

![의 이미지 [!UICONTROL 증명 워크플로] 문서의 섹션입니다.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 증명 상태

증명 상태는 단계의 증명 수신자의 상태를 기반으로 합니다. 전체 증명 상태가 다음에 표시됨 [!UICONTROL 문서] 페이지, 오른쪽 [!UICONTROL SOCD] 지표를 통해 증명에 대한 결정이 있는지 쉽게 알 수 있습니다.

![의 이미지 [!UICONTROL 문서] 의 목록 [!DNL  Workfront] 프로젝트(전체 증명 상태 강조 표시)](assets/manage-proofs-overall-status.png)

이 증명 상태는 증명의 전체 상태를 나타냅니다. 예를 들어 두 수신자가 증명을 승인한 경우 개별 상태가 표시됩니다 [!UICONTROL 승인됨]. 그러나 세 번째 수신자는 아직 결정을 하지 않았기 때문에 해당 사용자의 상태는 입니다. [!UICONTROL 보류 중]. 따라서 전체 상태는 다음과 같이 표시됩니다. [!UICONTROL 보류 중].

조직에 대해 사용자 정의 상태가 구성된 경우 해당 상태가 사용됩니다. 그렇지 않으면 다음의 표준 상태 옵션이 표시됩니다.

* [!UICONTROL 보류 중]
* [!UICONTROL 승인됨]
* [!UICONTROL 변경 사항과 함께 승인됨]
* [!UICONTROL 변경 필요]
* [!UICONTROL 관련 없음]

증명 워크플로 창을 열어 지정된 수신자에 대한 증명 상태를 확인합니다. [!UICONTROL 검토자 및 승인자] 또는 [!UICONTROL 승인자]증명 역할.

## 의 보고서 [!DNL Workfront]

다음을 활용할 수도 있습니다 [!DNL Workfront’s] 검토 및 승인 프로세스를 진행할 때 증명을 추적할 보고 기능.

증명 승인 보고서는 기한이 충족되었는지 확인하기 위해 미해결 승인을 추적하는 데 도움이 됩니다.

![의 증명 승인 보고서 이미지 [!DNL  Workfront].](assets/proof-approval-report.png)

문서 버전 보고서를 통해 증명 버전을 관리하고 추적할 수 있습니다.

![의 문서 버전 보고서 이미지 [!DNL  Workfront].](assets/document-version-report.png)

을(를) 사용하여 작업하는 것이 좋습니다 [!DNL Workfront] 컨설턴트가 조직의 요구 사항에 맞는 보고서를 만듭니다. 일부 보고서는 다음에 대한 익숙함이 필요합니다. [!DNL Workfront’s] 텍스트 모드 보고.

## 당신 차례입니다

증명 워크플로가 원활하게 실행되도록 하기 위해 Workfront에서 사용할 보고 종류를 알아보려면 팀 또는 증명 시스템 관리자에게 문의하십시오.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
