---
title: 오류 처리 지시 이해
description: 실행을 계속할 수 있는 오류 처리기 지시문과 실행을 중지하는 지시어에 대해 알아봅니다. [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# 오류 처리 지시 이해

이 비디오에서는 다음을 학습합니다.

* 실행을 계속할 수 있는 세 개의 오류 처리기 지시문입니다
* 실행을 중지하는 두 오류 처리기 지시문

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## 지시 — 시나리오 지속

### 다시 시작

* 대체 출력이 지정되고 오류가 발생하는 모듈에 제공됩니다.
* 후속 모듈이 처리됩니다.
* 시나리오 실행 상태는 &quot;성공&quot;으로 표시됩니다.

![Resume 지시문 이미지](assets/troubleshooting-and-error-handling-2.png)

### 브레이크

* 시나리오 실행 상태는 오류를 수동으로 해결할 수 있는 불완전한 실행 큐에 저장됩니다. 그러나 여기에 언급된 몇 가지 예외가 있습니다.
* 후속 모듈이 처리되지 않습니다.
* 처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속 실행됩니다.
* 시나리오 실행 상태는 &quot;경고&quot;로 표시됩니다.

![Break 지시어의 이미지](assets/troubleshooting-and-error-handling-3.png)

### 무시

* 오류가 무시되고 후속 모듈이 처리되지 않습니다.
* 처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속 실행됩니다.
* 시나리오 실행 상태는 &quot;성공&quot;으로 표시됩니다.

![Ignore 지시문의 이미지](assets/troubleshooting-and-error-handling-4.png)

## 지시어 — 시나리오 정지

### 롤백

* 시나리오 실행이 즉시 중지되고 모든 모듈에서 롤백 단계가 시작되어 초기 상태로 모두 되돌릴 수 있습니다.
* 후속 모듈이 처리되지 않습니다.
* 몇 가지 오류 유형이 없는 경우 시나리오 설정에서 지정된 &quot;연속 오류 수&quot; 후에 시나리오가 비활성화됩니다.
* 시나리오 실행 상태는 &quot;error&quot;로 표시됩니다.

>[!NOTE]
>
>모듈에 연결된 오류 처리기 경로가 없고 시나리오 설정의 &quot;완료되지 않은 실행 저장 허용&quot; 설정이 선택되어 있지 않은 경우 이 동작이 기본 동작입니다.

![Rollback 지시문의 이미지](assets/troubleshooting-and-error-handling-5.png)

### 커밋

* 오류가 무시되고 후속 모듈이 처리되지 않습니다.
* 처리되지 않은 번들이 있으면 시나리오 실행이 정상적으로 계속 실행됩니다.
* 시나리오 실행 상태는 &quot;성공&quot;으로 표시됩니다.

![Commit 지시문 이미지](assets/troubleshooting-and-error-handling-6.png)
