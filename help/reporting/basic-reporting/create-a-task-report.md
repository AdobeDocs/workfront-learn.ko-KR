---
title: 작업 보고서 만들기
description: 복잡한 필터로 작업 보고서를 만들고 Workfront에서 만든 보고서를 찾는 방법에 대해 알아봅니다. 활동 - 프롬프트가 있는 메모 보고서를 만듭니다.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 11%

---

# 작업 보고서 만들기

이 비디오에서는 다음 사항에 대해 알아봅니다.

* 복잡한 필터로 작업 보고서를 만드는 방법
* 만든 보고서를 찾는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## 활동: 프롬프트가 있는 메모 보고서 만들기

메모 내용, 작성자, 입력 날짜, 프로젝트 이름 또는 감사 유형을 기반으로 사용자 메모(댓글 또는 업데이트) 또는 시스템 메모를 검색하는 데 사용할 수 있는 메모 보고서를 만듭니다. 보고서 이름을 &quot;메모 검색&quot;으로 지정합니다.

참고 텍스트 프롬프트를 사용할 때 이 보고서는 업데이트 스레드 내에서 검색하여 프롬프트에 지정된 기준을 충족하는 스레드를 신속하게 추출합니다. 보고서를 실행할 때 모든 프롬프트를 작성할 필요가 없으며, 필요한 메시지만 입력해야 합니다. 빈 항목은 자동으로 무시됩니다.

보기에는 다음 열이 포함되어야 합니다.

* 참고 텍스트
* 텍스트 심사
* 시작 날짜
* 소유자: 이름
* 감사 유형
* 작업 이름
* 문제 이름

필터 탭을 비워 둡니다.

프로젝트 이름의 그룹.

다음에 대한 프롬프트를 포함합니다.

* 텍스트 심사
* 참고 텍스트
* 소유자 이름
* 시작 날짜
* 프로젝트 이름
* 감사 유형

## 답변

1. 선택 **[!UICONTROL 보고서]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 다음을 클릭합니다. **[!UICONTROL 새 보고서]** 메뉴 및 선택 **[!UICONTROL 참고]**.
1. 위치 **[!UICONTROL 열(보기)]** 다음을 포함하도록 열 설정:

   ![메모 보고서 열을 만들기 위한 화면의 이미지](assets/note-report-columns.png)

   * [!UICONTROL 참고] > [!UICONTROL 메모 텍스트]
   * [!UICONTROL 참고] > [!UICONTROL 감사 텍스트]
   * [!UICONTROL 참고] > [!UICONTROL 입력 일자]
   * [!UICONTROL 소유자] > [!UICONTROL 이름]
   * [!UICONTROL 참고] > [!UICONTROL 감사 유형]
   * [!UICONTROL 작업] > [!UICONTROL 이름]
   * [!UICONTROL 문제] > [!UICONTROL 이름]

1. 다음 항목 선택 **[!UICONTROL 입력 일자]** 열 및 변경 **[!UICONTROL 내림차순으로 정렬]**.
1. 다음에서 **[!UICONTROL 그룹화]** 탭, 보고서를 그룹화 기준으로 설정 [!UICONTROL 프로젝트] > [!UICONTROL 이름].

   ![메모 보고서 그룹화를 만들기 위한 화면 이미지](assets/note-report-groupings.png)

1. 나가기 [!UICONTROL 필터] 비어 있음.
1. 열기 **[!UICONTROL 보고서 설정]** 보고서 이름을 &quot;메모 검색&quot;으로 지정합니다.
1. 다음에서 [!UICONTROL 설명] 필드에는 &quot;선택한 감사 유형 및 기타 프롬프트에 따라 시스템 또는 사용자 메모 검색&quot;과 같은 것을 입력합니다. 시스템 메모는 감사 텍스트 열에 나타나고 사용자 메모는 메모 텍스트 열에 나타납니다.&quot;

   ![메모 보고서 설정을 만드는 화면 이미지](assets/note-report-report-options.png)

1. 선택 **[!UICONTROL 세부 정보 탭]** 보고서가 로드될 때 표시됩니다.
1. 보고서가 대시보드에 포함되어 있을 때 200개의 항목이 표시되도록 보고서를 설정하십시오.
1. 클릭 **[!UICONTROL 보고서 프롬프트]** 및 추가:

   ![메모 보고서 프롬프트를 만들 화면 이미지](assets/note-report-report-prompts.png)

   * [!UICONTROL 참고] > [!UICONTROL 감사 텍스트]
   * [!UICONTROL 참고] > [!UICONTROL 메모 텍스트]
   * [!UICONTROL 소유자] > [!UICONTROL 이름]
   * [!UICONTROL 참고] > [!UICONTROL 입력 일자]
   * [!UICONTROL 프로젝트] > [!UICONTROL 이름]
   * [!UICONTROL 참고] > [!UICONTROL 감사 유형]

1. 다음 확인란을 선택합니다. **[!UICONTROL 대시보드에 프롬프트 표시]**.
1. 보고서를 저장하고 닫습니다.
