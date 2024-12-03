---
title: 오류 처리 지시문 이해
description: ' [!DNL Adobe Workfront Fusion]에서 계속해서 실행할 수 있는 오류 핸들러 지시문과 실행을 정지하는 오류 핸들러 지시문에 대해 알아봅니다.'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 오류 처리 지시문 이해

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* 계속해서 실행할 수 있는 세 가지 오류 핸들러 지시문
* 실행을 중지하는 두 가지 오류 핸들러 지시문

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## 지시문 - 시나리오 계속

### Resume

* 대체 출력이 지정되어 오류가 발생한 모듈에 제공됩니다.
* 후속 모듈이 처리됩니다.
* 시나리오 실행 상태는 “성공”으로 표시됩니다.

![Resume 지시문의 이미지](assets/troubleshooting-and-error-handling-2.png)

### Break

* 시나리오 실행 상태가 오류를 수동으로 해결할 수 있는 불완전한 실행 대기열에 저장됩니다. 그러나 여기에 언급된 바와 같이 몇 가지 예외가 있습니다.
* 후속 모듈이 처리되지 않습니다.
* 처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속됩니다.
* 시나리오 실행 상태는 “경고”로 표시됩니다.

![Break 지시문의 이미지](assets/troubleshooting-and-error-handling-3.png)

### 무시

* 오류가 무시되고 후속 모듈이 처리되지 않습니다.
* 처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속됩니다.
* 시나리오 실행 상태는 “성공”으로 표시됩니다.

![Ignore 지시문의 이미지](assets/troubleshooting-and-error-handling-4.png)

## 지시문 - 시나리오 정지

### Rollback

* 시나리오 실행이 즉시 중지되고, 모든 모듈을 초기 상태로 되돌리기 위해 모든 모듈에서 롤백 단계가 시작됩니다.
* 후속 모듈이 처리되지 않습니다.
* 몇 가지 오류 유형을 제외하고 시나리오 설정에서 지정한 “연속 오류 수” 후에 시나리오가 비활성화됩니다.
* 시나리오 실행 상태는 “오류”로 표시됩니다.

>[!NOTE]
>
>오류 핸들러 경로가 모듈에 연결되어 있지 않고 시나리오 설정 아래에서 “불완전한 실행 저장 허용” 설정이 선택되지 않은 경우 이것이 기본 동작입니다.

![Rollback 지시문의 이미지](assets/troubleshooting-and-error-handling-5.png)

### 커밋

* 오류가 무시되고 후속 모듈이 처리되지 않습니다.
* 처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속됩니다.
* 시나리오 실행 상태는 “성공”으로 표시됩니다.

![Commit 지시문의 이미지](assets/troubleshooting-and-error-handling-6.png)
