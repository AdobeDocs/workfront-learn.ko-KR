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
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:51.152Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 93%

---

# 불완전한 실행 이해

불완전한 실행은 나중에 검토하고 해결할 수 있는 Workfront Fusion에 저장할 수 있습니다. 이러한 놀라운 기능을 활용하는 방법을 알아봅니다.

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 불완전한 실행 정의
* 불완전한 실행을 초래하는 오류를 처리하는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## 불완전한 실행으로 인한 오류

불완전한 실행을 저장하는 오류에는 몇 가지 카테고리가 있습니다.

수신되는 다른 오류 유형은 연결하려는 API에 따라 다릅니다. 오류는 대부분 모듈을 통과하는 모든 데이터를 성공적으로 처리하기 위해 예상되는 누락된 항목으로 인해 불완전하거나 잘못된 데이터에서 발생하는 유효성 검사 오류일 수 있습니다. 또는 일시적 또는 장기적인 연결 실패(예: 이메일 또는 원격 FTP 서버 연결 중)로 인해 최종 대상이 사용할 수 없는 오류가 발생할 수 있습니다.

시나리오의 첫 번째 모듈에서 오류가 발생하면 실행이 즉시 중지되고 불완전한 실행은 저장되지 않습니다.

다른 모듈에서 오류가 발생하고 연결된 오류 핸들러 경로가 없는 경우:

* 오류 유형이 ConnectionError, RateLimitError, OutOfSpaceError 또는 ModuleTimeoutError인 경우, 자동 재시도가 있는 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError 또는 MaxResultsExceededError인 경우, 자동 재시도 없이 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 위와 다른 경우 실행이 실패합니다.

## 자세히 알아보고자 하십니까? 다음 자료를 참조하십시오.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
