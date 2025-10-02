---
title: ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS 표현식 만들기
description: Adobe [!DNL Workfront]의 계산된 필드에서 ADD 표현식을 사용하고 만드는 방법을 알아봅니다.
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
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 97%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS 표현식 만들기

이 비디오를 통해 다음과 같은 사항을 알아볼 수 있습니다.

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 표현식이 계산하는 것
* 계산된 필드에서 ADDWEEKDAYS 데이터 표현식을 만드는 방법

>[!VIDEO](https://video.tv.adobe.com/v/3416192/?quality=12&learn=on&enablevpops=1&captions=kor)

## 추가 예시

다음은 Adobe Workfront 고객이 만든 몇 가지 추가 ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 표현식입니다.

**완료 필요 기한**

고객은 실제 시작 일자와 계획된 기간을 기준으로 작업이 완료되어야 하는 시점을 확인하고자 했습니다. 이 경우 작업이 늦어지면 일자가 이동할 수 있기 때문에 ‘예상 완료 일자’와는 조금 다르며, 이전 작업이 지연되면 ‘계획된 완료 일자’도 도움이 되지 않습니다.

만들어진 식은 ADDDAYS({actualStartDate},{durationMinutes}/480)입니다.

‘기간’ 필드의 시간은 분 단위로 저장됩니다. 따라서 이 표현식에서 시간이 일 단위로 반영되는 경우 ‘기간’ 필드는 독립적일 수 없습니다. 시간을 일 단위로 반영하려면 기간을 480분으로 나누어야 합니다(480분 = 8시간 = 1일).

이것이 두 번째 값 슬롯에 (기간/480)이 포함되는 이유입니다.


**인보이스 완료 일자**

이 예시에서는 ADDDAYS 표현식을 사용할 뿐만 아니라 이전에 사용자 정의 양식에서 만들고 저장한 사용자 정의 필드가 포함됩니다.

고객은 “인보이스 제출 일자”라는 사용자 정의 일자 필드를 통해 인보이스가 제출된 일자를 캡처합니다.

인보이스는 제출된 지 30일 이내에 작성 및 등록해야 합니다. 해당 완료 및 제출 일자를 자동으로 생성하기 위해 “인보이스 제출 일자” 사용자 정의 필드와 함께 ADDDAYS 계산 필드가 사용됩니다. 표현식은 다음과 같습니다.

ADDDAYS({DE:Invoice Submission Date},30)
