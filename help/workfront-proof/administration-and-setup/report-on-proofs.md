---
title: 증명에 대한 보고서
description: 보고 기능을 사용하여 증명 진행률을 관리하는 방법에 대해 알아봅니다.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
kt: 10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# 증명에 대한 보고서

[!DNL Workfront]의 디지털 교정 기능을 사용하면 프로젝트 및 관련 검토 워크플로를 한 곳에서 모두 관리할 수 있습니다. [!DNL Workfront]. 검토 및 승인 정보를 표시하는 보고서 유형, 필드 소스 및 필드 이름으로 수행되는 증명 작업에 대한 중요한 통찰력을 얻으십시오.

을(를) 사용하여 작업하는 것이 좋습니다 [!DNL Workfront] 컨설턴트가 조직의 요구 사항에 맞는 보고서를 만듭니다. 일부 보고서는 다음에 대한 익숙함이 필요합니다. [!DNL Workfront]의 텍스트 모드 보고.

다음의 기본 표준 보고서로 시작하여에서 검토 및 승인 프로세스를 거친 증명을 팀이 관리할 수 있습니다. [!DNL Workfront].

## [!UICONTROL 증명 승인]

이 보고서 유형은 기한이 충족되는지 확인하기 위해 미해결 증명 승인을 추적하는 데 도움이 됩니다.

![선택 [!UICONTROL 증명 승인] 다음에서 [!UICONTROL 새 보고서] 드롭다운 메뉴](assets/proof-system-setups-proof-approval-report.png)

보기 및 필터 옵션은 다음과 같습니다 [!UICONTROL 결정 일자], [!UICONTROL 증명 승인], [!UICONTROL 승인자 단계], [!UICONTROL 워크플로 템플릿], 및 [!UICONTROL 요청자 정보]. 텍스트 모드 보고를 사용하면 문서 이름별로 목록을 구성하는 그룹화를 만들 수 있습니다. 다음을 참조하십시오 [그룹화를 위한 기본 텍스트 모드 이해](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=en).

증명 승인 보고서를 작성할 때 가장 최신 버전의 증명과 관련된 정보가 있는지 확인하십시오. [!DNL Workfront] 는 이 필드 소스와 필드 이름을 필터에 포함할 것을 권장합니다.

**[!UICONTROL 증명 승인]>>[!UICONTROL 현재 문서 버전임]**

![Report Builder의 필터 탭](assets/proof-system-setups-proof-approval-report-is-current-version.png)

이 기능은 여러 버전이 있는 증명에 대해 보고할 때 유용하며, 따라서 보고서에는 승인이 필요한 각 증명의 현재 버전만 나열됩니다. 이렇게 하면 더 이상 작업할 필요가 없는 이전 버전이 필터링됩니다.

## [!UICONTROL 문서 버전]

이 보고서 유형을 사용하여에서 버전을 관리하고 추적할 수 있습니다. [!DNL Workfront].

![선택 [!UICONTROL 문서 버전] 다음에서 [!UICONTROL 새 보고서] 드롭다운 메뉴](assets/proof-system-setups-document-version-report.png)

보기 옵션에는 다음 항목의 정보가 포함됩니다. [!UICONTROL 문서 버전], [!UICONTROL 문서], [!UICONTROL 입력한 사람:], [!UICONTROL 증명 승인 상태], [!UICONTROL 증명 작성자], 및 [!UICONTROL 문서 공급자].

그룹화는 다음 방법으로 수행할 수 있습니다. [!UICONTROL 문서 버전], [!UICONTROL 입력한 사람:], [!UICONTROL 증명 승인 상태], 또는 증명 소유자 정보.

필터에는 다음이 포함됩니다 [!UICONTROL 문서 버전], [!UICONTROL 액세스 수준], [!UICONTROL 문서], [!UICONTROL 입력한 사람:], [!UICONTROL 증명 승인 상태], [!UICONTROL 증명 작성자]및 문서 공급자 정보입니다.

보기의 이 열을 사용하여 보고서의 각 문서에 대해 현재 활성화된 증명 단계의 이름을 표시할 수 있습니다.

**[!UICONTROL 문서 버전] >> [!UICONTROL 활성 증명 단계]**

![Report Builder의 필터 탭](assets/proof-system-setups-active-proof-stages.png)

현재 활성화된 스테이지가 없으면 열이 비어 있습니다.

이 필드 소스 >> 필드 이름은 보고서의 필터로도 사용할 수 있습니다.

사용 [!UICONTROL 증명 생성자] 증명을 만든 사용자에 대한 정보를 보고할 필드 소스입니다. 다음을 선택합니다. [!UICONTROL 이름] 보기에 증명 작성자의 이름을 표시할 필드 소스입니다.

**[!UICONTROL 증명 생성자] >> [!UICONTROL 이름]**

이 필드 소스 >> 필드 이름 콤보 또한 필터로 사용할 수 있습니다.

![Report Builder의 필터 탭](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
