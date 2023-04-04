---
title: 에서 자산 찾기 및 구성 [!UICONTROL Workfront DAM]
description: 에서 자산을 검색하고, 폴더 내에서 검색하고, 검색 결과를 간소화하고, 메타데이터 및 키워드를 검색 필터로 사용하는 방법을 알아봅니다. [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 기여자: 자산 찾기

이 비디오에서는 다음 방법을 배웁니다.

* 자산 검색
* 폴더 내에서 검색
* 검색 결과 간소화
* 검색 필터로 메타데이터 및 키워드 사용
* 폴더 세부 사항 보기
* 자산 메타데이터 및 키워드 보기 및 업데이트

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## 기본 검색 기준

기본 검색은 파일 이름, 메타데이터 필드, 키워드 및 자산 컨텐츠를 봅니다(자산 유형에 따라 다름). 폴더 이름은 포함되지 않습니다.

대부분의 검색 결과가 정확히 일치합니다. 이 &quot;exact match&quot; 규칙의 예외는 [!UICONTROL Workfront DAM] 파일 이름 필드를 검색합니다. [!UICONTROL Workfront DAM] 정확한 파일 이름이 일치하는 경우가 아니라 부분 파일 이름 일치 항목을 반환합니다.

## 검색하는 동안 사용자 연산자

기본 검색 기능은 필요한 자산을 찾는 경우가 많지만, 수시로 추가 검색 매개 변수를 사용해야 할 수도 있습니다.

### 부분 일치

부분 일치를 찾으려면 검색어에 별표를 추가합니다. 별표는 단어의 끝에서만 사용할 수 있다.

### AND 연산자

여러 검색어가 포함된 결과를 찾으려면 단어 사이에 AND를 입력합니다. 그 단어들은 어떤 순서로도 찾을 수 있다. 모든 필드를 검색할 때 두 단어가 동일한 필드에 없을 수 있습니다. 예를 들어, Paris AND Tower는 그 두 단어를 모두 필드에 가지고 있는 자산을 찾습니다.

### OR 연산자

검색어가 포함된 자산을 찾으려면 OR 연산자를 사용하십시오. 예를 들어, Paris OR Arc는 두 단어 중 하나가 있는 자산을 찾지만 반드시 두 단어가 모두 있는 자산은 찾지 못합니다.

### 구

정확한 구를 찾으려면 단어 둘레에 큰따옴표를 사용하십시오. 모든 단어는 순서대로 찾을 수 있다. 예를 들어, &quot;에펠탑&quot;은 그 단어들을 정확한 순서로 찾습니다.

### 음수 연산자

검색 결과에서 단어를 제외하려면 단어 앞에 빼기 기호(-)를 추가합니다. 빼기 기호와 단어 사이에 공백이 없는지 확인하세요. 예를 들어 메타데이터에 &quot;tower&quot;라는 단어가 있는 자산을 제외하려면 검색을 Paris -tower로 설정할 수 있습니다.

### 빈 필드 연산자

특정 메타데이터 필드에 정보가 없는 자산을 찾으려면 검색할 필드를 다음 형식으로 입력합니다. ?[xxxxx]. 예를 들어 키워드가 지정되지 않은 자산을 찾으려면 ?[키워드] 검색 필드에서 을 클릭합니다.
