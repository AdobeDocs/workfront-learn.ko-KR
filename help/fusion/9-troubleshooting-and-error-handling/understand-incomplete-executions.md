---
title: 불완전한 실행 이해
description: 불완전한 실행의 정의와 에서 불완전한 실행을 가져오는 오류를 처리하는 방법을 알아봅니다. [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
source-git-commit: 96f963bf5a44eac234cbf9215f19f6dddbe23143
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 불완전한 실행 이해

불완전한 실행은 Workfront Fusion에 저장될 수 있으며, 이 경우 나중에 검토 및 해결할 수 있습니다. 이 놀라운 기능을 활용하는 방법을 배웁니다.

이 비디오에서는 다음을 학습합니다.

* 불완전한 실행은
* 불완전한 실행을 일으키는 오류를 처리하는 방법입니다

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12)

## 오류가 발생하여 실행이 완료되지 않았습니다.

불완전한 실행을 저장하는 오류 범주가 몇 가지 있습니다.

받은 다른 오류 유형은 연결 중인 API에 따라 달라집니다. 모듈을 통해 진행되는 모든 데이터를 성공적으로 처리하기 위해 필요한 항목이 누락되어 불완전하거나 잘못된 데이터에서 발생하는 유효성 검사 오류가 오류일 수 있습니다. 또는 일시적인 또는 장기 연결 실패(예: 이메일 또는 원격 FTP 서버에 연결하는 동안)로 인해 최종 대상의 비가용성 상태에서 오류가 발생할 수 있습니다.

시나리오의 첫 번째 모듈에서 오류가 발생하면 실행이 즉시 중지되고 불완전한 실행이 저장되지 않습니다.

다른 모듈에서 오류가 발생하여 연결된 오류 처리기 경로가 없는 경우 다음을 수행합니다.

* 오류 유형이 ConnectionError, RateLimitError, OutOfSpaceError 또는 ModuleTimeoutError인 경우, 자동 재시도가 있는 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError 또는 MaxResultsExceededError인 경우 자동 재시도가 없는 불완전한 실행 레코드가 저장됩니다.
* 오류 유형이 위 이외의 다른 경우 실행이 실패합니다.

## 자세한 내용 다음 사항을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
