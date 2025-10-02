---
title: 웹후크 워크스루
description: ' [!DNL Adobe Workfront Fusion]에서 웹 후크를 사용하여 고객이 주류를 구매할 수 있는 연령인지 판단하는 앱을 만드는 방법을 알아봅니다.'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 99%

---

# 웹후크 워크스루

이 시나리오는 고객이 주류를 구매할 수 있는 나이인지 여부를 쉽게 확인할 수 있도록 스토어 앱을 만듭니다. 계산원은 제공된 URL에 고객의 이름과 생년월일 및 확인된 클라이언트 토큰을 게시하기만 하면 됩니다. 입력한 후에 시나리오가 트리거되어 적절한 응답을 계산하고 이를 요청자에게 반환합니다.

![전환 모듈을 사용하는 이미지](assets/beyond-basic-modules-5.png)

## 웹후크 워크스루

Workfront에서는 연습 워크스루 비디오를 시청한 다음, 사용자 개인의 환경에서 연습 내용을 재현할 것을 권장합니다.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on&enablevpops=1)


## Postman 설정

워크스루 연습을 따라가려면 무료 Postman 애플리케이션을 다운로드해야 합니다. 아래 단계에 따라 연습을 위해 Postman의 올바른 영역으로 이동합니다.

1. 작업 영역을 만든 다음 엽니다.
1. 새로 만들기 탭을 클릭하고 음주 연령이라는 새 컬렉션을 만듭니다.
1. 새로 만들기 탭을 다시 클릭하고 GET 생년월일이라는 새 GET 요청을 만듭니다.
1. 요청 작업을 GET에서 POST로 변경합니다.
1. POST URL 필드 아래의 본문 하위 탭 영역으로 이동합니다.
1. 인증 하위 탭 아래에서 양식 데이터를 선택합니다.
1. Name, Birthdate 및 clientToken에 대한 세 개의 키를 만듭니다.

![전환 모듈을 사용하는 이미지](assets/beyond-basic-modules-6.png)

## 사용자 차례

>[!NOTE]
>
>실습 및 과제는 옵션이며 Fusion 교육을 완료하는 데 필수는 아닙니다.

이 실습은 워크스루에서 배운 내용을 기반으로 하나, 해결 방법은 제공되지 않습니다.

생성된 새 업데이트를 기다리는 Workfront 웹 후크를 만든 다음 일자, 업데이트한 사람의 이름 및 업데이트 내용을 기록합니다. 이 정보를 자신에게 이메일로 보냅니다.

**힌트**: Workfront 이벤트 보기 트리거 모듈을 사용하여 웹 후크를 만듭니다. 또한 Workfront에서는 업데이트를 메모라고 합니다.

**과제**: 쉽게 접근할 수 있도록 업데이트가 이루어진 URL을 찾아 추가할 수 있습니까?


## 자세히 알아보고 싶으신가요? 다음 자료를 참조하십시오.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
