---
title: 기본 조건부 서식 추가
description: 설정한 기준에 따라 열 규칙을 사용하여 보고서나 보기의 텍스트 색상, 서식 및 배경색을 변경하는 방법에 대해 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 보기에 기본 조건부 서식 추가

조건부 서식은 열 규칙을 만들어 수행합니다. 열 규칙을 사용하면 설정한 기준에 따라 특정 방식으로 열 서식을 지정할 수 있습니다.

이 비디오에서는 다음 사항에 대해 알아봅니다.

* 보기에 있는 조건부 서식
* 조건부 서식을 만들고 수정하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## 요약

조건부 서식을 만들려면 다음 작업을 수행하십시오.

1. 서식을 표시할 열을 선택합니다
1. 서식을 변경할 조건 결정
1. 가장 적합한 서식 변경 유형을 결정합니다.

   * 배경색
   * 텍스트 색상
   * 대체 텍스트
   * 아이콘 표시

## 활동: 보기에 조건부 서식 추가

기존 표준 보기를 사용하고 의 조건부 서식에 이 조건부 서식을 추가하여 &quot;표준 + 진행률&quot;이라는 작업 보기를 만듭니다. [!UICONTROL 이름] 열.

1. 작업의 진행 상태가 [지연]일 때 필드를 빨간색으로 만드는 열 규칙을 추가합니다.
1. 진행 상태가 지연되거나 위험 상태일 때 필드 배경을 노란색으로 표시하는 열 규칙을 추가합니다.

진행률 상태에 대한 열을 보기의 일부로 포함하지 않고 문제가 발생한 작업을 찾는 데 도움이 됩니다.

## 답변

![새 열 규칙을 만들기 위한 화면 이미지](assets/conditional-formatting-exercise.png)

1. 작업 목록 보고서에서 **[!UICONTROL 보기]** 드롭다운 메뉴 및 선택 **[!UICONTROL 새 보기]**.
1. 보기의 이름을 &quot;Standard + Progress&quot;로 지정합니다.
1. 제공된 기본 열을 사용합니다.
1. 다음 항목 선택 [!UICONTROL 작업 이름] 열. 조건부 서식을 적용할 열이므로 작업의 진행 상태가 정시가 아니면 빨간색이나 노란색으로 표시됩니다.
1. 클릭 **[!UICONTROL 고급 옵션]** report builder 창의 오른쪽 상단 모서리입니다.
1. 클릭 **[!UICONTROL 이 열에 대한 규칙 추가]**.
1. 다음을 변경하여 열 규칙 시작 [!UICONTROL 작업] > [!UICONTROL 이름] 을(를) 위해 창 맨 위에서 [!UICONTROL 작업] > [!UICONTROL 진행 상태]. 을(를) 클릭합니다. **[!UICONTROL X]** 아이콘 옆에 있음 [!UICONTROL 작업] > [!UICONTROL 이름] 필드에서 삭제합니다.
1. 필드에 &quot;progress&quot;를 입력한 다음 을(를) 선택합니다 [!UICONTROL 진행 상태] 다음 아래에 [!UICONTROL 작업] 필드 소스입니다.
1. 선택 **[!UICONTROL 지연]** 의 오른쪽에 있는 필드에서 [!UICONTROL 같음] 한정자.
1. 에서 빨간색 배경 선택 [!UICONTROL 텍스트 색상] 행.
1. 클릭 **[!UICONTROL 규칙 추가]** 열 규칙을 저장합니다.
1. 이제 클릭 **[!UICONTROL 열 규칙 추가]** 다시 한 번 클릭하여 다른 규칙을 추가합니다.
1. 이전과 동일하게 삭제 [!UICONTROL 작업] > [!UICONTROL 이름] 기준 필드에서 참조할 수 있습니다. 다음으로 바꾸기 [!UICONTROL 진행 상태] 다음 아래에 [!UICONTROL 작업] 필드 소스입니다.
1. 둘 다 선택 [!UICONTROL 위험 상태] 및 [!UICONTROL 늦음] 를 입력합니다.
1. 에서 노란색 배경 선택 [!UICONTROL 텍스트 색상] 행.
1. 클릭 **[!UICONTROL 규칙 추가]** 열 규칙을 저장합니다.
1. 클릭 **[!UICONTROL 보기 저장]** 를 클릭하여 보기를 저장합니다.
