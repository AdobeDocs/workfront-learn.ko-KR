---
title: 기본 조건부 서식 추가
description: 이 비디오에서는 보기에 조건부 서식이 무엇인지, 에서 조건부 서식을 만들고 수정하는 방법을 알아봅니다 [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
source-git-commit: b09d634a8b4ec32eda2663f1df04cc8bc04596a9
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 보기에 기본 조건부 서식 추가

이 비디오에서는 다음을 학습합니다.

* 보기에 조건부 서식 지정
* 조건부 서식을 만들고 수정하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12)

## 활동: 보기에 조건부 서식 추가

기존 표준 보기를 사용하고 이 조건부 서식을 [!UICONTROL 이름] 열.

1. 작업의 진행 상태가 늦을 때 필드 배경이 빨간색으로 바뀌는 열 규칙을 추가합니다.
1. 진행 상태가 &quot;뒤로&quot; 또는 &quot;위험&quot; 상태일 때 필드 배경색을 노란색으로 변경하는 열 규칙을 추가합니다.

진행 상태 열을 보기의 일부로 포함하지 않고 문제가 있는 작업을 발견하는 데 도움이 됩니다.

## 답변

![새 열 규칙을 만드는 화면의 이미지입니다](assets/conditional-formatting-exercise.png)

1. 작업 목록 보고서에서 **[!UICONTROL 보기]** 드롭다운 메뉴를 선택하고 **[!UICONTROL 새 보기]**.
1. 보기의 이름을 &quot;Standard + Progress&quot;로 지정합니다.
1. 제공된 기본 열을 사용합니다.
1. 을(를) 선택합니다 [!UICONTROL 작업 이름] 열. 조건부 서식을 적용하려는 열이므로 작업의 진행 상태가 On Time이 아닌 경우 빨간색 또는 노란색으로 표시됩니다.
1. 클릭 **[!UICONTROL 고급 옵션]** ( report builder 창의 오른쪽 상단 모서리에서)를 클릭합니다.
1. 클릭 **[!UICONTROL 이 열에 대한 규칙 추가]**.
1. 다음을 변경하여 열 규칙 시작 [!UICONTROL 작업] > [!UICONTROL 이름] 창 상단에서 [!UICONTROL 작업] > [!UICONTROL 진행 상태]. 을(를) 클릭합니다. **[!UICONTROL X]** 아이콘 옆에 있는 아이콘 [!UICONTROL 작업] > [!UICONTROL 이름] 필드에서 삭제할 수 있습니다.
1. 필드에 &quot;progress&quot;를 입력한 다음 을 선택합니다 [!UICONTROL 진행 상태] 아래에 [!UICONTROL 작업] 필드 소스.
1. 선택 **[!UICONTROL 늦게]** 오른쪽 필드에서 [!UICONTROL Equal] 한정자입니다.
1. 에서 빨간색 배경을 선택합니다 [!UICONTROL 텍스트 색상] 행을 클릭합니다.
1. 클릭 **[!UICONTROL 규칙 추가]** 열 규칙을 저장하려면 다음을 수행합니다.
1. 이제 **[!UICONTROL 열 규칙 추가]** 다른 규칙을 추가하려면 다시 하십시오.
1. 전과 마찬가지로 삭제 [!UICONTROL 작업] > [!UICONTROL 이름] 기준 필드에서 을 선택합니다. 다음으로 바꾸기 [!UICONTROL 진행 상태] 아래에 [!UICONTROL 작업] 필드 소스.
1. 둘 다 선택 [!UICONTROL 위험] 및 [!UICONTROL 뒤] Equal Qualifier의 오른쪽에 있는 필드에 있습니다.
1. 에서 노란색 배경을 선택합니다 [!UICONTROL 텍스트 색상] 행을 클릭합니다.
1. 클릭 **[!UICONTROL 규칙 추가]** 열 규칙을 저장하려면 다음을 수행합니다.
1. 클릭 **[!UICONTROL 보기 저장]** 보기를 저장합니다.
