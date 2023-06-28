---
title: 집계
description: 여러 정보 번들을 하나의 값으로 집계하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 집계

여러 정보 번들을 하나의 값으로 집계하는 방법을 알아봅니다.

## 연습 개요

지난 연습에서 빌드한 &quot;반복 소개&quot; 시나리오를 사용하여 프로젝트의 모든 작업 시 계획된 시간을 집계한 다음 해당 정보가 포함된 전자 메일을 본인에게 보냅니다.

![집계 이미지 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## 따라야 할 단계

**필터를 추가하고 계획된 시간을 합산합니다.**

1. 이전 연습에서 만든 &quot;반복 소개&quot; 시나리오를 복제하고 이름을 &quot;집계 소개&quot;로 지정합니다.
1. 프로젝트의 작업 읽기 모듈과 작업 수 카운트 모듈 사이에 필터를 추가합니다. 필터 이름을 &quot;작업 중인 작업만&quot;으로 지정합니다.
1. 조건을 하위 항목 수로 설정 [숫자 연산자: 같음] 0.

   ![집계 이미지 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. 임의 계산 모듈 뒤에 숫자 집계 도구 모듈을 추가합니다.
1. 프로젝트의 작업을 읽도록 소스 모듈을 설정합니다.
1. Aggregate 함수를 SUM으로 설정합니다.
1. 프로젝트의 작업 읽기 모듈에서 값을 작업 필드로 설정합니다.
1. 이 모듈의 이름을 &quot;모든 작업 계획 시간의 합계&quot;로 바꿉니다.

   ![집계 이미지 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **합계가 이터레이션을 끝냄을 보여 주는 그림자를 확인합니다.**

   ![집계 이미지 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **집계된 시간으로 이메일을 전송합니다.**

1. 숫자 집계 다음에 이메일 앱에서 이메일 보내기 모듈을 추가합니다.
1. 본인에게 이메일을 보내십시오.
1. 제목 줄은 &quot;프로젝트 세부 정보&quot;입니다.
1. 콘텐츠 필드에 &quot;There is a project called. [프로젝트 이름] 의 총 수는 [결과] 계획된 시간.&quot; &quot;[프로젝트 이름]&quot;는 레코드 읽기 모듈 및&quot;에서 가져옵니다.[결과]&quot;는 집계 모듈에서 가져옵니다.

   ![집계 이미지 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. 한 번 저장 및 실행. 받은 편지함에서 이메일을 찾습니다.

반복 내에서 개별 번들에 액세스할 수 있습니다. 그러나 반복 외부에서 이메일 전송 모듈에서는 집계된 필드에만 액세스할 수 있습니다.
