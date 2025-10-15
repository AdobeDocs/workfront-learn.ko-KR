---
title: 기본 보기 만들기
description: Workfront에서 보기란 무엇인지와 보기를 만드는 방법, 다른 사용자와 보기를 공유하는 방법을 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2025-06-06T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 75%

---

# 기본 보기 만들기

이 비디오에서는 프로젝트, 작업, 문제 및 문서와 같이 목록에 있는 항목에 대한 특정 정보를 표시하기 위해 Workfront에서 보기를 만들고 사용자 지정하는 방법을 설명합니다. &#x200B; 보기를 사용하면 이름, 설명, 상태 및 항목과 관련된 기타 필드와 같은 세부 정보를 볼 수 있습니다. &#x200B;

이 비디오는 Workfront 보기의 유연성을 강조하며 작성, 사용자 지정 및 관리에 대한 단계별 지침을 제공합니다.

>[!VIDEO](https://video.tv.adobe.com/v/3450245/?captions=kor&quality=12&learn=on&enablevpops=0)

## 핵심 사항

* **보기 사용자 지정**: 사용자는 프로젝트 상태 또는 예산과 같은 특정 정보를 표시하기 위해 열을 추가, 제거 또는 다시 정렬하여 기존 보기를 편집하거나 새 보기를 만들 수 있습니다.
* **인라인 편집**: 개별 항목을 열지 않고 목록 보기의 일부 필드를 직접 업데이트할 수 있으므로 변경 속도가 빨라집니다. &#x200B;
* **처음부터 보기 만들기**: 사용자는 예산, 실제 비용 및 진행 상태와 같은 관련 열을 추가하여 프로젝트 상태 추적과 같은 특정 요구 사항에 맞게 보기를 디자인할 수 있습니다. &#x200B;
* **보기 공유 및 관리**: 사용자 지정 보기는 공동 작업을 위해 팀원과 공유하거나 더 이상 필요하지 않으면 제거할 수 있습니다.

## “기본 보기 만들기” 활동


### 활동 1: 작업 상태 보기 만들기

프로젝트 관리자, 팀 리드 또는 리소스 관리자로서 작업 진행 상황을 추적하려고 합니다. 이 보기를 사용하면 목록 또는 보고서의 한 행에서 작업의 여러 상태 표시기를 모두 볼 수 있습니다.

다음 열을 사용하여 “작업 상태 보기”라는 작업 보기를 만듭니다.

* [!UICONTROL 작업 이름]
* [!UICONTROL 할당]
* [!UICONTROL 기간]
* [!UICONTROL 완료율]
* [!UICONTROL 상태]
* [!UICONTROL 진행 상태]
* [!UICONTROL 상태 아이콘]

### 답변 1

![작업 상태 보기를 만드는 화면의 이미지](assets/view-exercise.png)

1. 작업 목록 보고서에서 **[!UICONTROL 보기]** 드롭다운 메뉴로 이동하고 **[!UICONTROL 새 보기]**&#x200B;를 선택합니다.
1. 보기 이름을 “작업 상태 보기”로 지정합니다.
1. [!UICONTROL 계획된 시간], [!UICONTROL 전임 작업], [!UICONTROL 시작 일자] 및 [!UICONTROL 기한] 열을 제거합니다.
1. **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에 “상태”를 입력한 다음 [!UICONTROL 작업] 필드 소스 아래에서 “상태”를 선택합니다.
1. 다시 **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에 “상태”를 입력한 다음 [!UICONTROL 작업] 필드 소스 아래에서 “진행 상태”를 선택합니다.
1. 다시 **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에 “상태”를 입력한 다음 작업 필드 소스 아래에서 “상태 아이콘”을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

[!UICONTROL 상태 아이콘] 열의 각 아이콘 위로 마우스를 가져다 대면 해당 아이콘이 무엇을 나타내는지 확인할 수 있습니다. 회색으로 표시된 아이콘은 작업에 메모, 문서, 승인 프로세스 등이 없음을 의미합니다. 아이콘이 컬러로 표시되어 있으면 작업과 관련된 해당 항목이 하나 이상 있는 것입니다. 메모 또는 문서 아이콘을 클릭하여 해당 항목으로 이동할 수 있습니다.

### 활동 2: 마일스톤 보기 만들기

마일스톤을 사용하는 경우 이 보기를 통해 작업 목록에서 이름별로 마일스톤을 가장 쉽게 확인하고 인라인 편집을 사용하여 작업에서 마일스톤을 추가하거나 제거할 수 있습니다.

다음 열을 사용하여 “마일스톤 보기”라는 작업 보기를 만듭니다.

* [!UICONTROL 작업 이름]
* [!UICONTROL 할당]
* [!UICONTROL 기간]
* [!UICONTROL 계획된 시간]
* [!UICONTROL 마일스톤: 이름]
* [!UICONTROL 시작 일자:]
* [!UICONTROL 기한:]
* [!UICONTROL 완료율]


### 답변 2

![마일스톤 보기를 만드는 화면의 이미지](assets/view-milestone-exercise-1.png)

1. 프로젝트 작업 목록에서 **[!UICONTROL 보기]** 드롭다운 메뉴로 이동하고 **[!UICONTROL 새 보기]**&#x200B;를 선택합니다.
1. 보기 이름을 “마일스톤 보기”로 지정합니다.
1. [!UICONTROL 전임 작업] 열을 클릭하여 선택합니다.
1. [!UICONTROL 이 열에 표시] 필드에서 [!UICONTROL 작업 >> 전임 작업] 필드의 &quot;빼기&quot; 아이콘을 클릭한 다음 &quot;[!UICONTROL 마일스톤 이름]&quot;을(를) 입력하고 목록에서 &quot;[!UICONTROL 이름]&quot;을(를) 클릭합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![마일스톤 보기를 사용하는 작업 목록의 이미지](assets/view-milestone-exercise-2.png)

### 활동 3: 기간 유형 및 작업 제한 사항 보기 만들기

이 보기를 통해 프로젝트의 모든 기간 유형 및 작업 제한 사항을 검사하고 편집할 수 있습니다.

다음 열을 사용하여 “기간 유형 및 작업 제한 사항 보기”라는 작업 보기를 만듭니다.

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

[!UICONTROL 시작 일자] 및 [!UICONTROL 기한] 열에서 [!UICONTROL 필드 형식]을 일자와 시간을 모두 표시하도록 변경합니다.

### 답변 3

![기간 유형 및 작업 제한 사항 보기를 보여 주는 화면 이미지](assets/view-activity-3.png)

1. 프로젝트 작업 목록에서 **[!UICONTROL 보기]** 드롭다운 메뉴로 이동하고 **[!UICONTROL 새 보기]**&#x200B;를 선택합니다.
1. 보기 이름을 “기간 유형 및 작업 제한 사항 보기”로 지정합니다.
1. [!UICONTROL 완료율] 열을 제거합니다.
1. **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에서 [!UICONTROL “기간”]을 입력한 다음 [!UICONTROL 작업] 필드 소스 아래에서 [!UICONTROL “계획된 기간”]을 선택합니다.
1. 이 열을 [!UICONTROL 기간] 열과 [!UICONTROL 계획된 시간] 열 사이로 이동합니다.
1. 다시 **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에서 [!UICONTROL “기간 유형”]을 입력한 다음 [!UICONTROL 작업] 필드 소스 아래에서 [!UICONTROL “기간 유형”]을 선택합니다.
1. 다시 **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에서 [!UICONTROL “제한”]을 입력한 다음 ‘작업’ 필드 소스 아래에서 [!UICONTROL “작업 제한 사항”]을 선택합니다.
1. 다시 **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에서 [!UICONTROL “제한”]을 입력한 다음 ‘작업’ 필드 소스 아래에서 [!UICONTROL “제한 일자”]를 선택합니다.
1. [!UICONTROL 시작 일자] 열을 선택한 다음 [!UICONTROL 고급 옵션]을 클릭합니다.
1. [!UICONTROL 필드 형식] 드롭다운 아래에서 [!UICONTROL &quot;10/17/60 3:00 AM&quot;]을(를) 선택합니다.
1. [!UICONTROL 기한] 열을 선택한 다음 [!UICONTROL 고급 옵션]을 클릭합니다.
1. [!UICONTROL 필드 형식] 드롭다운 아래에서 [!UICONTROL &quot;10/17/60 3:00 AM&quot;]을(를) 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

### 활동 4: 프로젝트 템플릿 활성 상태 보기 만들기

프로젝트 템플릿 관리자는 목록에 있는 각 템플릿의 활성 상태(True 또는 False)를 확인할 수 있습니다. 심지어 필드를 인라인 편집할 수도 있습니다.

다음 열이 포함된 “표준+활성 상태”라는 이름의 프로젝트 템플릿 보기를 만듭니다.

* [!UICONTROL 이름]
* [!UICONTROL 소유자]
* [!UICONTROL 기간]
* [!UICONTROL 계획된 시간]
* [!UICONTROL 계획된 비용]
* [!UICONTROL 플래그]
* [!UICONTROL 그룹 이름]
* [!UICONTROL 활성화됨]


### 답변 4

![프로젝트 템플릿 활성 상태 보기를 보여 주는 화면의 이미지](assets/view-activity-4.png)

1. 프로젝트 템플릿 목록에서 **[!UICONTROL 보기]** 드롭다운 메뉴로 이동하고 **[!UICONTROL 새 보기]**&#x200B;를 선택합니다.
1. 보기 이름을 “표준+활성 상태”로 지정합니다.
1. **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 이 열에 표시] 필드에 “is”를 입력한 다음 [!UICONTROL 템플릿] 필드 소스 아래에서 “활성화됨”를 선택합니다.
1. **[!UICONTROL 보기 저장]**&#x200B;을 클릭합니다.
