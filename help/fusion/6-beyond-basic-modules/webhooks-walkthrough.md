---
title: Webhooks 연습
description: 웹후크를 사용하여 앱을 만들어 고객이 알코올을 구매할 수 있을 정도의 나이인지 여부를 판별하는 방법에 대해 알아봅니다. [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Webhooks 연습

## 개요

이 시나리오는 편의점 앱을 만들어 고객이 술을 구매할 만큼 나이가 들었는지 여부를 쉽게 판단할 수 있도록 한다. 계산원은 고객의 이름과 생년월일, 그리고 확인된 클라이언트 토큰을 제공된 URL에 게시하기만 하면 됩니다. 그러면 시나리오가 트리거되어 적절한 응답을 계산하고 요청자에게 반환됩니다.

![스위치 모듈을 사용하는 이미지](assets/beyond-basic-modules-5.png)

## Webhooks 연습

Workfront에서는 연습 연습 비디오를 시청한 후 자신의 환경에서 연습을 다시 만들 것을 권장합니다.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>이 연습을 완료하는 방법에 대한 단계별 지침은 [Webhooks 연습](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) 연습.

## Postman 설정

연습 연습을 따라 무료 Postman 애플리케이션을 다운로드해야 합니다. 연습을 위해 아래 단계에 따라 Postman의 오른쪽 영역으로 이동합니다.

1. 작업 영역을 만든 다음 엽니다.
1. New 탭을 클릭하고 Drinking Age 라는 새 컬렉션을 만듭니다.
1. 새 탭을 다시 클릭하고 GET 생년월일이라는 새 GET 요청을 만듭니다.
1. 요청 작업을 GET에서 POST으로 변경합니다.
1. POST URL 필드 아래의 본문 하위 탭 영역으로 이동합니다.
1. 인증 하위 탭 아래에서 양식 데이터를 선택합니다.
1. Name, Birthdate 및 clientToken에 대한 세 개의 키를 만듭니다.

![스위치 모듈을 사용하는 이미지](assets/beyond-basic-modules-6.png)

## 당신 차례입니다

>[!NOTE]
>
>연습 연습과 과제는 선택 사항이며 Fusion 교육을 완료하는 데 필요하지 않습니다.

이 연습 연습은 연습에서 배운 내용을 기반으로 하지만 해결 방법은 제공되지 않습니다.

새 업데이트가 생성될 때까지 대기하는 Workfront 웹후크를 만든 다음 날짜, 업데이트를 수행한 사용자의 이름 및 업데이트에 포함된 내용을 기록합니다. 이 정보를 이메일로 직접 보내십시오.

**힌트**: Workfront Watch 이벤트 트리거 모듈을 사용하여 웹후크를 만듭니다. 또한 Workfront 업데이트에서는 메모를 라고 합니다.

**과제**: 쉽게 액세스할 수 있도록 업데이트가 수행된 위치의 URL을 찾아 추가할 수 있습니까?


## 자세히 알아보시겠습니까? 다음 사항을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
