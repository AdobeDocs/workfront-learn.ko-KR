---
title: 의 그룹 및 사용자 이해 [!UICONTROL Workfront DAM]
description: 에서 폴더, 그룹 및 사용자를 만드는 방법을 알아봅니다. [!UICONTROL Workfront DAM]. 사용자 역할 유형을 파악하고 폴더에 권한을 부여합니다.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 시스템 설정: 그룹 및 사용자

이 비디오에서는 다음 방법을 배웁니다.

* 그룹 설정이 자산 액세스에 미치는 영향을 이해합니다
* 특정 순서로 폴더, 그룹 및 사용자 만들기
* 사용자 역할 유형 이해
* 폴더에 권한 부여
* 그룹 만들기 및 편집
* 사용자 추가 및 편집

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12)

## 그룹 및 사용자 검토

를 구성할 때 [!UICONTROL Workfront DAM] 시스템, 사용자와 그룹이 큰 그림에서 수행하는 역할을 고려하는 것이 중요합니다.

그룹 제어 [!UICONTROL Workfront DAM]. 그룹 설정은 사용자가 자산으로 수행할 수 있는 작업(보기, 다운로드, 편집 등)을 제어합니다. 그들은 액세스할 권한이 있다.

그룹을 생성할 때 해당 그룹의 구성원이 액세스해야 하는 자산 폴더를 고려해야 합니다 [!UICONTROL Workfront DAM].

사용자는 [!UICONTROL Workfront DAM]. 사용자는 의 어떤 항목에도 액세스할 수 없습니다 [!UICONTROL Workfront DAM] 그룹에 할당되지 않은 경우 사용자는 필요에 따라 두 개 이상의 그룹에 속할 수 있습니다.

## 기본 그룹

다음과 같은 두 개의 기본 그룹이 있습니다 [!UICONTROL Workfront DAM]. 모든 사용자는 그룹 소유여부에 따라 자동으로 이러한 그룹에 속합니다 [!UICONTROL Workfront DAM] 로그인 자격 증명. 다음 그룹에서 사용자를 추가하거나 제거할 수 없습니다.

* **게스트 그룹**- 익명 사용자에 대한 액세스를 제어하는 데 사용됩니다. 로그인 자격 증명이 없거나 현재 로그인하지 않은 사용자일 수 있습니다.
* **기록됨**-In 그룹 - 로그인한 모든 사용자가 이 그룹에 속합니다.

관리자 그룹 및 해당 설정도 기본적으로 존재합니다. 사용자를 이 그룹에 추가할 수는 있지만 설정을 조정할 수는 없습니다.

## 역할 유형

그룹이 만들어지면 역할 유형이 할당됩니다. 역할 유형은 [!UICONTROL Workfront DAM] 시스템 사용자는 로그인하면 받게 됩니다 — [!UICONTROL Workfront DAM] 또는 [!UICONTROL Brand Connect].

에는 세 가지 역할 유형이 있습니다 [!UICONTROL Workfront DAM] 라이센스:

* **[!UICONTROL Brand Portal]**—이러한 사용자는에 대해서만 액세스 권한이 있습니다. [!UICONTROL Brand Connect]: 승인된 자산을 보고 다운로드할 수 있는 위치입니다.
* **[!UICONTROL 기여자]**—이러한 사용자가 [!UICONTROL Workfront DAM] 및 [!UICONTROL Brand Connect]. 자산 및 폴더에 대한 보기, 다운로드, 업로드, 편집, 이동 및 삭제 등의 전체 액세스 권한이 있습니다.
* **[!UICONTROL 관리자]**—시스템 관리자는 [!UICONTROL Brand Connect] 및 [!UICONTROL Workfront DAM]뿐만 아니라, 각 사용자에 대한 글로벌 시스템 설정을 지정하는 기능도 추가되었습니다. 또한 만료되었거나 비활성 상태로 설정된 자산에 액세스할 수도 있습니다.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
