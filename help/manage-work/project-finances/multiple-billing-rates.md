---
title: 여러 청구 요금 이해
description: 프로젝트 내에서 시스템 청구 요금을 재정의하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 여러 청구 요금 이해

다음 범위 내 [!DNL Workfront], 프로젝트 관리자는 특정 프로젝트 내에서 시스템 청구 요율을 오버라이드할 수 있습니다. 이전에는 프로젝트에 새 청구 요금이 적용되면 향후 시간뿐만 아니라 프로젝트에 이미 기록된 시간에도 영향을 주었습니다.

포함 [!DNL Workfront]의 새로운 다중 청구 요금 기능을 사용하면 프로젝트 관리자가 청구 요금을 적용할 기간을 결정할 수 있습니다. 이렇게 하면 비율이 협상되거나 변경된 경우 프로젝트 관리자가 해당 비율이 언제 적용되어야 하는지 결정할 수 있습니다.

## 청구 요금 변경

1. 프로젝트의 랜딩 페이지로 이동합니다. 선택 **[!UICONTROL 청구 요금]** 왼쪽 패널에서 가져옵니다.

   ![선택하는 이미지 [!UICONTROL 청구 요금] 위치: [!DNL Workfront]](assets/project-finances-1.png)

1. 다음에서 **[!UICONTROL 청구 요금]** 탭을 클릭하고 **[!UICONTROL 청구 요금 추가]** 단추를 클릭합니다. 선택 **[!UICONTROL 새 청구 요금]** 드롭다운에서 을 클릭합니다.

   ![선택하는 이미지 [!UICONTROL 새 청구 요금] 위치: [!DNL Workfront]](assets/project-finances-2.png)

1. 다음 [!UICONTROL 새 청구 요금] 대화 상자가 나타납니다. 다음에서 **[!UICONTROL 작업 역할]** 드롭다운에서 새 청구 요금이 적용될 작업 역할을 선택합니다.

   ![의 새 청구 요금에 대한 작업 역할 선택 이미지 [!DNL Workfront]](assets/project-finances-3.png)

1. 작업 역할을 선택하면 [!UICONTROL 기본 청구 요금] 및 [!UICONTROL 청구 요금 1] 필드가 나타납니다. 새 청구 요율을 입력합니다. [!UICONTROL 청구 요금 1] 필드. 청구 요금이 전체 프로젝트(과거, 현재 및 미래 기록된 시간)에 적용되는 경우 **[!UICONTROL 저장]** 단추를 클릭합니다.

   ![의 전체 프로젝트에 적용되는 새 청구 요금을 저장하는 이미지입니다. [!DNL Workfront]](assets/project-finances-5.png)

1. 새 청구 요금이 특정 기간 동안만 적용되는 경우 **[!UICONTROL 비율 추가]** 단추를 클릭합니다. 다음 [!UICONTROL 청구 요금 1 종료 일자] 및 [!UICONTROL 청구 요금 2] 필드가 나타납니다. 에 대한 종료 일자 입력 [!UICONTROL 청구 요금 1]. 다음에 대한 시작 일자를 입력할 수 없습니다. [!UICONTROL 청구 요금 1] 시스템이 프로젝트가 시작될 때 시작된 것으로 간주하기 때문입니다.

   ![의 프로젝트 시작 시점에 시작하여 특정 기간에 적용되는 새 청구 요금을 생성하는 이미지입니다. [!DNL Workfront]](assets/project-finances-6.png)

1. 그렇지 않은 경우:

   * 다음에 대한 기본 청구 요금 입력 [!UICONTROL 청구 요금 1].
   * 다음에 대한 종료 날짜 선택 [!UICONTROL 청구 요금 1] ([!UICONTROL 기본 청구 요금]).
   * 에 대한 시작 일자 [!UICONTROL 청구 요금 2] 다음 다음 날짜로 자동 설정됩니다. [!UICONTROL 청구 요금 1] 종료.
   * 에 원하는 청구 요금을 입력합니다. [!UICONTROL 청구 요금 2] 섹션.
   * 필요에 따라 다음을 클릭하여 청구 요금을 계속 추가합니다. **[!UICONTROL 비율 추가]** 단추를 클릭합니다.
   * 완료되면 다음을 클릭합니다. **[!UICONTROL 저장]**.
   * 모든 청구 요금이 다음에 표시됩니다. [!UICONTROL 청구 요금] 프로젝트의 탭입니다.

   ![의 서로 다른 기간에 적용되는 새 청구 요금을 생성하는 이미지입니다. [!DNL Workfront]](assets/project-finances-7.png)
