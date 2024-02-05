---
title: 증명 진행 상황 추적
description: ' [!DNL  Workfront]에서 [!UICONTROL SOCD] 표시기, 증명 진행 상황 및 보고서를 사용하여 증명 진행 상황을 추적하는 방법에 대해 알아봅니다.'
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
workflow-type: ht
source-wordcount: '674'
ht-degree: 100%

---

# 증명 진행 상황 추적

프로젝트 관리자, 증명 관리자 또는 검토 및 승인 프로세스의 기타 관련자로서 증명 진행 상황을 추적하고자 합니다. 이 작업은 [!UICONTROL 문서] 페이지에 있는 [!DNL Workfront’s]의 기본 제공 **증명 진행률 표시기**&#x200B;를 사용하거나 사용자 정의 보고서를 작성하여 수행할 수 있습니다.

[!DNL Workfront]에서 증명 진행 상황을 보려면 플랜, 작업 또는 검토 라이선스가 있는 증명 사용자여야 합니다. 사용자의 [!DNL Workfront] 프로필이 이러한 요구 사항을 충족하는지 여부는 조직의 증명 시스템 관리자에게 확인하십시오.

## [!UICONTROL SOCD] 표시기 및 증명 상태를 통해 증명 진행 상황 추적

[!UICONTROL 문서] 목록의 [!UICONTROL SOCD] 아이콘을 사용하여 검토 및 승인 프로세스를 통해 증명이 진행되는 방식을 전체적으로 볼 수 있습니다. 이 아이콘은 증명에 대해 수행된 특정 작업을 나타냅니다.

![[!UICONTROL SOCD] 아이콘이 강조 표시된 [!DNL  Workfront] 프로젝트의 [!UICONTROL 문서] 목록 이미지](assets/manage-proofs-socd.png)

아이콘은 수신자에게 증명을 보내는 시간부터 증명에 대한 결정을 내리는 시간까지 증명에 수행된 작업을 나타냅니다.

* **S -** 수신자에게 증명이 전송되었습니다.
* **O -** 증명이 열렸습니다.
* **C -** 증명에 대한 댓글이 작성되었습니다.
* **D -** 증명에 대한 결정이 내려졌습니다(승인됨, 거부됨 등).

색상은 작업이 완료되었는지 여부를 나타냅니다.

* **흰색 -** 아직 단계가 이루어지지 않았습니다.
* **녹색 -** 단계가 완료되었습니다.
* **주황색 -** 증명 기한은 24시간 이내이며 단계가 이루어지지 않았습니다.
* **빨간색 -** 증명 기한이 지났고 단계가 이루어지지 않았습니다.

요약 패널 또는 [!UICONTROL 문서 세부 정보]에 있는 [!UICONTROL 문서] 목록의 [!UICONTROL SOCD]는 증명 진행 상황에 대한 높은 수준의 개요입니다. [!DNL Workfront]는 증명 프로세스에서 “가장 뒤쳐진” 수신자를 기반으로 이를 구성합니다.

예를 들어 세 명의 검토자/승인자 중에 두 명만이 증명을 보고 댓글을 단 경우, [!UICONTROL SOCD] 아이콘에는 증명이 전송되고([!UICONTROL S]) 열렸으나([!UICONTROL O]) 댓글([!UICONTROL C])이 달리지 않은 것으로 표시됩니다.

각 개별 증명 수신자의 진행 상황을 알고 싶다면 증명 워크플로를 엽니다. 전체 증명 진행률은 창 상단에 있습니다. 각 단계의 회색 막대에는 자체 진행률 표시기가 있습니다.  그리고 각 사용자 옆에는 개인의 진행 상황이 있습니다.

![문서의 [!UICONTROL 증명 워크플로] 섹션 이미지](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 증명 상태

증명 상태는 단계의 증명 수신자 상태를 기반으로 합니다. 전체적인 증명 상태는 [!UICONTROL SOCD] 표시기의 오른쪽에 있는 [!UICONTROL 문서] 페이지에서 볼 수 있으므로 증명에 대한 결정이 있는지 쉽게 알 수 있습니다.

![전체 증명 상태가 강조 표시된 [!DNL  Workfront] 프로젝트의 [!UICONTROL 문서] 목록 이미지](assets/manage-proofs-overall-status.png)

이 증명 상태는 증명의 전체 상태를 나타냅니다. 예를 들어 두 명의 수신자가 증명을 승인한 경우, 개별 상태는 [!UICONTROL 승인됨]으로 표시됩니다. 그러나 세 번째 수신자가 아직 결정을 내리지 않았기 때문에 해당 사용자의 상태는 [!UICONTROL 보류 중]입니다. 따라서 전체 상태는 [!UICONTROL 보류 중]으로 표시됩니다.

조직에 대해 사용자 정의 상태가 구성된 경우 해당 상태가 사용됩니다. 그렇지 않으면 다음과 같은 표준 상태 옵션이 표시됩니다.

* [!UICONTROL 보류 중]
* [!UICONTROL 승인됨]
* [!UICONTROL 변경 사항과 함께 승인됨]
* [!UICONTROL 변경 필요]
* [!UICONTROL 관련 없음]

증명 워크플로 창을 열어 [!UICONTROL 검토자 및 승인자] 또는 [!UICONTROL 승인자] 증명 역할이 할당된 수신자의 증명 상태를 확인합니다.

## [!DNL Workfront] 보고서

또한 [!DNL Workfront’s]의 보고 기능을 활용하여 검토 및 승인 프로세스를 진행하면서 증명을 추적할 수 있습니다.

증명 승인 보고서를 사용하면 처리되지 않은 승인을 추적하여 기한을 준수할 수 있습니다.

![[!DNL  Workfront]의 증명 승인 보고서 이미지](assets/proof-approval-report.png)

문서 버전 보고서를 사용하면 증명 버전을 관리하고 추적할 수 있습니다.

![[!DNL  Workfront]의 문서 버전 보고서 이미지](assets/document-version-report.png)

[!DNL Workfront] 컨설턴트와 협력하여 조직의 요구 사항에 맞는 보고서를 작성하는 것이 좋습니다. 일부 보고서는 [!DNL Workfront’s] 텍스트 모드 보고에 대해 숙지해야 합니다.

## 사용자 차례

팀 또는 증명 시스템 관리자와 대화하여 증명 워크플로를 원활하게 실행하도록 Workfront에서 사용할 보고 유형을 알아봅니다.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
