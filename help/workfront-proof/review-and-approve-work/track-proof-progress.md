---
title: 증명 진행 추적
description: 사용 방법 알아보기 [!UICONTROL SOCD] 증명의 진행 상황을 추적할 지표, 증명 진행률 및 보고서 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# 증명 진행 추적

프로젝트 관리자, 증명 관리자 또는 검토 및 승인 프로세스의 다른 이해 담당자는 증명을 추적할 수 있습니다. 이 작업은 [!DNL Workfront’s] 기본 제공 **진행률 표시기** on [!UICONTROL 문서] 페이지 또는 사용자 지정 보고서를 작성하여 페이지를 보거나 페이지를 작성합니다.

에서 증명 진행 상황을 보려면 [!DNL Workfront], 계획, 작업 또는 검토 라이센스가 있고 교정 사용자여야 합니다. 만약 [!DNL Workfront] 프로파일이 이러한 요구 사항을 충족하려면 조직의 교정 시스템 관리자에게 문의하십시오.

## 증명 진행 추적 [!UICONTROL SOCD] 지표 및 증명 상태

를 사용하여 증명의 진행 과정을 개략적으로 파악할 수 있습니다. [!UICONTROL SOCD] 의 아이콘 [!UICONTROL 문서] 목록. 이러한 아이콘은 증명의 특정 작업을 나타냅니다.

![의 이미지 [!UICONTROL 문서] 목록의 [!DNL  Workfront] 프로젝트를 [!UICONTROL SOCD] 강조 표시된 아이콘입니다.](assets/manage-proofs-socd.png)

아이콘은 사용자가 증명을 수신자에게 보낼 때부터 증명의 결정을 내릴 때까지의 증표에 대해 수행된 작업을 나타냅니다.

* **S —** 증명을 수신자에게 보냈습니다.
* **O —** 증거가 개시되었다.
* **C —** 그 증명에 대한 의견이 나왔다.
* **D —** 증명(승인, 거부 등)에 대한 결정이 내려졌습니다.

색상은 작업이 완료되었는지 여부를 나타냅니다.

* **흰색 —** 아직 단계가 발생하지 않았습니다.
* **녹색 —** 단계가 완료되었습니다.
* **주황 —** 증명 기한은 24시간 이내이고 단계가 발생하지 않았습니다.
* **빨간색 —** 증명 마감일이 지났고 단계가 발생하지 않았습니다.

다음 [!UICONTROL SOCD] on [!UICONTROL 문서] 목록, 요약 패널 또는 [!UICONTROL 문서 세부 정보]는 증명의 진행 상황을 개략적으로 요약합니다. [!DNL Workfront] 언어 교정 프로세스에서 &quot;가장 부족&quot;인 수신자를 기반으로 이 항목을 구성합니다.

예를 들어 검토자/승인자가 3명이고 이 중 2명만 증명을 보고 주석을 작성한 경우 [!UICONTROL SOCD] 증명서가 전송되었음을 나타내는 아이콘이 표시됩니다([!UICONTROL S]) 및 열림( )[!UICONTROL O]) 하지만 그런 말은 하지 않았습니다([!UICONTROL C]).

개별 증명 수신자가 수행하는 방법을 알아보려면 교정 워크플로우를 엽니다. 전체 증명 진행 상태가 창 맨 위에 있습니다. 각 스테이지에는 회색 막대에 자체 진행률 표시기가 있습니다.  그리고 각 사용자 옆에는 개인의 진척이 있습니다.

![의 이미지 [!UICONTROL 교정 워크플로] 문서의 섹션.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 증명 상태

증명 상태는 스테이지의 증명 수신자의 상태를 기반으로 합니다. 전체 증명 상태는 [!UICONTROL 문서] 페이지 오른쪽의 [!UICONTROL SOCD] 지표들, 그래서 당신은 당신이 증명에 대한 결정이 있는지 쉽게 알 수 있습니다.

![의 이미지 [!UICONTROL 문서] 목록의 [!DNL  Workfront] 전체 증명 상태가 강조 표시된 프로젝트](assets/manage-proofs-overall-status.png)

이 증명 상태는 증명의 전체 상태를 나타냅니다. 예를 들어 두 명의 수신자가 증명을 승인한 경우 개별 상태가 표시됩니다 [!UICONTROL 승인됨]. 그러나 세 번째 수신자는 아직 결정을 내리지 않았기 때문에 그 사람의 상태는 입니다 [!UICONTROL 보류 중]. 따라서 전체 상태는 [!UICONTROL 보류 중].

조직에 대해 사용자 지정 상태가 구성된 경우 해당 상태가 사용됩니다. 그렇지 않으면 다음과 같은 표준 상태 옵션이 표시됩니다.

* [!UICONTROL 보류 중]
* [!UICONTROL 승인됨]
* [!UICONTROL 변경 사항과 함께 승인됨]
* [!UICONTROL 변경 필요]
* [!UICONTROL 관련 없음]

제품 교정 워크플로우 창을 열어 [!UICONTROL 검토자 및 승인자] 또는 [!UICONTROL 승인자 ]증명 역할.

## 의 보고서 [!DNL Workfront]

활용할 수도 있습니다 [!DNL Workfront’s] 보고 기능을 통해 증명 검토 및 승인 프로세스를 진행할 때 증명을 추적할 수 있습니다.

증명 승인 보고서는 미결 승인을 추적하여 마감일이 충족되는지 확인하는 데 도움이 됩니다.

![의 증명 승인 보고서 이미지 [!DNL  Workfront].](assets/proof-approval-report.png)

문서 버전 보고서를 사용하면 증명 버전을 관리하고 추적할 수 있습니다.

![의 문서 버전 보고서 이미지 [!DNL  Workfront].](assets/document-version-report.png)

을 사용하여 작업하는 것이 좋습니다 [!DNL Workfront] 조직의 요구 사항을 충족하는 보고서를 만들 수 있는 컨설턴트입니다. 일부 보고서에서는 다음과 같은 정보를 필요로 합니다 [!DNL Workfront’s] 텍스트 모드 보고.

## 네 차례야

증명 워크플로우가 원활하게 실행되도록 하기 위해 Workfront에서 사용할 보고 종류를 확인하려면 팀이나 언어 교정 시스템 관리자에게 문의하십시오.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
