---
title: 참여자로서의 자산 관리 이해
description: 워크플로를 향상하기 위해 [!UICONTROL Workfront DAM]에서 자산을 관리하는 방법을 알아보십시오.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 100%

---

# 참여자로서의 자산 관리 이해

이 비디오에서는 다음 방법을 배우게 됩니다.

* 자산에서 편집 메뉴 사용
* 만료 일자 설정
* 알림 보기
* 개별 알림 설정 구성
* 자산 버전 업로드
* 새 폴더 만들기
* 폴더에 메타데이터 템플릿 적용
* 폴더 권한 설정

>[!VIDEO](https://video.tv.adobe.com/v/3414422/?quality=12&learn=on&enablevpops=1&captions=kor)

## 자산 버전 작동 방식

워크플로 일부에는 자산의 여러 버전(또는 라운드, 교정쇄, 반복 등) 관리가 포함될 수 있습니다. [!UICONTROL Workfront DAM]을 통해 모든 버전을 관리할 수 있습니다.

시스템은 기존 파일과 이름이 동일한 파일이 동일한 폴더에 업로드될 때 자동 자산 버전 제어를 허용합니다. 이 기능이 켜져 있는지 확인하려면 시스템 관리자에게 문의하십시오.

자동 버전 제어가 켜져 있는 경우 자산은 원래 자산이 있는 폴더에 로드된 경우에만 버전이 지정됩니다. 두 자산의 파일 이름은 같아야 합니다. 자산이 다른 폴더에 로드되면 자산이 새 파일로 들어갑니다.
버전 제어가 켜져 있지 않으면 어떤 폴더에 넣었는지에 관계없이 기존 파일과 이름이 같은 파일이 새 파일로 업로드됩니다. 이로 인해 같은 폴더에 이름이 같은 두 개의 자산이 있을 수 있습니다.

특정 자산 버전을 수동으로 업로드할 수도 있습니다. 자산에서 편집 아이콘을 클릭한 다음 **[!UICONTROL 새 버전 업로드]**&#x200B;를 선택합니다.

버전이 있는 자산을 Brand Connect에 게시하면 Brand Connect 사용자는 최신 자산 버전만 볼 수 있습니다.

## 폴더 및 자산 상태 및 만료

상태는 [!UICONTROL Workfront DAM]에서 폴더 및 자산에 대한 액세스를 관리할 수 있는 또 다른 방법입니다. 상태를 사용하여 특정 자산 또는 폴더를 [!UICONTROL Brand Connect] 사용자로부터 숨기거나 자산 또는 폴더를 만료하여 시스템 관리자 외에는 액세스할 수 없습니다.

* **[!UICONTROL 활성]** - 자산 및 폴더에 사용됩니다. [!UICONTROL 활성] 상태인 자산 및 폴더는 권한을 가진 모든 사용자에게 표시되며 [!UICONTROL Brand Connect]에 게시될 수 있습니다. [!UICONTROL 활성]은 자산 또는 폴더에 녹색 점으로 표시됩니다.
* **[!UICONTROL 비활성]** - 자산 및 폴더에 사용됩니다. [!UICONTROL 비활성] 상태인 자산 및 폴더는 [!UICONTROL Workfront DAM] 사용자에게는 표시되나 [!UICONTROL Brand Connect]에는 표시되지 않습니다. [!UICONTROL 비활성]은 자산 또는 폴더에 빨간색 점으로 표시됩니다.
* **[!UICONTROL 만료되지 않음]** - 자산에만 사용됩니다. 모든 자산의 기본 상태입니다. [!UICONTROL 활성] 상태인 완료되지 않은 자산은 [!UICONTROL Brand Connect]에 표시됩니다.
* **[!UICONTROL 만료됨]** - 자산에만 사용됩니다. 시스템 관리자를 제외한 사용자는 [!UICONTROL 만료됨] 상태인 자산을 다운로드할 수 없습니다. 시스템 구성에 따라 [!UICONTROL Brand Connect]에 만료된 자산이 표시되거나 표시되지 않습니다.
