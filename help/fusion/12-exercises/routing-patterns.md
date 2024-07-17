---
title: 라우팅 패턴 연습
description: 다른 API를 실제로 다루지 않고 라우팅 및 대체 경로의 개념을 강화합니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,noCatalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 100%

---

# 라우팅 패턴 연습

다른 API를 실제로 다루지 않고 라우팅 및 대체 경로의 개념을 강화합니다.

## 연습 개요

변수 설정 모듈을 사용하여 여러 경로를 통해 번호를 보내 라우팅할 때 필터 및 대체가 어떻게 작동하는지 확인합니다.

![라우팅 패턴 이미지 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 따라야 할 단계

1. 새 시나리오를 만들고 “라우팅 패턴 및 대체”라고 합니다.
1. 트리거에 대해 변수 설정 도구 모듈을 추가합니다. 변수 이름에 “내 번호”를 입력하고, 변수 수명을 한 주기로 두고 변수 필드는 “75”로 설정합니다.

   ![라우팅 패턴 이미지 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 다른 모듈을 추가하고 라우터 모듈을 선택합니다. 두 경로에 대해 증분 함수 도구를 선택한 다음 변경하지 않고 확인을 클릭합니다.

   + 첫 번째 경로에 대해 필터를 만들고 이름을 “100 미만”으로 지정한 다음, 조건을 [내 번호] 100 미만으로 설정합니다.

   + 두 번째 경로에 대해 필터를 만들고 이름을 “1,000 미만”으로 지정한 다음, 조건을 [내 번호] 1,000 미만으로 설정합니다. 둘 다에 대해 숫자 연산자를 사용하도록 합니다.

   ![라우팅 패턴 이미지 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![라우팅 패턴 이미지 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 한 번 실행을 클릭하고 번들이 “100 미만” 경로 아래로 전달되는 것을 확인합니다.
1. 그런 다음 변수 설정 모듈 필드를 950으로 변경하고 다시 한 번 실행을 클릭합니다. 두 번째 경로 아래로 전달되는 것을 확인합니다.
1. 라우터를 클릭하고 경로를 하나 더 추가합니다. 증분 함수 도구 모듈을 추가합니다. 필터에 대해 “대체 경로” 확인란을 클릭합니다. 해당 경로를 가리키는 화살표가 대체 경로임을 나타내는 삽입 기호로 변경되는 방법을 확인합니다.

   ![라우팅 패턴 이미지 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 변수 번호 설정을 9,500으로 변경하고 한 번 실행을 클릭합니다. 숫자가 100 이상 또는 1,000 미만이므로 번들은 대체 경로를 따라 이동합니다.

증분 함수 도구 모듈로 경로를 하나 더 추가하고 필터를 설정하지 않은 경우, 다시 한 번 실행을 클릭하면 어떻게 됩니까? 번들은 네 번째 경로가 추가된 대체 경로로 이동합니까?

+ 아니요. 필터를 설정하지 않으면 모든 번들이 항상 대체 경로 대신 이 경로를 따라 이동합니다.
