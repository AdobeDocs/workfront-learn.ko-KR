---
title: 메타데이터 매핑 설정
description: '[!UICONTROL Workfront DAM]에 대한 메타데이터 매핑을 설정하는 방법을 알아봅니다.'
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: ht
source-wordcount: '275'
ht-degree: 100%

---

# 메타데이터 매핑 설정

자산에 대한 [!DNL Workfront] 관련 정보를 [!DNL Workfront]에서 자산과 함께 [!UICONTROL Workfront DAM]으로 전송할 수 있습니다. [!DNL Workfront] [!UICONTROL 설정] 영역의 메타데이터 매핑 옵션을 통해 이와 같이 정보를 전송할 수 있습니다.

메타데이터 매핑 설정에 대한 모범 사례 권장 사항은 [!DNL Workfront] 컨설턴트에게 문의하십시오.

[!DNL Workfront] 관리자이자 [!UICONTROL Workfront DAM] 관리자여야 메타데이터 매핑을 설정할 수 있습니다. 시작하기 전에 [!DNL Workfront] 계정과 [!UICONTROL Workfront DAM] 계정을 연결해야 합니다.

## 계정 연결

1. [!DNL Workfront]에 로그인합니다.
1. 프로젝트, 작업 또는 문제를 열고 **[!UICONTROL 문서]** 탭을 클릭합니다.
1. **[!UICONTROL 새로 추가]** 버튼을 클릭하고 드롭다운 메뉴에서 **[!UICONTROL 출처: Workfront DAM]**&#x200B;을 선택합니다.
1. 표시되는 [!UICONTROL Workfront DAM] 인증 상자에 로그인 이름 및 암호를 입력합니다.
1. 다음으로 **[!UICONTROL 예]**&#x200B;를 클릭하여 [!UICONTROL DAM] 계정에 [!DNL Workfront] 액세스 권한을 부여합니다.
1. 필요한 경우 페이지를 새로 고쳐 [!UICONTROL Workfront DAM] 액세스 권한을 업데이트합니다.

이 연결이 설정되면 이제 두 시스템 간의 메타데이터 매핑을 시작할 수 있습니다. 매핑을 시작하기 전에 [!UICONTROL Workfront DAM]에서 필요한 메타데이터 필드를 이미 만들어 둔 상태여야 합니다.

## 매핑 설정

1. [!DNL Workfront]에 로그인합니다.
1. [!UICONTROL 메인 메뉴]에서 **[!UICONTROL 설정]**&#x200B;을 선택합니다.
1. 왼쪽 패널 메뉴에서 **[!UICONTROL 문서]** 섹션을 확장합니다.
1. 그런 다음 **[!UICONTROL 메타데이터 매핑]**&#x200B;을 클릭합니다.
1. Workfront 필드에 매핑할 [!DNL Workfront] 필드의 필드 소스를 입력합니다.
1. 그런 다음 해당 또는 대상 **[!UICONTROL Workfront DAM]** 메타데이터 필드를 선택합니다.
1. **[!UICONTROL 매핑 추가]** 버튼을 클릭합니다.
1. 창 하단의 차트에 [!UICONTROL Workfront 필드 소스] 및 [!UICONTROL Workfront DAM 대상 필드]가 표시됩니다.
1. 원하는 모든 메타데이터 필드에 대해 반복합니다.

![[!DNL Workfront]](assets/01-metadata-mapping.png) [!UICONTROL 메타데이터 매핑] 화면의 스크린샷
