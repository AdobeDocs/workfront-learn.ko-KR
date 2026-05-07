---
title: 사용자로서 탐색 및 검색 이해
description: '[!UICONTROL Workfront DAM]의 Brand Connect 정의 및 탐색 방법에 대해 알아봅니다.'
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8984
exl-id: 6a7350cf-c9e3-4af6-a1bf-0f159e8eaf09
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T02:00:53.580Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 494
ht-degree: 91%

---

# 사용자로서 탐색 및 검색 이해

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 로그인하면 보이는 항목
* Brand Connect 탐색 방법
* 자산 검색 방법

>[!VIDEO](https://video.tv.adobe.com/v/3418750/?captions=kor&quality=12&learn=on&enablevpops=1)

## 기본 검색 기준

기본 검색은 파일 이름, 메타데이터 필드, 키워드 및 자산 콘텐츠(자산 유형에 따라 다름)를 찾습니다. 폴더 이름은 포함되지 않습니다.

대부분의 검색 결과는 정확히 일치합니다. 이 “완전 일치” 규칙의 예외는 [!UICONTROL Brand Connect]가 파일 이름 필드를 검색하는 경우입니다. [!UICONTROL Brand Connect]는 정확한 파일 이름 일치가 아닌 부분 파일 이름 일치를 반환합니다.

## [!UICONTROL Brand Connect]의 고급 검색

기본 검색 기능으로 필요한 자산을 찾을 수 있는 경우가 많으나, 경우에 따라 추가 검색 매개변수를 사용해야 할 수도 있습니다.

### 부분 일치

부분 일치 항목을 찾으려면 검색어에 별표를 추가합니다. 별표는 단어의 끝에만 사용할 수 있습니다.

### AND 연산자

여러 검색어가 포함된 결과를 찾으려면 단어 사이에 AND를 입력합니다. 단어는 임의의 순서로 찾을 수 있습니다. 모든 필드에서 검색할 때 동일한 필드에 두 단어가 모두 표시되지 않을 수 있습니다. 예를 들어 Paris AND tower는 모든 필드에 두 단어가 모두 포함된 자산을 찾습니다.

### OR 연산자

OR 연산자를 사용하여 검색어를 포함하는 자산을 찾습니다. 예를 들어 Paris OR Arc는 두 단어 중 하나를 포함(반드시 둘 다 포함해야 하는 것은 아님)하는 자산을 찾습니다.

### 구문

정확한 구문을 찾으려면 단어 주위에 큰따옴표를 사용합니다. 모든 단어가 순서대로 함께 검색됩니다. 예를 들어 “Eiffel Tower”는 정확한 순서로 된 해당 단어를 찾습니다.

### 부정 연산자

검색 결과에서 단어를 제외하려면 단어 앞에 빼기 기호(–)를 입력합니다. 빼기 기호와 단어 사이에 공백이 없는지 확인하십시오. 예를 들어 메타데이터에 “tower”라는 단어가 있는 자산을 제외하려면 검색을 Paris -tower로 설정할 수 있습니다.

### 빈 필드 연산자

특정 메타데이터 필드에 정보가 없는 에셋을 찾으려면 검색할 필드를 ?[xxxxx] 형식으로 입력하십시오. 예를 들어 키워드가 할당되지 않은 자산을 찾으려면 검색 필드에 ?[keyword]을 입력하십시오.

## 브랜드 지침

브랜드 지침은 조직의 브랜드가 작동하는 방식을 설명하는 일련의 규칙입니다. 브랜드 표준, 스타일 가이드, 브랜드 북 또는 브랜드 아이덴티티 안내서라고도 하는 이러한 지침에는 다음이 포함될 수 있습니다.

* 브랜드의 역사, 비전, 성격 및 어조에 대한 개요입니다.
* 회사 로고를 사용할 때 해야 할 일과 하지 말아야 할 일
* 인쇄 및 웹용으로 승인된 글꼴의 예
* 회사의 기본 및 보조 색상 분석
* 브랜드와 잘 어울리는 이미지 스타일 및 사진 샘플

[!UICONTROL Brand Connect]에 로그인하면 상단 탐색 막대에서 브랜드 지침을 클릭하여 지침에 액세스합니다.
