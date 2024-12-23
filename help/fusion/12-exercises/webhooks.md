---
title: 웹 후크 연습
description: 웹 후크 시작 시나리오를 생성, 트리거 및 관리하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
recommendations: noDisplay,catalog
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '0'
ht-degree: 100%

---

# 웹 후크 연습

웹 후크 시작 시나리오를 생성, 트리거 및 관리하는 방법을 알아봅니다.

## 연습 개요

이 시나리오의 목적은 고객이 주류를 구매할 수 있는 나이인지 여부를 쉽게 확인할 수 있도록 편의점에 판매할 앱을 만드는 것입니다. 계산원은 제공된 URL에 고객의 이름과 생년월일을 게시하기만 하면 됩니다. 해당 게시물은 답변을 계산하고 요청자에게 반환하는 시나리오를 트리거합니다.

1. 시나리오는 세 개의 웹 후크로 구성됩니다.
1. 트리거 모듈은 게시물을 수신 대기하는 사용자 정의 웹 후크입니다.
1. 게시물을 받으면 다음 모듈 중 하나로 출력합니다.
1. 다음 모듈은 요청자에게 응답을 반환합니다.

   ![웹 후크 이미지 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## 따라야 할 단계

**트리거 웹 후크를 설정합니다.**

1. 새 시나리오를 만들고 이름을 “웹 후크 사용”으로 지정합니다.
1. 트리거의 경우, 웹 후크 앱에서 사용자 정의 웹 후크 모듈을 추가합니다.
1. 추가를 클릭하여 새 웹 후크를 만듭니다.
1. “음주 연령 앱”이라는 웹 후크 이름을 입력합니다.
1. IP 제한을 비워 두면 누구나 데이터를 보낼 수 있습니다.
1. 저장을 클릭합니다.


   ![웹 후크 이미지 2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. 웹 후크 매핑 패널에서 특정 웹 후크에 대한 URL이 생성되었습니다. “클립보드에 주소 복사”를 클릭하여 해당 URL을 복사합니다.
1. 확인을 클릭합니다.
1. 한 번 실행을 클릭합니다.
1. Postman의 URL을 사용하여 사용자 정의 웹 후크에 이름 및 생년월일을 보냅니다. Postman 설정에 대한 지침은 [웹 후크 워크스루](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=ko-KR) 튜토리얼을 참조하십시오.

   **웹 후크 모듈 패널은 다음과 같아야 합니다.**

   ![웹 후크 이미지 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **이제 웹 후크 상태는 데이터 구조를 확인하기 위해 데이터를 수신 대기합니다.**

1. 가져올 것으로 예상되는 페이로드의 데이터 구조를 정의할 수 있습니다(데이터 구조는 나중에 설명함). 데이터 구조를 정의하지 않으면 Fusion은 게시물이 전송될 때 자동으로 데이터 구조를 결정합니다.
1. Postman 쪽에서 복사한 URL로 보내려고 합니다. 게시물에는 기본 양식 데이터가 포함되어야 합니다. 이 예에서는 Name, Birthdate 및 clientToken의 세 가지 필드가 필요합니다.

   ![웹 후크 이미지 4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Postman에서 보내기를 클릭하면 게시물이 수락되었다는 표시가 나타납니다.
1. 이는 데이터 구조가 성공적으로 확인되었음을 시나리오에 표시하는 포인트입니다.
1. 실행 검사기를 열면 데이터가 수신되었음을 알 수 있습니다.

   ![웹 후크 이미지 5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **클라이언트 토큰에 대한 라우팅을 설정합니다.**

1. 트리거 모듈에 라우터를 추가합니다.
1. 상위 경로에 웹 후크 응답 모듈을 추가합니다. 클라이언트 토큰이 일치하지 않을 때의 경로입니다.
1. 상태를 401로 설정합니다.
1. 본문을 {“오류”: “요청을 인증하지 못했습니다. clientToken을 확인하십시오.”}로 설정합니다.

   ![웹 후크 이미지 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. 라우터와 웹 후크 응답 모듈 사이에 필터를 만듭니다. 이름을 “클라이언트 토큰이 일치하지 않음”이라고 지정합니다.
1. 조건의 경우, 트리거 모듈의 clientToken 필드를 사용하여 숫자 5121933과 숫자 “같지 않음”을 비교합니다.

   ![웹 후크 이미지 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. 하단 경로에서 다른 Webhook 응답 모듈을 추가합니다. 클라이언트 토큰이 일치할 때의 경로입니다.
1. 상태를 200으로 설정합니다.
1. 본문을 설정할 때 매핑 패널 기능을 사용하여 연령이 21세 이상인지 테스트합니다. 21세 이상이면 “음주가 가능합니다!”를 반환하고 그렇지 않으면 “죄송하지만...”을 반환합니다.

   ![웹 후크 이미지 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. 라우터와 하위 경로에 있는 웹 후크 응답 모듈 사이에 필터를 만듭니다. 이름을 “클라이언트 토큰이 일치함”이라고 지정합니다.
1. 조건의 경우, 트리거 모듈의 clientToken 필드를 사용하여 숫자 5121933과 숫자 “같음”을 비교합니다.


   ![웹 후크 이미지 8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. 한 번 실행 아래의 예약 버튼을 클릭하여 시나리오를 활성화하면 새 게시물이 있을 때마다 수신되고 두 경로 중 하나로 이동하여 응답을 생성할 수 있습니다.
