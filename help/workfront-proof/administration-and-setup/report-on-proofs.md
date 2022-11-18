---
title: 증명 보고
description: 보고 기능을 사용하여 증명 진행 상황을 관리하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
kt: 10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 증명 보고

[!DNL Workfront]의 디지털 교정 기능을 사용하면 프로젝트 및 관련 검토 워크플로우를 한 곳에서 관리할 수 있습니다. [!DNL Workfront]. 검토 및 승인 정보를 표시하는 보고서 유형, 필드 소스 및 필드 이름으로 이루어지는 교정 작업에 대한 중요한 통찰력을 얻을 수 있습니다.

을 사용하여 작업하는 것이 좋습니다 [!DNL Workfront] 조직의 요구 사항을 충족하는 보고서를 만들 수 있는 컨설턴트입니다. 일부 보고서에서는 다음과 같은 정보를 필요로 합니다 [!DNL Workfront]의 텍스트 모드 보고.

에서 검토 및 승인 프로세스를 통해 팀이 증명을 관리할 수 있도록 지원하는 이러한 기본적인 표준 보고서로 시작하십시오. [!DNL Workfront].

## [!UICONTROL 증명 승인]

이 보고서 유형을 사용하면 미처리 증명 승인을 추적하여 마감일이 충족되는지 확인할 수 있습니다.

![선택 [!UICONTROL 증명 승인] 에서 [!UICONTROL 새 보고서] 드롭다운 메뉴](assets/proof-system-setups-proof-approval-report.png)

보기 및 필터 옵션은 다음과 같습니다 [!UICONTROL 결정 날짜], [!UICONTROL 증명 승인], [!UICONTROL 승인자 단계], [!UICONTROL 워크플로우 템플릿], 및 [!UICONTROL 요청자 정보]. 텍스트 모드 보고를 사용하면 문서 이름별로 목록을 구성하는 그룹을 만들 수 있습니다.

증명 승인 보고서를 작성할 때 가장 최신 버전의 증명과 관련된 정보가 있는지 확인하십시오. [!DNL Workfront] 필터에 이 필드 소스 및 필드 이름을 포함하는 것이 좋습니다.

**[!UICONTROL 증명 승인]>>[!UICONTROL 현재 문서 버전입니다.]**

![Report Builder의 필터 탭](assets/proof-system-setups-proof-approval-report-is-current-version.png)

이 기능은 여러 버전이 있는 증명을 보고하여 보고서에 승인이 필요한 각 증명의 현재 버전만 나열하도록 할 때 유용합니다. 더 이상 작업할 필요가 없는 이전 버전을 필터링합니다.

## [!UICONTROL 문서 버전]

이 보고서 유형에서는 의 버전을 관리하고 추적할 수 있습니다 [!DNL Workfront].

![선택 [!UICONTROL 문서 버전] 에서 [!UICONTROL 새 보고서] 드롭다운 메뉴](assets/proof-system-setups-document-version-report.png)

보기 옵션에는 [!UICONTROL 문서 버전], [!UICONTROL 문서], [!UICONTROL 입력], [!UICONTROL 증명 승인 상태], [!UICONTROL 증명 작성자], 및 [!UICONTROL 문서 공급자].

그룹화는 다음 방법으로 수행할 수 있습니다 [!UICONTROL 문서 버전], [!UICONTROL 입력], [!UICONTROL 증명 승인 상태], 또는 증명 소유자 정보.

필터에는 다음이 포함됩니다 [!UICONTROL 문서 버전], [!UICONTROL 액세스 수준], [!UICONTROL 문서], [!UICONTROL 입력], [!UICONTROL 증명 승인 상태], [!UICONTROL 증명 작성자], 및 문서 공급자 정보.

뷰에 이 열이 있는 보고서에서 각 문서에 대해 현재 활성화된 언어 교정 단계의 이름을 표시할 수 있습니다.

**[!UICONTROL 문서 버전] >> [!UICONTROL 활성 증명 단계]**

![Report Builder의 필터 탭](assets/proof-system-setups-active-proof-stages.png)

현재 활성 상태인 스테이지가 없으면 열이 비어 있습니다.

이 필드 소스 >> 필드 이름은 보고서에서 필터로도 사용할 수 있습니다.

를 사용하십시오 [!UICONTROL 증명 작성자] 증명을 만든 사용자에 대한 정보를 보고하는 필드 소스입니다. 을(를) 선택합니다 [!UICONTROL 이름] 증명 작성자의 이름을 뷰에 표시하는 필드 소스입니다.

**[!UICONTROL 증명 작성자] >> [!UICONTROL 이름]**

이 필드 소스 > 필드 이름 콤보 상자도 필터로 사용할 수 있습니다.

![Report Builder의 필터 탭](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
