---
title: 라우터 연습
description: 라우터를 사용하여 Pokemon과 슈퍼히어로들 번들을 의 올바른 경로로 전달하는 방법을 알아봅니다. [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
source-git-commit: 82b0e8e5875f3cedd25446507b29a46c9d598d29
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 라우터 연습

## 개요

라우터를 사용하여 Pokemon과 슈퍼히어로들 번들을 올바른 경로로 전달한 다음 각 캐릭터에 대한 작업을 만듭니다.

![Fusion 시나리오의 이미지](assets/universal-connectors-and-routing-2.png)

## 라우터 연습

Workfront에서는 자체 환경에서 연습을 다시 시도하기 전에 연습 연습 연습 비디오 를 시청하는 것이 좋습니다.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12)

## 연습 URL

* 슈퍼히어로 API 웹 사이트: https://www.superheroapi.com/
* 연습의 첫 번째 URL: https://www.superheroapi.com/api/{access-token}/{character-id}/appearance
* 연습용 두 번째 URL: https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats

자신의 슈퍼히어로 토큰에 액세스하는 데 문제가 있으면 다음 공유 토큰을 사용할 수 있습니다. 10110256647253588. 이 공유 토큰이 모든 사람에게 계속 작동할 수 있도록 슈퍼 히어로 API를 몇 번 호출하는지 주의하십시오.

>[!TIP]
>
>이 연습을 완료하는 방법에 대한 단계별 지침은 [라우터 연습](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) 운동.


## 매핑 패널에서 항목 검색

매핑 패널 위쪽에 있는 검색 항목 필드를 사용하면 배열에 중첩된 경우에도 패널에서 필드를 빠르게 찾을 수 있습니다. 검색은 대/소문자를 구분하지 않습니다.

![첫 번째 검색 패널의 이미지입니다](assets/universal-connectors-and-routing-3.png)

![두 번째 검색 패널의 이미지입니다](assets/universal-connectors-and-routing-4.png)

## API 작업을 위한 팁과 트릭

지금까지 시나리오에 필요한 정보를 가져오기 위해 추가 인증이 필요하지 않은 매우 간단한 API(Application Programming Interface)로 작업했습니다. 다음은 API 및 Universal Connectors 작업을 탐색하는 데 도움이 되는 몇 가지 팁입니다.

## 1단계: API 유형 확인

Workfront 및 많은 소프트웨어 시스템은 현재 API의 가장 쉽고 표준 유형인 REST(Representative State Transfer) API를 사용하여 구축되었습니다. 그러나 다음과 같은 몇 가지 다른 항목이 있습니다.

* SOAP(Simple Object Access Protocol)(Workfront의 증명 API는 SOAP를 기반으로 함)
* FTP(파일 전송 프로토콜)
* SFTP(Secure File Transfer Protocol)
* 자세한 내용은 API 유형 및 관심사 키워드를 웹 검색하십시오.

>[!NOTE]
>
>Salesforce와 같은 대형 플랫폼에 연결할 때 해당 플랫폼의 다양한 영역에서 다른 API를 제공합니다. 연결하려는 서비스에 적합한 서비스가 있는지 확인하십시오.

## 2단계: API에 필요한 인증 유형 확인

API 인증은 Workfront Fusion을 통해 연결하려고 할 때와 같이 서비스에 대한 액세스를 제어하는 데 사용되는 식별 형식입니다. 시스템에 액세스할 수 있는 권한이 있는 다른 시스템에 대한 인증을 제공하는 데 도움이 됩니다. OAuth 2는 현재 사용되는 가장 일반적인 인증 유형입니다. API 인증에 대한 인터넷 검색을 통해 자세히 알아보십시오.

API 작업의 가장 어려운 측면은 인증일 수 있습니다. Workfront Fusion의 Universal Connectors에서 가장 중요한 기능 중 하나는 Workfront Fusion이 기본 인증(예: OAuth 2, API 키 등)과 같은 일반적인 인증 방법을 사용할 때 인증을 처리할 수 있다는 것입니다. 인증 방법(예: OAuth 2)에 적합한 Workfront Fusion 모듈을 사용하여 연결을 만들면 Workfront Fusion은 시나리오를 실행할 때마다 계속 API 키 및/또는 토큰을 생성합니다.

Experience League의 고급 인증 개요 문서에서 Workfront이 제공하는 다양한 유형의 인증에 대해 알아보십시오.

## 3단계: API 설명서를 읽고 필요한 엔드포인트를 찾습니다

API가 다른 시스템과 상호 작용할 때 이 커뮤니케이션의 터치포인트는 종단점으로 간주됩니다. 종단점은 API가 요청을 보내고 리소스가 상주하는 위치입니다.

범용 커넥터를 사용하여 API와 상호 작용할 때 API가 지원하는 엔드포인트와 각 요청에 필요한 데이터를 이해해야 합니다. API 설명서는 API의 종단점과 만들기, 읽기, 업데이트 또는 삭제와 같은 일반적인 작업을 수행하는 방법을 설명해야 합니다. 이러한 호출을 수행하는 데는 특히 API 호출을 처음 사용하는 경우나 새 API 작업을 수행하는 경우에 몇 가지 방법이 필요합니다.

Workfront Fusion Universal Connectors에 대해 자세히 알아보고 Experience League 시 필요한 API와 연결하도록 설정하는 방법을 알아봅니다.

## 최종 참고 사항

Experience League에서 사전 빌드된 앱 커넥터의 전체 목록을 확인할 수 있습니다. Workfront Fusion 제품 팀에 새로운 앱 커넥터를 제안하려면 Innovation Lab에 아이디어를 제출하십시오. 아직 제출하지 않았다면 Innovation Lab에 대해 자세히 알아보고 아이디어를 투표할 수 있으며 1년에 2회 리더보드 우선 순위에 참여할 수 있습니다. 이미 Innovation Lab에 액세스할 수 있는 경우에는 로그인한 다음 아이디어를 제출하십시오.

## 네 차례야

이 연습 연습은 연습에서 학습한 내용을 기반으로 만들어지지만 솔루션은 제공되지 않습니다.

Pokemon 문자의 여러 변수 설정 모듈에서 &quot;시작(레벨)&quot;이라는 변수를 만듭니다. Pokemon Stats의 이름을 이 변수에 매핑합니다. 배열 값 기능을 사용하여 배열의 표시 방식을 변경할 수 있습니다. 이렇게 하면 각 통계가 아래와 같이 새 라인으로 표시됩니다.

**힌트:** 해당 수준을 갖는 6개의 다른 Pokemon 통계만 있습니다.

![통계 이미지](assets/universal-connectors-and-routing-5.png)

**과제:** 배열 수식을 사용하여 쉼표로 구분된 값 문자열이 아닌 다른 행과 동일한 방식으로 표시할 수 있는 기능을 얻을 수 있는지 확인하십시오. 아래 스크린샷에는 힌트가 있습니다.

![배열 이름의 이미지입니다.](assets/universal-connectors-and-routing-6.png)

## 자세한 내용 다음 사항을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
