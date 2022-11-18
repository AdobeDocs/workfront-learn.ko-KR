---
title: 재무 액세스 이해
description: 관리자가 재무 액세스 권한을 통해 Workfront에서 추적된 재무 정보를 보고 편집할 수 있는 사용자를 제어하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
kt: 10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 5%

---

# 재무 액세스 이해

조직에서 [!DNL Workfront]를 지정하는 경우, 시스템 관리자는 해당 정보를 보고 편집할 수 있는 액세스 권한이 있는 사용자를 보호하고 관리할 책임이 있습니다.

사용자가 재무 정보를 보거나 편집하려면 다음 두 가지가 필요합니다.

1. 액세스 권한은 [!UICONTROL 액세스 수준].
2. 이러한 액세스 권한을 사용할 수 있는 권한은 객체별로 부여되어야 합니다.

예를 들어, 사용자에게 액세스 수준에서 재무 데이터를 볼 수 있는 권한이 부여될 수 있지만, 사용자와 공유되는 작업에 대한 재무 데이터만 볼 수 있으며 해당 작업의 공유에서는 재무 보기를 사용할 수 있습니다.

따라서 [!UICONTROL 액세스 수준] 해당 객체의 개별 공유 옵션에 따라 일부 객체에서 재무 상태를 조회할 수 있는 재무 정보를 조회할 수 있는 권한 그러나 어떤 사용자도 해당 객체에 부여된 권한이 없으면 어떤 객체에서도 재무 상태를 볼 수 없습니다 [!UICONTROL 액세스 수준].

## [!UICONTROL 액세스 수준] 설정

재무 데이터에 대한 전체 액세스 권한은 [!DNL Workfront] 라이센스 유형.

**[!UICONTROL 계획] 라이선스:**

* 청구 레코드 관리
* 역할 청구 및 비용 요율 관리 및 보기
* 사용자 청구 및 비용 비율 관리 및 보기
* 비용 관리
* 재무 보기 및 편집

**[!UICONTROL 작업] 라이선스:**

* 비용 관리
* 재무 보기

**[!UICONTROL 검토] 라이선스:**

* 재무 보기

**권한은 [!UICONTROL 액세스 수준]. 재무 데이터 액세스에 대한 세 가지 옵션은 다음과 같습니다.**

* [!UICONTROL 액세스 권한 없음] — 사용자가 재무 정보를 볼 수 없습니다.
* [!UICONTROL 보기] — 사용자가 정보를 검토하고 공유할 수 있습니다.
* [!UICONTROL 편집] — 사용자는 정보를 생성, 편집, 삭제 및 공유할 수 있습니다. (계획 라이센스에만 사용 가능)

![액세스 수준의 일반 재무 데이터 옵션을 보여주는 이미지](assets/setting-up-finances-8.png)

중요한 것은 [!UICONTROL 보기] 및 [!UICONTROL 편집] 옵션에는 [!UICONTROL 계획] 라이센스. 에서 톱니바퀴를 클릭합니다 [!UICONTROL 보기] 버튼 을 사용하십시오.

**** 보기

* 역할 청구 및 비용 요금 보기
* 사용자 청구 및 비용 요금 보기

![액세스 수준에서 재무 데이터 보기 옵션을 표시하는 이미지](assets/setting-up-finances-9.png)

**[!UICONTROL 편집]**

이러한 두 옵션은 [!UICONTROL 편집] 선택 사항 및 함께:

* 역할 청구 및 비용 요금 편집
* 사용자 청구 및 비용 요금 편집

![액세스 수준에서 재무 데이터 편집 옵션을 표시하는 이미지](assets/setting-up-finances-10.png)

>[!NOTE]
>
>비용을 추가할 수 있는 사용자는 직접 보고서에서 추가한 비용과 비용을 확인할 수도 있습니다.
