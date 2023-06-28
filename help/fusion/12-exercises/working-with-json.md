---
title: JSON 작업
description: 시나리오 내에서 JSON을 만들고 구문 분석하여 디자인 요구 사항을 지원하는 방법에 대해 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# JSON 작업

시나리오 내에서 JSON을 만들고 구문 분석하여 디자인 요구 사항을 지원하는 방법에 대해 알아봅니다.

## 연습 개요

이 연습의 목적은 시나리오에 전송된 정보를 JSON 형식으로 활용하여 시나리오 전체에 매핑할 수 있는 필드 및 항목으로 구문 분석하는 방법을 개념적으로 보여 주는 것입니다. 그런 다음 매핑된 배열의 정보를 가져오거나 JSON에 정보를 집계하여 JSON을 수신 입력으로 예상하는 다른 시스템으로 전송할 수 있습니다.

![json 이미지 1을 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-1.png)

## 따라야 할 단계

**데이터 구조를 만들고 JSON을 구문 분석합니다.**

1. 새 시나리오를 만들고 이름을 &quot;JSON 도넛 데이터 작업&quot;으로 지정합니다.
1. 트리거 모듈의 경우 변수 설정 모듈을 사용합니다.
1. 변수 이름에 &quot;도넛 데이터&quot;를 입력합니다.
1. 변수 값의 경우 테스트 드라이브의 Fusion Exercise Files 폴더에 있는 &quot;_Donut Data - Sample JSON.rtf&quot; 문서의 내용을 복사하여 붙여넣습니다.

   ![json 이미지 2를 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. 이 모듈의 이름을 &quot;다른 커넥터에서 JSON&quot;으로 바꿉니다.
1. JSON 구문 분석 모듈을 추가합니다.
1. 데이터 구조 필드에 대해 추가를 클릭합니다.
1. 생성기 를 선택하고 샘플 데이터 필드에 복사한 도넛 데이터 - 샘플 JSON 데이터를 붙여넣습니다.

   ![json 이미지 3을 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. 데이터 구조의 이름을 &quot;도넛 데이터&quot;로 지정하여 저장을 클릭합니다. 그런 다음 [저장]을 클릭합니다.
1. 변수 설정 모듈의 도넛 데이터를 JSON 문자열 필드에 매핑합니다.

   ![json 이미지 4를 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. 시나리오를 저장한 다음 실행을 한 번 클릭하여 출력을 확인합니다.

   **JSON 구문 분석 모듈의 출력은 다음과 같아야 합니다.**

   ![json 이미지 5를 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **특정 배열 변수에 매핑**

1. JSON 구문 분석 모듈 뒤에 라우터를 추가합니다.
1. 맨 위 경로에 변수 설정 모듈을 추가합니다.
1. Variable 이름에 &quot;Batter types by donut&quot;을 입력합니다.
1. Variable 값의 경우 map 함수를 사용하여 타자 배열에서 타자 유형을 가져옵니다.

   ![json 이미지 6을 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. 확인, 실행을 차례로 클릭합니다.
1. 실행 검사기를 열어 세 가지 작업 각각에 대한 출력 번들을 확인하고 각 작업의 타자 유형을 표시합니다.

   ![json 이미지 7을 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **시나리오 데이터를 JSON에 집계합니다.**

1. 하위 라우팅 경로에서 JSON 모듈에 집계를 추가합니다.
1. 소스 모듈의 경우 반복자(JSON 구문 분석 모듈)를 선택합니다.
1. 데이터 구조에 대해 데이터 구조를 만들거나 선택합니다. 이 예제에서는 도넛 데이터를 사용합니다.
1. 계속해서 아래 표시된 대로 이 예제에 대해 직접 필드를 매핑합니다.
1. 타자와 토핑에 도달하면 배열이 표시되므로 항목 추가 를 클릭하여 매핑해야 합니다.

   ![json 이미지 8을 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. 시나리오를 저장하고 실행 을 한 번 클릭합니다.

실행 검사기에서 JSON으로 집계 모듈을 확인하고 세 개의 번들을 하나의 JSON 문자열로 집계하는 방법을 확인합니다. 그런 다음 이 문자열을 JSON이 필요한 다른 시스템으로 보낼 수 있습니다.

![json 이미지 9를 사용하여 작업](../12-exercises/assets/working-with-json-walkthrough-9.png)
