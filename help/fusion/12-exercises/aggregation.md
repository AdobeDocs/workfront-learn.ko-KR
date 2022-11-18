---
title: 집계
description: 여러 정보 번들을 하나의 값으로 통합하는 방법을 살펴볼 수 있습니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 집계

여러 정보 번들을 하나의 값으로 통합하는 방법을 살펴볼 수 있습니다.

## 연습 개요

마지막 연습에서 작성한 &quot;반복 소개&quot; 시나리오를 사용하여 프로젝트의 모든 작업 작업에 대한 계획 시간을 집계하고 해당 정보를 이메일로 사용자에게 보냅니다.

![집계 이미지 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## 수행할 단계

**필터와 SUM을 계획된 시간에 추가합니다.**

1. 이전 연습에서 만든 &quot;반복 소개&quot; 시나리오를 복제하고 이름을 &quot;Aggregation 소개&quot;로 지정합니다.
1. 프로젝트 읽기 작업 모듈과 작업 수 계산 모듈 사이에 필터를 추가합니다. 필터 이름을 &quot;작업 작업만&quot;으로 지정합니다.
1. 조건을 1차 하위 구성요소 수로 설정 [숫자 연산자: 같음] 0.

   ![집계 이미지 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Random Math 모듈 후에 숫자 누적 도구 모듈을 추가합니다.
1. 소스 모듈을 프로젝트 작업 읽기로 설정합니다.
1. 합계 함수를 SUM으로 설정합니다.
1. 프로젝트 읽기 작업 모듈에서 작업 필드로 값을 설정합니다.
1. 이 모듈 이름을 &quot;모든 작업 계획 시간의 SUM&quot;으로 바꿉니다.

   ![집계 이미지 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **집계가 반복을 종료한다는 것을 보여주는 그림자에 주목하십시오.**

   ![집계 이미지 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **시간을 집계하여 이메일을 보냅니다.**

1. 숫자 누적 후에 이메일 앱에서 이메일 모듈 보내기 를 추가합니다.
1. 직접 이메일을 보냅니다.
1. 제목 줄은 &quot;프로젝트 세부 사항&quot;입니다.
1. 컨텐츠 필드에 &quot;라는 프로젝트가 있습니다. [프로젝트 이름] 총 개수의 [결과] 계획된 시간&quot;입니다. &quot;[프로젝트 이름]&quot;&quot;은(는) 레코드 모듈 읽기 및 &quot;[결과]&quot; 는 누적 모듈에서 가져옵니다.

   ![집계 이미지 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. 한 번 저장하고 실행합니다. 받은 편지함에서 전자 메일을 찾습니다.

반복 내에서 개별 번들에 액세스할 수 있습니다. 하지만 반복 외부에서 이메일 모듈 보내기에서 집계된 필드만 액세스할 수 있습니다.
