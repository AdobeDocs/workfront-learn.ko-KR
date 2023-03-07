---
title: 라우터 연습
description: 라우터를 사용하여 Pokemon과 슈퍼 히어로 번들을 올바른 경로로 전달하는 방법에 대해 알아봅니다. [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 라우터 연습

## 개요

라우터를 사용하여 포켓몬과 슈퍼 히어로 번들을 올바른 경로로 전달한 다음 각 문자에 대한 작업을 만듭니다.

![Fusion 시나리오의 이미지](assets/universal-connectors-and-routing-2.png)

## 라우터 연습

Workfront에서는 연습 연습 비디오를 시청한 후 자신의 환경에서 연습을 다시 만들 것을 권장합니다.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12)

## 운동 URL

* Superhero API 웹 사이트: `https://www.superheroapi.com/`
* 연습의 첫 번째 URL: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* 연습용 두 번째 URL: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

자신의 superhero 토큰에 액세스하는 데 문제가 있는 경우 이 공유 토큰(10110256647253588)을 사용할 수 있습니다. 이 공유 토큰이 모든 사람에게 계속 작동하도록 슈퍼 히어로 API에 대해 몇 번 호출하는지 고려하십시오.

>[!TIP]
>
>이 연습을 완료하는 방법에 대한 단계별 지침은 [라우터 연습](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) 연습.


## 매핑 패널에서 항목 검색

매핑 패널 상단에 있는 항목 검색 필드를 사용하면 배열에 중첩된 경우에도 패널에서 필드를 빠르게 찾을 수 있습니다. 검색은 대/소문자를 구분하지 않습니다.

![첫 번째 검색 패널의 이미지](assets/universal-connectors-and-routing-3.png)

![두 번째 검색 패널의 이미지](assets/universal-connectors-and-routing-4.png)

## API 작업을 위한 팁과 요령

지금까지 시나리오에 필요한 정보를 가져오기 위해 추가 인증이 필요하지 않은 매우 간단한 API(Application Programming Interface)로 작업했습니다. 다음은 API 및 범용 커넥터 작업을 탐색하는 데 도움이 되는 몇 가지 팁입니다.

## 1단계: API 유형 결정

Workfront 및 많은 소프트웨어 시스템은 현재 가장 쉽고 가장 표준적인 API 유형인 REST(대표 상태 전송) API를 사용하여 구축됩니다. 그러나 다음과 같은 몇 가지 다른 요소가 있습니다.

* SOAP(Simple Object Access Protocol)(Workfront의 Proof API는 SOAP 기반)
* FTP (File Transfer Protocol)
* SFTP(Secure File Transfer Protocol)
* 자세한 내용을 보려면 관심 있는 API 유형 및 키워드에 대한 웹 검색을 수행합니다.

>[!NOTE]
>
>Salesforce와 같은 더 큰 플랫폼에 연결하는 경우 해당 플랫폼의 다른 영역에서 다른 API를 제공합니다. 연결하려는 서비스에 적합한 것을 찾으십시오.

## 2단계: API에 필요한 인증 유형 결정

API 인증은 Workfront Fusion을 통해 연결을 시도하는 경우와 같이 서비스 액세스를 제어하는 데 사용되는 식별 형식입니다. 시스템에 액세스할 권한이 있음을 다른 시스템에 증명하는 데 도움이 됩니다. OAuth 2는 현재 사용되는 가장 일반적인 인증 유형입니다. API 인증에 대한 인터넷 검색을 통해 자세히 알아보십시오.

인증은 API 작업 중 가장 어려운 측면일 수 있습니다. Workfront Fusion 유니버설 커넥터의 가장 중요한 기능 중 하나는 OAuth 2, API 키 등과 같은 기본 인증과 같은 일반적인 인증 방법을 사용할 때 Workfront Fusion이 인증을 처리할 수 있다는 것입니다. 인증 방법에 적절한 Workfront Fusion 모듈(예: OAuth 2)을 사용하여 연결을 만들면 Workfront Fusion은 시나리오를 실행할 때마다 API 키 및/또는 토큰을 지속적으로 생성합니다.

Experience League에 대한 향상된 인증 개요 문서에서 Workfront이 제공하는 다양한 유형의 인증에 대해 알아봅니다.

## 3단계: API 설명서 를 읽고 필요한 엔드포인트 찾기

API가 다른 시스템과 상호 작용할 때 이 통신의 터치포인트는 엔드포인트로 간주됩니다. 끝점은 API가 요청을 보내는 위치와 리소스가 사는 위치입니다.

범용 커넥터를 사용하여 API와 상호 작용할 때 API가 지원하는 엔드포인트와 각 요청에 필요한 데이터를 이해해야 합니다. API 설명서에는 API의 엔드포인트와 만들기, 읽기, 업데이트 또는 삭제와 같은 일반적인 작업을 수행하는 방법이 설명되어 있습니다. 이러한 호출을 수행하려면 몇 가지 연습이 필요합니다. 특히 API 호출을 처음 수행하거나 새 API로 작업하는 경우에는 더욱 그렇습니다.

Workfront Fusion Universal Connectors에 대해 자세히 알아보고 Experience League 시 필요한 API와 연결하도록 설정하는 방법을 알아봅니다.

## 최종 메모

Experience League에서 사전 설치된 앱 커넥터의 전체 목록을 확인할 수 있습니다. Workfront Fusion 제품 팀에 새 앱 커넥터를 제안하려면 Innovation Lab에 아이디어를 제출하십시오. 이전에 제출하지 않은 경우 Innovation Lab에 대해 자세히 알아보고, 아이디어를 투표하고 1년에 두 번 리더보드 우선 순위에 참여하는 방법에 대해 살펴보십시오. 이미 Innovation Lab에 액세스할 수 있는 경우 로그인하고 아이디어를 제출합니다.

## 당신 차례입니다

>[!NOTE]
>
>연습 연습과 과제는 선택 사항이며 Fusion 교육을 완료하는 데 필요하지 않습니다.

이 연습 연습은 연습에서 배운 내용을 기반으로 하지만 해결 방법은 제공되지 않습니다.

포켓몬 문자에 대한 여러 변수 설정 모듈에서 &quot;Stat (Level)&quot;라는 변수를 만듭니다. Pokemon 통계의 이름을 이 변수에 매핑합니다. 배열 값 기능을 사용하여 각 상태가 아래와 같이 새 줄이 되도록 배열이 표시되는 방식을 변경합니다.

**힌트:** 해당 수준의 포켓몬 통계는 6개뿐입니다.

![통계 이미지](assets/universal-connectors-and-routing-5.png)

**과제:** 배열 수식을 사용하여 쉼표로 구분된 값 문자열이 아닌 다른 행으로 위와 동일한 방법을 표시하는 기능을 가져올 수 있는지 확인하십시오. 아래 스크린샷에 힌트가 있습니다.

![배열 이름의 이미지](assets/universal-connectors-and-routing-6.png)

## 자세히 알아보시겠습니까? 다음 사항을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
