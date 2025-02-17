---
title: '[!UICONTROL Brand Connect] 모양 사용자 정의'
description: '[!UICONTROL Workfront DAM]의 [!UICONTROL Brand Connect]에서 탐색 막대 및 바닥글을 사용자 정의하고 홈 페이지 및 로그인 페이지를 사용자 정의하는 방법을 알아봅니다.'
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '373'
ht-degree: 100%

---

# [!UICONTROL Brand Connect] 모양 사용자 정의

이 비디오에서는 다음 방법을 배우게 됩니다.

* 탐색 막대 및 바닥글 사용자 정의
* 홈 페이지 및 로그인 페이지 사용자 정의

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on&enablevpops)

## 추가 [!UICONTROL 모양] 설정

[!UICONTROL 모양] 메뉴의 [!UICONTROL 글꼴] 옵션은 선택한 글꼴로 [!UICONTROL Brand Portal] 전체의 모든 텍스트 스타일을 지정합니다. 800여 개의 Google 글꼴이 지원됩니다.

![[!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)의 [!UICONTROL 모양] 메뉴 스타일 아래의 [!UICONTROL 글꼴] 옵션

## 홈 페이지 위젯

조직에 맞게 [!UICONTROL Brand Connect] 홈 페이지의 디자인을 사용자 정의합니다. 위젯을 사용하여 폴더 및 이미지 슬라이더와 같은 요소를 추가할 수 있습니다. 조직에 여러 [!UICONTROL Brand Connect]가 있는 경우, 각각 고유한 홈 페이지가 있어 뚜렷한 디자인을 선사할 수 있습니다.

![[!UICONTROL Brand Connect] 홈 페이지의 사용 가능한 위젯 스크린샷](assets/03-brand-connect-home-page-widgets.png)

다음 위젯을 사용할 수 있습니다.

**A. 캐러셀**- 이미지 슬라이더에 여러 자산을 표시합니다. 각 자산에 설명을 추가할 수 있습니다. 추가 아이콘을 클릭하여 캐러셀에 표시할 이미지를 선택합니다.

**B. 폴더**- 선택한 자산이 포함된 폴더를 표시합니다. 추가 아이콘을 클릭하여 [!UICONTROL 자산 선택기]를 열어 폴더를 선택할 수 있습니다. 폴더 자산은 [!UICONTROL Brand Connect] 사용자에게 표시되지만, 권한이 있는 사용자만 다운로드할 수 있습니다.

**C. 라이트박스**- 기존 [!UICONTROL 라이트박스]를 표시합니다. [!UICONTROL 라이트박스]의 자산은 [!UICONTROL Brand Connect] 사용자에게 표시되나 권한이 있는 사용자만 다운로드할 수 있습니다.

**D. 브랜드 지침**- 상단 탐색 막대에서 대신/추가로 홈 페이지에 브랜드 지침을 표시합니다.

**E. 설명**- 짧은 텍스트를 표시합니다.

**F. 채워진 설명**- 회색 배경에 표시할 텍스트 복사 블록을 입력합니다.

**G. HTML**- HTML 및 CSS를 사용하여 사용자 정의 콘텐츠를 만듭니다. 예를 들어 비디오에 대한 링크를 임베드할 수 있습니다. 다음은 몇 가지 [피해야 할 HTML 태그](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html)입니다.

## 검색 창 추가

조직의 [!UICONTROL Brand Connect]에 대한 사용자 정의 홈 페이지를 설계하는 경우, 사용자는 [!UICONTROL 자산] 영역을 클릭하여 검색을 실행해야 합니다.

그러나 시스템 관리자는 HTML 위젯과 다음 HTML 태그를 사용하여 검색 창을 만들 수 있습니다.

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
