---
title: 그룹 및 사용자 설정
description: '[!UICONTROL Workfront DAM]에서 폴더, 그룹 및 사용자를 만드는 방법을 알아봅니다. 사용자 역할 유형을 이해하고 폴더에 권한을 부여합니다.'
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '414'
ht-degree: 100%

---

# 그룹 및 사용자 설정

이 비디오에서는 다음 방법을 배우게 됩니다.

* 그룹 설정이 자산 액세스에 미치는 영향 이해
* 특정 순서로 폴더, 그룹 및 사용자 만들기
* 사용자 역할 유형 이해
* 폴더에 권한 부여
* 그룹 만들기 및 편집
* 사용자 추가 및 편집

>[!VIDEO](https://video.tv.adobe.com/v/3414470/?quality=12&learn=on&enablevpops&captions=kor)

## 그룹 및 사용자 검토

[!UICONTROL Workfront DAM] 시스템을 구성할 때는 전체적으로 사용자 및 그룹이 수행하는 역할을 고려하는 것이 중요합니다.

그룹은 [!UICONTROL Workfront DAM]의 자산 폴더에 대한 액세스를 제어합니다. 그룹 설정은 또한 사용자가 액세스 권한이 있는 자산으로 수행할 수 있는 작업(보기, 다운로드, 편집 등)을 제어합니다.

그룹을 만들 때 [!UICONTROL Workfront DAM]에서 해당 그룹의 멤버가 액세스해야 하는 자산 폴더를 유념해야 합니다.

사용자는 [!UICONTROL Workfront DAM]에 로그인하는 개인 사용자입니다. 사용자는 그룹에 할당되지 않으면 [!UICONTROL Workfront DAM]에 있는 어떤 것에도 액세스할 수 없습니다. 사용자는 필요에 따라 둘 이상의 그룹에 속할 수 있습니다.

## 기본 그룹

[!UICONTROL Workfront DAM]과 함께 제공되는 두 개의 기본 그룹이 있습니다. 모든 사용자는 [!UICONTROL Workfront DAM] 로그인 자격 증명이 있는지 여부에 따라 자동으로 이러한 그룹에 속합니다. 다음 그룹에서 사용자를 추가하거나 제거할 수 없습니다.

* **게스트 그룹**- 익명 사용자의 액세스를 제어하는 데 사용됩니다. 로그인 자격 증명이 없는 사람이거나 현재 로그인하지 않은 사용자일 수 있습니다.
* **로그인** 그룹- 로그인한 모든 사용자는 이 그룹에 속합니다.

기본적으로 관리자 그룹 및 해당 설정도 있습니다. 이 그룹에 사용자를 추가할 수 있지만 설정을 조정할 수는 없습니다.

## 역할 유형

그룹이 만들어지면 역할 유형이 할당됩니다. 역할 유형은 사용자가 로그인할 때 얻을 수 있는 [!UICONTROL Workfront DAM] 시스템의 부분([!UICONTROL Workfront DAM] 자체 또는 [!UICONTROL Brand Connect])을 확인합니다.

[!UICONTROL Workfront DAM] 라이선스에는 다음 세 가지 역할 유형이 있습니다.

* **[!UICONTROL Brand Portal]**- 이 사용자는 승인된 자산을 보고 다운로드할 수 있는 [!UICONTROL Brand Connect]에만 액세스할 수 있습니다.
* **[!UICONTROL 참여자]**- 이 사용자는 [!UICONTROL Workfront DAM] 및 [!UICONTROL Brand Connect]에 액세스할 수 있습니다. 자산 및 폴더에 대한 전체 액세스 권한(보기, 다운로드, 업로드, 편집, 이동 및 삭제)이 있습니다.
* **[!UICONTROL 관리자]**- 시스템 관리자는 [!UICONTROL Brand Connect] 및 [!UICONTROL Workfront DAM]의 모든 항목에 액세스할 수 있으며, 각 항목에 대한 전역 시스템 설정을 구성할 수도 있습니다. 또한 만료되었거나 비활성으로 설정된 자산에 액세스할 수 있습니다.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
