---
title: 여러 청구 비율 이해
description: 프로젝트 내에서 시스템 청구 비율을 무시하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 여러 청구 비율 이해

내 [!DNL Workfront]를 설정하는 경우 프로젝트 관리자는 특정 프로젝트 내에서 시스템 청구 비율을 무시할 수 있습니다. 이전에는 새 청구 비율이 프로젝트에 적용되었을 때 향후 시간뿐만 아니라 프로젝트에 이미 로그인한 시간도 영향을 받았습니다.

사용 [!DNL Workfront]의 새로운 다중 청구 비율 기능을 통해 프로젝트 관리자는 청구 비율을 적용할 기간을 결정할 수 있습니다. 이렇게 하면 비율이 협상되거나 변경된 경우 프로젝트 관리자가 해당 비율이 적용되는 시기를 결정할 수 있습니다.

## 청구 비율 변경

1. 프로젝트의 랜딩 페이지로 이동합니다. 선택 **[!UICONTROL 청구 비율]** 왼쪽 패널에서 생성합니다.

   ![선택 이미지 [!UICONTROL 청구 비율] in [!DNL Workfront]](assets/project-finances-1.png)

1. 에서 **[!UICONTROL 청구 비율]** 탭에서 **[!UICONTROL 청구 비율 추가]** 버튼을 클릭합니다. 선택 **[!UICONTROL 신규 청구 비율]** 드롭다운

   ![선택 이미지 [!UICONTROL 신규 청구 비율] in [!DNL Workfront]](assets/project-finances-2.png)

1. 다음 [!UICONTROL 신규 청구 비율] 대화 상자가 나타납니다. 에서 **[!UICONTROL 작업 역할]** 드롭다운에서 새 청구 비율이 적용될 작업 역할을 선택합니다.

   ![의 새 청구 비율로 작업 역할을 선택하는 이미지 [!DNL Workfront]](assets/project-finances-3.png)

1. 작업 역할을 선택하면 [!UICONTROL 기본 청구 비율] 그리고 [!UICONTROL 청구 비율 1] 필드가 나타납니다. 에 신규 청구 비율을 입력합니다. [!UICONTROL 청구 비율 1] 필드. 해당 청구 비율이 전체 프로젝트(과거, 현재 및 로그된 이후 시간)에 적용되는 경우 **[!UICONTROL 저장]** 버튼을 클릭합니다.

   ![전체 프로젝트에 적용되는 새 청구 비율을 저장하는 이미지 [!DNL Workfront]](assets/project-finances-5.png)

1. 새 청구 비율이 특정 기간 동안만 적용되는 경우 **[!UICONTROL 비율 추가]** 버튼을 클릭합니다. 다음 [!UICONTROL 청구 비율 1 종료 날짜] 그리고 [!UICONTROL 청구 비율 2] 필드가 나타납니다. 종료 일자 입력 [!UICONTROL 청구 비율 1]. 시작 일자를 입력할 수 없습니다 [!UICONTROL 청구 비율 1] 시스템은 프로젝트 시작 부분에서 시작되었다고 간주하므로

   ![에서 프로젝트 시작 시점부터 일정 기간에 적용되는 새 청구 비율을 생성하는 이미지입니다 [!DNL Workfront]](assets/project-finances-6.png)

1. 그렇지 않은 경우:

   * 에 대한 기본 청구 비율을 입력합니다 [!UICONTROL 청구 비율 1].
   * 종료 날짜 선택 [!UICONTROL 청구 비율 1] ([!UICONTROL 기본 청구 비율]).
   * 에 대한 시작 날짜 [!UICONTROL 청구 비율 2] 은(는) 자동으로 다음 날로 설정됩니다. [!UICONTROL 청구 비율 1] 종료.
   * 원하는 청구 비율을 입력합니다. [!UICONTROL 청구 비율 2] 섹션을 참조하십시오.
   * 필요에 따라 **[!UICONTROL 비율 추가]** 버튼을 클릭합니다.
   * 완료되면 를 클릭합니다 **[!UICONTROL 저장]**.
   * 모든 청구 비율은 [!UICONTROL 청구 비율] 탭에서 사용할 수 있습니다.
   ![의 다른 기간에 적용되는 새 청구 비율을 생성하는 이미지 [!DNL Workfront]](assets/project-finances-7.png)
