---
title: 필터
description: 모듈 간에 필터를 사용하여 특정 유형의 번들만 허용하는 방법을 알아봅니다.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# 필터

모듈 간에 필터를 사용하여 특정 유형의 번들만 허용하는 방법을 알아봅니다.

## 연습 개요

기본 매핑 이외의 시나리오의 두 모듈 사이에 필터를 추가하여 CSV 파일에 &quot;빨간색&quot; 프로젝트 색상이 있는 프로젝트만 만듭니다.

![이미지 1 필터링](../12-exercises/assets/filters-walkthrough-1.png)

## 수행할 단계

1. &quot;기본 매핑 이외의&quot; 시나리오의 클론을 만들고 이름을 &quot;강력한 필터 사용&quot;으로 지정합니다.

   **Workfront 프로젝트 만들기 모듈 앞에 필터를 추가하여 빨간색 프로젝트만 만들 수 있습니다.**

   ![이미지 2를 필터링합니다.](../12-exercises/assets/filters-walkthrough-2.png)

1. 모듈을 연결하는 점선을 클릭하거나 렌치를 클릭하고 필터 설정 을 선택하여 필터를 추가합니다.
1. 레이블 필드를 사용하여 필터 이름을 &quot;Only Red Projects&quot;로 지정합니다.
1. 조건 필드에서 프로젝트 색상 필드(CSV 파일의 열 3)를 매핑합니다. 다음과 같음(대/소문자 구분 안 함) 연산자를 선택한 다음 &quot;빨간색&quot;을 입력합니다.
1. 확인 을 클릭합니다.

   ![이미지 필터링 3](../12-exercises/assets/filters-walkthrough-3.png)

   **필터를 테스트하고 결과를 확인합니다.**

1. 저장 을 클릭하여 시나리오를 저장한 다음 한 번 실행합니다.
1. 필터에 대한 실행 관리자를 클릭하여 필터에서 각 번들을 검사한 후 Workfront 프로젝트 만들기 모듈로 전달되거나 이동하지 못한 방법을 확인합니다.

   ![이미지 4 필터링](../12-exercises/assets/filters-walkthrough-4.png)

1. Workfront 인스턴스에서 만든 프로젝트를 찾습니다.
