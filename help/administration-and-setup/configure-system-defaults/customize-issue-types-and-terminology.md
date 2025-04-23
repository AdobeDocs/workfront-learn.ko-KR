---
title: 문제 유형 및 용어 사용자 정의
description: 조직의 필요에 맞게 네 가지 기본 문제 유형을 사용자 정의하고 이름을 바꾸는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10021
exl-id: d1e5c2d6-b001-4e9e-b72d-c792c70d09e8
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 100%

---

# 문제 유형 및 용어 사용자 정의

## 기본 문제 유형의 이름 바꾸기

[!DNL Workfront]는 사용자가 생성되는 문제 종류를 분류할 수 있는 네 가지 유형의 문제를 제공합니다. 기본값:

* [!UICONTROL 버그 신고]
* [!UICONTROL 순서 변경]
* [!UICONTROL 문제]
* [!UICONTROL 요청]

기존의 문제 유형이 조직의 문제 관리 요구 사항과 일치하지 않으면 어떻게 됩니까? 또는 조직에서 다른 용어를 사용하면 어떻게 됩니까?

예를 들어 문제를 사용하여 프로젝트 위험을 추적하려는 팀이 있습니다. 시스템 관리자는 조직이 버그 보고서를 추적하지 않는다는 것을 알고 있습니다. 따라서 [!UICONTROL 버그 보고서]와 같이 사용되지 않는 문제 유형의 이름을 프로젝트 위험으로 변경할 수 있습니다.

문제 유형의 이름은 시스템 전체 수준에서 바뀌므로 변경 사항이 모든 사용자에게 적용됩니다.

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴 패널에서 **[!UICONTROL 프로젝트 환경 설정]** 섹션을 확장합니다.
1. **[!UICONTROL 상태]**&#x200B;를 선택합니다.
1. **[!UICONTROL 문제]** 탭을 선택합니다.
1. 오른쪽 상단 메뉴가 [!UICONTROL 시스템 상태]로 설정되어 있는지 확인하십시오.
1. 목록 상단에 있는 문제 유형 옆에 커서를 놓습니다. 연필 아이콘을 클릭하여 필드 편집을 활성화합니다.
1. 문제 유형의 이름을 바꿉니다.
1. 필드 외부를 클릭하여 저장합니다.

[!UICONTROL 설정]](assets/admin-fund-issue-types.png)의 [!UICONTROL 상태] 페이지에 있는 ![[!UICONTROL 문제] 탭

>[!NOTE]
>
>더 많은 문제 유형을 만들거나 문제 유형을 삭제할 수 없습니다.

<!--
learn more URLs
Customize default issue types
-->

## Workfront에서 “문제”라는 용어 변경

일부 조직에서는 “문제” 이외의 용어를 사용하여 계획되지 않은 작업 항목을 나타냅니다. 문제는 기본 용어이며 메뉴, 보고서, 필드 이름 등과 같이 소프트웨어 전체에 표시됩니다.
Workfront 관리자는 레이아웃 템플릿 기능을 사용하여 조직의 용어와 일치하도록 문제 항목의 이름을 바꿀 수 있습니다. 그런 다음 레이아웃 템플릿에 할당된 사용자에 대한 새 용어가 [!DNL Workfront] 전체에 표시됩니다.

[!UICONTROL 문제]가 강조 표시된 ![[!UICONTROL 용어] 창](assets/admin-fund-issue-custom-terminology.png)

<!--
paragraph below needs a hyperlink
-->

새로운 [!DNL Workfront] 환경: 제3부 제어 및 인터페이스 환경의 관리자 기본 사항의 학습 경로에서 시스템 및 그룹 관리자가 레이아웃 템플릿을 만드는 방법에 대해 알아봅니다.

<!--
learn more URLs
Create and manage layout templates
-->
