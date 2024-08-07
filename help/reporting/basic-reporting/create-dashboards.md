---
title: 대시보드 만들기
description: 다양한 목록 보고서, 차트, 캘린더 및 외부 웹 페이지를 Workfront의 대시보드에 결합하는 방법에 대해 알아봅니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
exl-id: 7adc2aeb-6618-4894-acc3-298e35175854
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 100%

---

# 대시보드 만들기

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* Workfront 대시보드 정의
* 대시보드를 만드는 방법
* 대시보드를 찾아서 사용하는 방법
* 다른 Workfront 사용자와 대시보드를 공유하는 방법
* 대시보드를 인쇄하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335157/?quality=12&learn=on)

## 활동: 대시보드 만들기

“이 프로젝트에서 메모 검색”이라는 하나의 보고서만 포함된 [!UICONTROL 대시보드]를 만듭니다. 검색할 업데이트가 수천 개인 경우에도 한 프로젝트에서 수행된 모든 업데이트를 빠르게 찾는 데 유용합니다. 이렇게 하면 업데이트 스레드를 검색하여 프롬프트에서 지정한 기준을 충족하는 모든 업데이트를 빠르게 추출합니다.

“메모 보고서 만들기” 활동에서 만든 “메모 검색” 보고서의 사본을 만들어 이 보고서를 만듭니다(또는 해당 활동을 수행하지 않은 경우 다른 보고서 사용).

* 사본에서 프로젝트 이름 프롬프트를 제거하고 “이 프로젝트에서 메모 검색” 보고서 이름을 바꿉니다.
* [!UICONTROL 대시보드] 이름을 “메모 검색”으로 지정합니다.
* 프로젝트 랜딩 페이지로 이동하여 [!UICONTROL 대시보드]의 사용자 정의 섹션을 만듭니다.
* 사용자 정의 섹션에서 메모를 검색하면 현재 있는 프로젝트에 포함된 메모만 표시됩니다.

## 답변

1. “메모 보고서 만들기” 활동에서 만든 보고서를 실행합니다.
1. **[!UICONTROL 보고서 작업]**&#x200B;을 클릭하고 **[!UICONTROL 복사]**&#x200B;를 선택합니다. [!DNL Workfront]는 “메모 검색 (사본)”이라는 새 보고서를 만듭니다.
1. **[!UICONTROL 보고서 작업]**&#x200B;으로 이동하여 **[!UICONTROL 편집]**&#x200B;을 선택합니다. **[!UICONTROL 보고서 설정]**&#x200B;을 클릭하고 이름을 “이 프로젝트에서 메모 검색”으로 변경합니다.
1. [!UICONTROL 보고서 프롬프트]를 클릭하고 목록에서 [!UICONTROL 프로젝트] > [!UICONTROL 이름] 프롬프트를 삭제합니다.

   ![새 대시보드를 생성하는 화면 이미지](assets/edit-report-prompts.png)

1. **[!UICONTROL 대시보드에 프롬프트 표시]** 상자를 선택합니다.
1. **[!UICONTROL 완료]**&#x200B;를 클릭한 다음, **[!UICONTROL 저장 및 닫기]**&#x200B;를 클릭합니다. 이제 보고서의 [!UICONTROL 프롬프트] 화면이 표시됩니다.

   다음에는 바로 가기를 사용하여 새 대시보드를 만들고 이 보고서를 추가합니다.

1. **[!UICONTROL 보고서 작업]**&#x200B;을 클릭하고 **[!UICONTROL 대시보드에 추가]** > **[!UICONTROL 새 대시보드]**&#x200B;를 선택합니다.
1. **[!UICONTROL 레이아웃]** 패널에 “이 프로젝트에서 메모 검색” 보고서를 끌어서 놓습니다.
1. 보고서 이름이 대시보드 이름이 됩니다. 이름을 “메모 검색”으로 편집합니다.

   ![새 대시보드를 생성하는 화면 이미지](assets/create-dashboard.png)

1. **[!UICONTROL 저장 및 닫기]**&#x200B;를 클릭합니다.

   이제 프로젝트 페이지에 대시보드를 추가합니다.

   ![새 대시보드를 생성하는 화면 이미지](assets/add-custom-section.png)

1. 프로젝트로 이동합니다. 왼쪽 패널 메뉴에서 **[!UICONTROL 사용자 정의 섹션 추가]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 대시보드 추가]** 필드에서 “메모 검색”을 입력한 다음, 목록에서 [!UICONTROL 대시보드]를 선택합니다.
1. **[!UICONTROL 사용자 정의 섹션 제목]** 필드에서 “메모 검색”을 입력합니다.
1. **[!UICONTROL 새 섹션 추가]**&#x200B;를 클릭합니다.
1. 왼쪽 패널 메뉴에서 메모 검색을 찾습니다. 섹션 이름 왼쪽에 있는 점을 클릭하고 업데이트 바로 아래로 끌어서 놓습니다.
