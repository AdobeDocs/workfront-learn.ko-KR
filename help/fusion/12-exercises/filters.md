---
title: 필터 연습
description: 모듈 사이에 필터를 사용하여 특정 유형의 번들만 허용하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# 필터 연습

모듈 사이에 필터를 사용하여 특정 유형의 번들만 허용하는 방법을 알아봅니다.

## 연습 개요

추가 기본 매핑 시나리오에서 두 모듈 사이에 필터를 추가하여 CSV 파일에 “빨간색” 프로젝트 색상이 있는 프로젝트만 만듭니다.

![필터 이미지 1](../12-exercises/assets/filters-walkthrough-1.png)

## 따라야 할 단계

1. “추가 기본 매핑” 시나리오의 복제본을 만들고 이름을 “강력한 필터 사용”으로 지정합니다.

   **Workfront 프로젝트 만들기 모듈 앞에 필터를 추가하여 빨간색 프로젝트만 만들 수 있도록 합니다.**

   ![필터 이미지 2](../12-exercises/assets/filters-walkthrough-2.png)

1. 모듈을 연결하는 점선을 클릭하거나 렌치를 클릭하고 ‘필터 설정’을 선택하여 필터를 추가합니다.
1. ‘레이블’ 필드를 사용하여 필터 이름을 “빨간색 프로젝트만”으로 지정합니다.
1. ‘상태’ 필드에서 ‘프로젝트 색상’ 필드(CSV 파일의 열 3)를 매핑합니다. ‘같음’(대소문자 구분 안 함) 연산자를 선택한 다음 “red”를 입력합니다.
1. ‘확인’을 클릭합니다.

   ![필터 이미지 3](../12-exercises/assets/filters-walkthrough-3.png)

   **필터를 테스트하고 결과를 확인합니다.**

1. ‘저장’을 클릭하여 시나리오를 저장한 다음 한 번 실행합니다.
1. 필터에 대한 실행 검사기를 클릭하여 각 번들이 필터에 의해 어떻게 검사되었는지, 그리고 Workfront 프로젝트 만들기 모듈로 이동하는 데 성공하거나 실패했는지 확인합니다.

   ![필터 이미지 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Workfront 인스턴스에서 만들어진 프로젝트를 찾습니다.
