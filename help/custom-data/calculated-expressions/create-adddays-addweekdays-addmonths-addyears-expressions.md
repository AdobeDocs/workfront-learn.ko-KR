---
title: ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS 표현식 만들기
description: Adobe의 계산된 필드에서 ADD 표현식을 사용하고 만드는 방법을 알아봅니다 [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS 표현식 만들기

이 비디오에서는 다음 사항에 대해 알아봅니다.

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 표현식에서 계산하는 내용
* 계산된 필드에서 ADDWEEKDAYS 데이터 표현식을 만드는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## 추가 예

다음은 Adobe Workfront 고객이 만든 몇 가지 추가 ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 표현식입니다.

**다음을 수행해야 합니다.**

고객은 실제 시작 일자 및 계획된 기간을 기반으로 작업을 완료해야 하는 시기를 알고자 했습니다. 작업이 늦어지면 계획된 완료 일자가 이동할 수 있으므로 이 경우 예상 완료 일자가 작동하지 않으며, 이전 작업이 지연되는 경우 계획된 완료 일자가 도움이 되지 않습니다.

생성된 표현식은 ADDDAYS({actualStartDate},{durationMinutes}/480)

기간 필드의 시간은 분 단위로 저장됩니다. 따라서 이 표현식에서는 시간을 일 단위로 반영해야 하는 경우 기간 필드를 단독으로 사용할 수 없습니다. 이를 위해서는 지속 시간을 480분 (480분 = 8시간 = 1일)으로 나누어야 합니다

이 때문에 두 번째 값 슬롯에는 (Duration/480)이 포함됩니다.


**송장 완료 일자**

이 예에는 ADDDAYS 표현식뿐만 아니라 사용자 정의 양식에서 이전에 만들어 저장한 사용자 정의 필드가 포함됩니다.

고객이 &quot;송장 제출 일자&quot;라는 사용자 정의 일자 필드를 통해 송장이 제출된 일자를 캡처하고 있습니다.

제출 후 30일 이내에 송장을 작성하여 제출해야 합니다. 해당 완료 및 제출 날짜를 자동으로 생성하기 위해 ADDDAYS 계산된 필드가 &quot;송장 제출 날짜&quot; 사용자 정의 필드와 함께 사용됩니다. 표현식은 다음과 같습니다.

ADDDAYS({DE:Invoice Submission Date},30)
