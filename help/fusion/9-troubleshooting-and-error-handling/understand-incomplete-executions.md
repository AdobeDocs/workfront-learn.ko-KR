---
title: 불완전한 실행 이해
description: ' [!DNL Adobe Workfront Fusion]에서 불완전한 실행의 정의 및 불완전한 실행을 초래하는 오류를 처리하는 방법에 대해 알아봅니다.'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,noCatalog
doc-type: video
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 100%

---

# 불완전한 실행 이해

불완전한 실행은 나중에 검토하고 해결할 수 있는 Workfront Fusion에 저장할 수 있습니다. 이러한 놀라운 기능을 활용하는 방법을 알아봅니다.

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 불완전한 실행 정의
* 불완전한 실행을 초래하는 오류를 처리하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on)

## 불완전한 실행으로 인한 오류

불완전한 실행을 저장하는 오류에는 몇 가지 카테고리가 있습니다.

수신되는 다른 오류 유형은 연결하려는 API에 따라 다릅니다. 오류는 대부분 모듈을 통과하는 모든 데이터를 성공적으로 처리하기 위해 예상되는 누락된 항목으로 인해 불완전하거나 잘못된 데이터에서 발생하는 유효성 검사 오류일 수 있습니다. 또는 일시적 또는 장기적인 연결 실패(예: 이메일 또는 원격 FTP 서버 연결 중)로 인해 최종 대상이 사용할 수 없는 오류가 발생할 수 있습니다.

시나리오의 첫 번째 모듈에서 오류가 발생하면 실행이 즉시 중지되고 불완전한 실행은 저장되지 않습니다.

다른 모듈에서 오류가 발생하고 연결된 오류 핸들러 경로가 없는 경우:

* 오류 유형이 ConnectionError, RateLimitError, OutOfSpaceError 또는 ModuleTimeoutError인 경우, 자동 재시도가 있는 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError 또는 MaxResultsExceededError인 경우, 자동 재시도 없이 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 위와 다른 경우 실행이 실패합니다.

## 자세히 알아보고 싶으신가요? 다음 자료를 참조하십시오.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=ko-KR)
