---
title: ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS 표현식 만들기
description: Adobe의 계산된 필드에서 ADD 표현식을 사용하고 만드는 방법을 알아봅니다 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
source-git-commit: 9cc845d6efe2ee27e66ad7de4e1800cb9077aebd
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS 표현식 만들기

이 비디오에서는 다음을 학습합니다.

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 표현식에서 계산하는 항목
* 계산된 필드에서 ADDWEEKDAY 데이터 표현식을 만드는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## 추가 예

다음은 Adobe Workfront 고객이 만든 몇 가지 추가 ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 표현입니다.

**다음에서 했어야 했는데**

고객은 실제 시작 날짜와 계획 기간을 기준으로 작업이 완료되어야 하는 시기를 알고 싶어했습니다. 작업이 늦을 경우 이동할 수 있고 이전 작업에 지연이 있을 경우 계획 완료 날짜가 도움이 되지 않으므로 이 경우 예상 완료 날짜가 작동하지 않습니다.

만든 식은 ADDDAYS({actualStartDate},{durationMinutes}/480)입니다.

기간 필드의 시간은 분 단위로 저장됩니다. 따라서 이 표현식에서 시간을 일 단위로 반영하는 경우 기간 필드를 단독으로 사용할 수 없습니다. 이렇게 하려면 기간을 480분(480분 = 8시간 = 1일)으로 나누어야 합니다

이 때문에 두 번째 값 슬롯에 (Duration/480)가 포함됩니다.


**송장 완료 일자**

이 예에는 ADDDAYS 표현식뿐만 아니라 사용자 지정 양식에 미리 만들어 저장된 사용자 지정 필드도 포함됩니다.

고객은 &quot;송장 실행 일자&quot;라는 사용자 지정 일자 필드를 통해 송장이 실행된 일자를 캡처하고 있습니다.

제출되면 30일 이내에 송장을 완료하고 제출해야 합니다. 해당 완료 및 등록 일자를 자동으로 생성하기 위해 &quot;송장 제출 일자&quot; 사용자 정의 필드와 함께 ADDDAYS 계산 필드가 사용됩니다. 표현식은 다음과 같습니다.

ADDDAYS({DE:Invoice Submission Date},30)
