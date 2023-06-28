---
title: 라우팅 패턴
description: 다른 API를 실제로 처리하지 않고도 라우팅 및 대체 경로에 대한 개념을 보강합니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 라우팅 패턴

다른 API를 실제로 처리하지 않고도 라우팅 및 대체 경로에 대한 개념을 보강합니다.

## 연습 개요

변수 설정 모듈을 사용하여 여러 경로를 통해 숫자를 전송하여 라우팅 시 필터 및 폴백이 작동하는 방식을 확인합니다.

![라우팅 패턴 이미지 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 따라야 할 단계

1. 새 시나리오를 만들고 &quot;라우팅 패턴 및 폴백&quot;이라고 합니다.
1. 트리거에 대해 변수 설정 도구 모듈을 추가합니다. 변수 이름에 &quot;내 번호&quot;를 입력하고 변수 수명을 한 주기로 두고 변수 필드를 &quot;75&quot;로 설정합니다.

   ![라우팅 패턴 이미지 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 다른 모듈을 추가하고 라우터 모듈을 선택합니다. 두 패스 모두에 대해 [증가 함수] 도구를 선택하고 각각에 대해 변경하지 않고 [확인]을 클릭합니다.

   + 첫 번째 경로에 대해 필터를 만들고 이름을 &quot;100 미만&quot;으로 지정한 다음 조건을 로 설정합니다. [내 번호] 100 미만.

   + 두 번째 경로에 대해 필터를 만들고 이름을 &quot;1000 미만&quot;으로 지정한 다음 조건을 로 설정합니다. [내 번호] 1000개 미만. 두 모두에 Numeric 연산자를 사용해야 합니다.

   ![라우팅 패턴 이미지 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![라우팅 패턴 이미지 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 실행 을 한 번 클릭하고 번들이 &quot;100개 미만&quot; 경로를 따라 이동하는 것을 확인합니다.
1. 그런 다음 변수 설정 모듈 필드를 950으로 변경하고 다시 실행합니다. 두 번째 길을 따라 가는 걸 봐.
1. 라우터를 클릭하고 경로를 한 개 더 추가합니다. 증가 함수 도구 모듈을 추가합니다. 필터의 경우 &quot;대체 경로&quot; 확인란을 클릭합니다. 대체 경로를 나타내는 화살표가 캐럿으로 어떻게 변경되는지 확인합니다.

   ![라우팅 패턴 이미지 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 변수 번호 설정을 9500으로 변경하고 한 번 실행합니다. 숫자가 100보다 작거나 1000보다 작기 때문에 번들은 대체 경로를 따라 이동합니다.

증가 함수 도구 모듈로 경로를 하나 더 추가했지만 필터를 설정하지 않은 경우 실행을 다시 클릭하면 어떤 일이 발생합니까? 번들이 네 번째 경로가 추가된 대체 경로를 따라 내려가나요?

+ 아니요. 필터가 설정되어 있지 않으면 모든 번들이 대체 경로 대신 항상 이 경로를 통해 전달됩니다.
