---
title: Webhooks 연습
description: 웹 후크를 사용하여 앱을 만들어 고객이 알코올 구입하기에 충분한지 여부를 확인하는 방법을 알아봅니다. [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Webhooks 연습

## 개요

이 시나리오는 고객이 술을 구입할 만큼 나이가 들었는지 여부를 쉽게 결정할 수 있도록 편의점 앱을 만듭니다. 계산원은 제공된 URL에 고객의 이름과 생년월일 및 검증된 클라이언트 토큰을 게시하면 됩니다. 입력한 후 해당 응답을 계산하여 요청자에게 반환하기 위해 시나리오를 트리거합니다.

![스위치 모듈을 사용한 이미지](assets/beyond-basic-modules-5.png)

## Webhooks 연습

Workfront에서는 자체 환경에서 연습을 다시 시도하기 전에 연습 연습 연습 비디오 를 시청하는 것이 좋습니다.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>이 연습을 완료하는 방법에 대한 단계별 지침은 [Webhooks 연습](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) 운동.

## Postman 설정

연습 연습과 함께 따라 무료 Postman 애플리케이션을 다운로드해야 합니다. 아래 절차에 따라 연습을 위해 Postman의 올바른 영역으로 이동합니다.

1. 작업 공간을 만든 다음 엽니다.
1. 새 탭을 클릭하고 새 컬렉션 이름을 &quot;음주 연령&quot;으로 지정합니다.
1. 새로 만들기 탭을 다시 클릭하고 GET 생일인 새 GET 요청을 만듭니다.
1. 요청 작업을 GET에서 POST으로 변경합니다.
1. POST URL 필드 아래의 본문 하위 탭 영역으로 이동합니다.
1. 권한 부여 하위 탭 아래에서 양식 데이터를 선택합니다.
1. 이름, 생년월일 및 clientToken에 대해 세 개의 키를 만듭니다.

![스위치 모듈을 사용한 이미지](assets/beyond-basic-modules-6.png)

## 네 차례야

이 연습 연습은 연습에서 학습한 내용을 기반으로 만들어지지만 솔루션은 제공되지 않습니다.

새로운 업데이트를 기다리고 있는 Workfront 웹 후크를 만든 다음 날짜, 업데이트를 만든 사람의 이름 및 업데이트에 표시되는 내용을 기록합니다. 이 정보를 자신에게 이메일로 보냅니다.

**힌트**: Workfront 감시 이벤트 트리거 모듈을 사용하여 웹 후크를 만듭니다. 또한 Workfront 업데이트에서는 메모라고 합니다.

**과제**: 쉽게 액세스할 수 있도록 업데이트가 수행된 URL을 찾아 추가할 수 있습니까?


## 자세한 내용 다음 사항을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
