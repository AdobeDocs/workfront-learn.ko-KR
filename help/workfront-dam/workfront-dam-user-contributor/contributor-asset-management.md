---
title: 에서 자산을 관리하는 방법 [!UICONTROL Workfront DAM]
description: 에서 자산을 관리하는 방법을 알아봅니다 [!UICONTROL Workfront DAM] 워크플로우 개선.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 기여자: 자산 관리

이 비디오에서는 다음 방법을 배웁니다.

* 자산에서 편집 메뉴 사용
* 만료 날짜 설정
* 알림 보기
* 개별 알림 설정 설정
* 자산 버전 업로드
* 새 폴더 만들기
* 폴더에 메타데이터 템플릿 적용
* 폴더 권한 설정

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## 자산 버전 작동 방식

워크플로우의 일부에는 자산의 여러 버전(또는 라운드, 증명, 반복 등 호출되는 모든 버전)을 관리하는 작업이 포함될 수 있습니다. 모든 버전을 [!UICONTROL Workfront DAM].

기존 파일과 동일한 이름의 파일을 동일한 폴더에 업로드할 때 자동 자산 버전 제어가 가능합니다. 이 기능이 설정되어 있는지 확인하려면 시스템 관리자에게 문의하십시오.

자동 버전 제어가 켜진 경우, 자산은 원래 자산이 들어 있는 폴더에 로드되는 경우에만 버전 전환이 됩니다. 두 자산 모두 파일 이름이 같아야 합니다. 자산이 다른 폴더에 로드되면 자산이 새 파일로 이동합니다.
버전 컨트롤이 켜져 있지 않으면 파일이 저장되는 폴더에 관계없이 기존 파일과 동일한 이름을 가진 파일이 새 파일과 업로드됩니다. 이로 인해 동일한 폴더에 이름이 같은 두 개의 자산이 있을 수 있습니다.

특정 자산의 버전을 수동으로 업로드할 수도 있습니다. 자산에서 편집 아이콘을 클릭한 다음, 을 선택합니다 **[!UICONTROL 새 버전 업로드]**.

버전이 있는 자산을 Brand Connect에 게시하면 Brand Connect 사용자는 최신 버전의 자산만 표시됩니다.

## 폴더 및 자산 상태 및 만료

상태는 의 폴더 및 자산에 대한 액세스를 관리하는 다른 방법입니다 [!UICONTROL Workfront DAM]. 상태를 사용하여 특정 자산이나 폴더를 [!UICONTROL Brand Connect] 사용자 또는 시스템 관리자가 아닌 사용자가 액세스할 수 있도록 자산 또는 폴더를 만료합니다.

* **[!UICONTROL 활성]**- 자산 및 폴더에 사용됩니다. 를 사용하는 자산 및 폴더 [!UICONTROL 활성] 상태는 권한이 있는 모든 사용자가 볼 수 있으며 [!UICONTROL Brand Connect]. [!UICONTROL 활성] 는 자산이나 폴더에 녹색 점으로 표시됩니다.
* **[!UICONTROL 비활성]**- 자산 및 폴더에 사용됩니다. 를 사용하는 자산 및 폴더 [!UICONTROL 비활성] 상태가 [!UICONTROL Workfront DAM] 사용자이지만 [!UICONTROL Brand Connect]. [!UICONTROL 비활성] 는 자산이나 폴더에 빨간색 점으로 표시됩니다.
* **[!UICONTROL 만료되지 않음]**- 자산에만 사용됩니다. 모든 자산의 기본 상태입니다. 또한 만료되지 않은 자산 [!UICONTROL 활성] 에 표시됩니다. [!UICONTROL Brand Connect].
* **[!UICONTROL 만료됨]**- 자산에만 사용됩니다. 가 있는 자산 [!UICONTROL 만료됨] 시스템 관리자를 제외한 사용자는 상태를 다운로드할 수 없습니다. 만료된 자산이 [!UICONTROL Brand Connect], 시스템 구성에 따라 다릅니다.
