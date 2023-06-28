---
title: 기본 보기 만들기
description: Workfront에서 보기의 정의, 보기를 만드는 방법 및 다른 사용자와 보기를 공유하는 방법에 대해 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2023-06-20T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 6%

---

# 기본 보기 만들기

이 비디오에서는 다음 사항에 대해 알아봅니다.

* Workfront의 보기
* 보기를 만들고 수정하는 방법
* 다른 Workfront 사용자와 보기를 공유하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12&learn=on)

## 활동 1: 작업 상태 보기 만들기

프로젝트 관리자, 팀 리더 또는 리소스 관리자는 작업 진행률을 추적할 수 있습니다. 이 보기를 사용하면 목록 또는 보고서의 한 행에 작업의 여러 상태 표시기가 모두 표시됩니다.

다음 열을 사용하여 &quot;작업 상태 보기&quot;라는 작업 보기를 만듭니다.

* [!UICONTROL 작업 이름]
* [!UICONTROL 할당]
* [!UICONTROL 기간]
* [!UICONTROL 완료율]
* [!UICONTROL 상태]
* [!UICONTROL 진행 상태]
* [!UICONTROL 상태 아이콘]

## 활동 1 대답

![작업 상태 보기를 만드는 화면의 이미지](assets/view-exercise.png)

1. 작업 목록 보고서에서 **[!UICONTROL 보기]** 드롭다운 메뉴 및 선택 **[!UICONTROL 새 보기]**.
1. 보기의 이름을 &quot;작업 상태 보기&quot;로 지정합니다.
1. 다음 열을 제거합니다. [!UICONTROL 계획된 시간], [!UICONTROL 전임 작업], [!UICONTROL 시작 일자], 및 [!UICONTROL 마감일:].
1. 클릭 **[!UICONTROL 열 추가]**.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드에 &quot;status&quot;를 입력한 다음 [!UICONTROL 작업] 필드 소스입니다.
1. 클릭 **[!UICONTROL 열 추가]** 다시.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드에 &quot;status&quot;를 입력한 다음 [!UICONTROL 작업] 필드 소스입니다.
1. 클릭 **[!UICONTROL 열 추가]** 다시.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드에 &quot;status&quot;를 입력한 다음 작업 필드 원본에서 &quot;Status Icons&quot;를 선택하십시오.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

의 각 아이콘 위로 마우스 오버 [!UICONTROL 상태 아이콘] 열을 사용하여 표현한 내용을 확인합니다. 회색으로 표시된 경우 작업에 메모, 문서, 승인 프로세스 등이 없음을 의미합니다. 아이콘이 색상으로 표시되면 해당 항목 중 하나 이상이 작업에 연결되어 있습니다. 메모 또는 문서 아이콘을 클릭하여 해당 항목으로 이동할 수 있습니다.

## 활동 2: 마일스톤 보기 만들기

이정표를 사용하는 경우 이 보기를 통해 이름별로 이정표를 가장 쉽게 확인하고 인라인 편집을 사용하여 이정표를 추가하거나 편집할 수 있습니다.

다음 열을 사용하여 &quot;마일스톤 보기&quot;라는 작업 보기를 만듭니다.

* [!UICONTROL 작업 이름]
* [!UICONTROL 할당]
* [!UICONTROL 기간]
* [!UICONTROL 계획된 시간]
* [!UICONTROL 마일스톤: 이름]
* [!UICONTROL 시작 일자:]
* [!UICONTROL 기한:]
* [!UICONTROL 완료율]


## 활동 2 대답

![마일스톤 보기를 만드는 화면 이미지](assets/view-milestone-exercise-1.png)

