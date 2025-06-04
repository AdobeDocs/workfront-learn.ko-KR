---
title: 교정 진행 상황 추적
description: ' [!DNL  Workfront]에서 [!UICONTROL SOCD] 표시기, 교정 진행 상황 및 보고서를 사용하여 교정 진행 상황을 추적하는 방법에 대해 알아봅니다.'
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 8ad86921177da189503211635116146e886dbd17
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 64%

---

# 교정 진행 상황 추적

프로젝트 관리자, 증명 관리자 또는 검토 및 승인 프로세스의 다른 이해 당사자는 증명의 진행 상황을 추적할 수 있습니다. 이 작업은 [!UICONTROL 문서] 페이지에 있는 [!DNL Workfront's]의 기본 제공 **교정 진행률 표시기**&#x200B;를 사용하거나 사용자 정의 보고서를 작성하여 수행할 수 있습니다.

[!DNL Workfront]에서 교정 진행 상황을 보려면 플랜, 작업 또는 검토 라이선스가 있는 교정 사용자여야 합니다. [!DNL Workfront] 프로필이 이러한 요구 사항을 충족하는지 확실하지 않은 경우 조직의 증명 시스템 관리자에게 문의하십시오.

## [!UICONTROL SOCD] 표시기 및 교정쇄 상태를 통해 교정 진행 상황 추적

[!UICONTROL 문서] 목록의 [!UICONTROL SOCD] 아이콘을 사용하여 검토 및 승인 프로세스를 통해 교정이 진행되는 방식을 전체적으로 볼 수 있습니다. 이 아이콘은 교정쇄에 대해 수행된 특정 작업을 나타냅니다.

![[!UICONTROL SOCD] 아이콘이 강조 표시된 [!DNL  Workfront] 프로젝트의 [!UICONTROL 문서] 목록 이미지](assets/manage-proofs-socd.png)

아이콘은 수신자에게 교정쇄를 보내는 시간부터 교정쇄에 대한 결정을 내리는 시간까지 교정쇄에 수행된 작업을 나타냅니다.

* **S -** 수신자에게 교정쇄가 전송되었습니다.
* **O -** 교정쇄가 열렸습니다.
* **C -** 교정쇄에 대한 댓글이 작성되었습니다.
* **D -** 교정쇄에 대한 결정이 내려졌습니다(승인됨, 거부됨 등).

색상은 작업이 완료되었는지 여부를 나타냅니다.

* **흰색 —** 단계가 아직 수행되지 않았습니다.
* **녹색 -** 단계가 완료되었습니다.
* **주황색 —** 증명 기한은 24시간 이내이며 단계가 수행되지 않았습니다.
* **빨강 —** 증명 기한이 지났고 단계가 수행되지 않았습니다.

[!UICONTROL 문서] 목록, 요약 패널 또는 [!UICONTROL 문서 세부 정보]의 [!UICONTROL SOCD]은(는) 증명 진행 상황에 대한 높은 수준의 요약입니다. [!DNL Workfront]은(는) 증명 프로세스에서 &quot;가장 뒤쳐진&quot; 수신자를 기준으로 이 작업을 구성합니다.

예를 들어 세 명의 검토자/승인자 중에 두 명만이 교정쇄를 보고 댓글을 단 경우, [!UICONTROL SOCD] 아이콘에는 교정쇄가 전송되고([!UICONTROL S]) 열렸으나([!UICONTROL O]) 댓글([!UICONTROL C])이 달리지 않은 것으로 표시됩니다.

**증명에 대한 최종 결정**(예: 승인됨 또는 거부됨)이 내려지면 해당 단계에서 개별 작업(예: 증명 열기 또는 댓글 달기)이 수행되지 않았더라도 사용자에게 모든 SOCD 표시기가 녹색으로 표시될 수 있습니다. 이는 개별 참여가 아닌 전체 단계 완료를 반영하도록 설계된 시스템 전체 동작입니다.

**결정이 등록되기 전에** 각 SOCD 표시기는 실제 사용자 활동을 반영합니다(예: 작업이 수행되지 않은 경우 흰색, 작업이 완료된 경우 녹색). 결정 후 시스템은 워크플로 완료를 가정하고 모든 지표를 그에 따라 업데이트합니다.

각 개별 교정쇄 수신자의 진행 상황을 알고 싶다면 교정 워크플로를 엽니다. 전체 교정 진행률은 창 상단에 있습니다. 각 단계의 회색 막대에는 자체 진행률 표시기가 있습니다.  그리고 각 사용자 옆에는 개개인의 진보가 있다.

![문서의 [!UICONTROL 교정 워크플로] 섹션 이미지](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 교정쇄 상태

증명 상태는 단계의 증명 수신자의 상태를 기반으로 합니다. 전체적인 교정쇄 상태는 [!UICONTROL SOCD] 표시기의 오른쪽에 있는 [!UICONTROL 문서] 페이지에서 볼 수 있으므로 교정쇄에 대한 결정이 있는지 쉽게 알 수 있습니다.

![전체 교정쇄 상태가 강조 표시된 [!DNL  Workfront] 프로젝트의 [!UICONTROL 문서] 목록 이미지](assets/manage-proofs-overall-status.png)

이 교정쇄 상태는 교정쇄의 전체 상태를 나타냅니다. 예를 들어 두 명의 수신자가 교정쇄를 승인한 경우, 개별 상태는 [!UICONTROL 승인됨]으로 표시됩니다. 그러나 세 번째 받는 사람이 아직 결정을 내리지 않았으므로 해당 사용자의 상태는 [!UICONTROL 보류 중]입니다. 따라서 전체 상태는 [!UICONTROL 보류 중]으로 표시됩니다.

조직에 대해 사용자 정의 상태가 구성된 경우 해당 상태가 사용됩니다. 그렇지 않으면 다음의 표준 상태 옵션이 표시됩니다.

* [!UICONTROL 보류 중]
* [!UICONTROL 승인됨]
* [!UICONTROL 변경 사항과 함께 승인됨]
* [!UICONTROL 변경 필요]
* [!UICONTROL 관련 없음]

교정 워크플로 창을 열어 [!UICONTROL 검토자 및 승인자] 또는 [!UICONTROL 승인자] 교정 역할이 할당된 수신자의 교정쇄 상태를 확인합니다.

## [!DNL Workfront] 보고서

또한 [!DNL Workfront's]의 보고 기능을 활용하여 검토 및 승인 프로세스를 진행하면서 교정쇄를 추적할 수 있습니다.

교정쇄 승인 보고서를 사용하면 처리되지 않은 승인을 추적하여 기한을 준수할 수 있습니다.

![[!DNL  Workfront]의 교정쇄 승인 보고서 이미지](assets/proof-approval-report.png)

문서 버전 보고서를 사용하면 교정쇄 버전을 관리하고 추적할 수 있습니다.

![[!DNL  Workfront]의 문서 버전 보고서 이미지](assets/document-version-report.png)

[!DNL Workfront] 컨설턴트와 협력하여 조직의 요구 사항에 맞는 보고서를 작성하는 것이 좋습니다. 일부 보고서는 [!DNL Workfront's] 텍스트 모드 보고에 대해 숙지해야 합니다.

## 사용자 차례

증명 워크플로가 원활하게 실행되도록 하기 위해 Workfront에서 사용할 보고 종류를 알아보려면 팀 또는 증명 시스템 관리자에게 문의하십시오.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
