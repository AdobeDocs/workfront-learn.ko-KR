---
title: 여러 과금 요율 이해
description: 프로젝트 내에서 시스템 과금 요율을 재정의하는 방법을 알아봅니다.
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
workflow-type: ht
source-wordcount: '427'
ht-degree: 100%

---

# 여러 과금 요율 이해

[!DNL Workfront] 내에서 프로젝트 관리자는 특정 프로젝트 내의 시스템 과금 요율을 재정의할 수 있습니다. 이전에는 새 과금 요율이 프로젝트에 적용되면 향후 시간뿐만 아니라 이미 프로젝트에 로그인한 시간에도 영향을 미쳤습니다.

프로젝트 관리자는 [!DNL Workfront]의 새로운 여러 과금 요율 기능을 사용하여 과금 요율을 적용해야 하는 기간을 정할 수 있습니다. 이렇게 하면 요율이 협상되었거나 변경된 경우 프로젝트 관리자가 해당 요율이 적용되는 시기를 결정할 수 있습니다.

## 과금 요율 변경

1. 프로젝트의 랜딩 페이지로 이동합니다. 왼쪽 패널에서 **[!UICONTROL 과금 요율]**&#x200B;을 선택합니다.

   ![[!DNL Workfront]](assets/project-finances-1.png)에서 [!UICONTROL 과금 요율]을 선택하는 이미지

1. **[!UICONTROL 과금 요율]** 탭에서 **[!UICONTROL 과금 요율 추가]** 버튼을 클릭합니다. 드롭다운에서 **[!UICONTROL 새로운 과금 요율]**&#x200B;을 선택합니다.

   ![[!DNL Workfront]](assets/project-finances-2.png)에서 [!UICONTROL 새로운 과금 요율]을 선택하는 이미지

1. [!UICONTROL 새로운 과금 요율] 대화 상자가 표시됩니다. **[!UICONTROL 작업 역할]** 드롭다운에서 새로운 과금 요율을 적용할 작업 역할을 선택합니다.

   ![[!DNL Workfront]](assets/project-finances-3.png)에서 새로운 과금 요율의 작업 역할을 선택하는 이미지

1. 작업 역할을 선택하면 [!UICONTROL 기본 과금 요율] 및 [!UICONTROL 과금 요율 1] 필드가 나타납니다. [!UICONTROL 과금 요율 1] 필드에 새로운 과금 요율을 입력합니다. 해당 과금 요율이 전체 프로젝트(기록된 과거, 현재 및 미래 시간)에 적용되는 경우, **[!UICONTROL 저장]** 버튼을 클릭합니다.

   ![[!DNL Workfront]](assets/project-finances-5.png)에서 전체 프로젝트에 적용되는 새로운 과금 요율을 저장하는 이미지

1. 새로운 과금 요율이 특정 기간에만 적용되는 경우, **[!UICONTROL 요율 추가]** 버튼을 클릭합니다. [!UICONTROL 과금 요율 1 종료 일자] 및 [!UICONTROL 과금 요율 2] 필드가 나타납니다. [!UICONTROL 과금 요율 1]에 대한 종료 일자를 입력합니다. 시스템이 프로젝트가 시작될 때 시작되었다고 가정하기 때문에 [!UICONTROL 과금 요율 1]에 대한 시작 일자를 입력할 수 없습니다.

   ![[!DNL Workfront]](assets/project-finances-6.png)에서 프로젝트 시작 시 특정 기간 동안 적용되는 새로운 과금 요율을 생성하는 이미지

1. 그러지 않은 경우:

   * [!UICONTROL 과금 요율 1]에 대한 기본 과금 요율을 입력합니다.
   * [!UICONTROL 과금 요율 1]([!UICONTROL 기본 과금 요율])에 대한 종료 일자를 선택합니다.
   * [!UICONTROL 과금 요율 2]에 대한 시작 일자는 [!UICONTROL 과금 요율 1]이 종료되는 다음 날로 자동 설정됩니다.
   * [!UICONTROL 과금 요율 2] 섹션에 원하는 과금 요율을 입력합니다.
   * **[!UICONTROL 요율 추가]** 버튼을 클릭하여 필요에 따라 과금 요율을 계속 추가합니다.
   * 완료되면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
   * 모든 과금 요율은 프로젝트의 [!UICONTROL 과금 요율] 탭에 표시됩니다.

   ![[!DNL Workfront]](assets/project-finances-7.png)에서 다양한 기간에 적용되는 새로운 과금 요율을 생성하는 이미지