1. 프로젝트 작업 목록에서 **[!UICONTROL 보기]** 드롭다운 메뉴 및 선택 **[!UICONTROL 새 보기]**.
1. 보기의 이름을 &quot;마일스톤 보기&quot;로 지정합니다.
1. 을(를) 클릭합니다 [!UICONTROL 전임 작업] 열 선택.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드에서 의 X 아이콘을 클릭합니다. [!UICONTROL 작업 >> 전임 작업] 필드를 입력한 다음 &quot;[!UICONTROL 마일스톤 이름]&quot;&quot;을(를) 클릭하고 &quot;[!UICONTROL 이름]목록에 있는 &quot;.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![마일스톤 보기를 사용하는 작업 목록의 이미지](assets/view-milestone-exercise-2.png)

## 활동 3: 기간 유형 및 태스크 제한조건 조회 생성

이 보기를 사용하면 프로젝트의 모든 기간 유형과 작업 제한을 검사하고 편집할 수 있습니다.

다음 열을 사용하여 &quot;기간 유형 및 작업 제한 보기&quot;라는 작업 보기를 만듭니다.

* [!UICONTROL 작업 이름]
* [!UICONTROL 할당]
* [!UICONTROL 기간]
* [!UICONTROL 계획된 기간]
* [!UICONTROL 계획된 시간]
* [!UICONTROL 전임 작업]
* [!UICONTROL 시작 일자:]
* [!UICONTROL 기한:]
* [!UICONTROL 기간 유형]
* [!UICONTROL 작업 제한 사항]
* [!UICONTROL 제한 일자]

변경 [!UICONTROL 필드 형식] 다음에 있음 [!UICONTROL 시작 일자] 및 [!UICONTROL 마감일:] 날짜 및 시간을 모두 표시할 열입니다.

## 활동 3 대답

![기간 유형 및 작업 제한 보기를 표시하는 화면 이미지](assets/view-activity-3.png)

1. 프로젝트 작업 목록에서 **[!UICONTROL 보기]** 드롭다운 메뉴 및 선택 **[!UICONTROL 새 보기]**.
1. 보기의 이름을 &quot;기간 유형 및 작업 제한 보기&quot;로 지정합니다.
1. 제거 [!UICONTROL % 완료] 열.
1. 클릭 **[!UICONTROL 열 추가]**.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드, 유형 [!UICONTROL &quot;duration&quot;] 그런 다음 선택 [!UICONTROL &quot;계획된 기간&quot;] 다음 아래에 [!UICONTROL 작업] 필드 소스입니다.
1. 이 열을 다음 사이에서 이동 [!UICONTROL 기간] 및 [!UICONTROL 계획된 시간] 열.
1. 클릭 **[!UICONTROL 열 추가]** 다시.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드, 유형 [!UICONTROL &quot;duration type&quot;] 그런 다음 선택 [!UICONTROL &quot;기간 유형&quot;] 다음 아래에 [!UICONTROL 작업] 필드 소스입니다.
1. 클릭 **[!UICONTROL 열 추가]** 다시.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드, 유형 [!UICONTROL &quot;제한&quot;] 그런 다음 선택 [!UICONTROL &quot;작업 제한 사항&quot;] 을 클릭합니다.
1. 클릭 **[!UICONTROL 열 추가]** 다시.
1. 다음에서 [!UICONTROL 이 열에 표시] 필드, 유형 [!UICONTROL &quot;제한&quot;] 그런 다음 선택 [!UICONTROL &quot;제한 일자&quot;] 을 클릭합니다.
1. 다음 항목 선택 [!UICONTROL 시작 일자] 열을 클릭한 다음 을(를) 클릭합니다 [!UICONTROL 고급 옵션].
1. 아래 [!UICONTROL 필드 형식] 드롭다운 선택 [!UICONTROL &quot;60년 10월 17일 오전 3시&quot;].
1. 다음 항목 선택 [!UICONTROL 마감일:] 열을 클릭한 다음 을(를) 클릭합니다 [!UICONTROL 고급 옵션].
1. 아래 [!UICONTROL 필드 형식] 드롭다운 선택 [!UICONTROL &quot;60년 10월 17일 오전 3시&quot;].
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
