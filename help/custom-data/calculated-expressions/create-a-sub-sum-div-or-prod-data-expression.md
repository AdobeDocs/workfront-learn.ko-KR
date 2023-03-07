---
title: SUB, SUM, DIV 또는 PROD 데이터 표현식 작성
description: Adobe의 계산된 필드에서 기본 수학 표현식을 사용하고 만드는 방법을 알아봅니다 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
kt: 8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# SUB, SUM, DIV 또는 PROD 데이터 표현식 작성

이 비디오에서는 다음 사항에 대해 알아봅니다.

* SUB, SUM, DIV 및 PROD 표현식의 기능
* 계산된 필드에서 SUB 데이터 표현식을 만드는 방법

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12)

## 추가 정보: ROUND 표현식

### ROUND 표현식 만들기

ROUND 표현식은 임의의 숫자를 사용하여 특정 소수 자릿수로 반올림합니다.

대부분의 경우 ROUND 데이터 표현식은 다른 데이터 표현식과 함께 사용되며 형식 필드를 텍스트 또는 숫자로 남겨둡니다.

다음과 같이 SUB 표현식이 필요하고 표시되는 작업에 계획된 시간과 실제로 로그온한 시간 간의 차이를 결정하기 위해 계산된 필드를 생성해 보겠습니다.

**SUB({workRequired},{actualWorkRequired})**

그리고 시간은 분 단위로 추적되고 기본 형식은 정보를 시간 단위로 표시하는 것이므로 표현식도 다음과 같이 60으로 나누어야 합니다.

**DIV(SUB({workRequired},{actualWorkRequired}),60)**

사용자 정의 양식에서 계산된 필드를 작성할 때 형식이 숫자로 변경되면 보기에서 필드를 추가할 때 숫자 형식을 변경할 수 있습니다.

![사용률 보고서를 포함한 업무 균형자](assets/round01.png)

하지만 사용자 정의 필드를 만들 때 필드 형식을 텍스트로 남겨두면 보기 내에서 형식을 쉽게 변경할 수 없습니다. 프로젝트에서 다음과 같은 숫자가 표시되지 않도록 하려면 ROUND 표현식을 사용해야 합니다.

![사용률 보고서를 포함한 업무 균형자](assets/round02.png)

<b>계산된 필드에서 ROUND 데이터 표현식 사용</b>

ROUND 표현식은 표현식 이름(ROUND)과 일반적으로 두 개의 데이터 포인트를 포함합니다. 이러한 데이터 포인트는 Workfront의 표현식 또는 필드일 수 있으며, 뒤에는 원하는 소수 자릿수를 나타내는 숫자가 옵니다.

표현식은 ROUND(데이터 포인트, #)와 같이 구성됩니다.

계획된 시간과 실제 시간의 차이를 계산하는 식에서 이 표현식 —DIV(SUB({workRequired},{actualWorkRequired}),60)—을 첫 번째 데이터 포인트로 사용합니다. 그런 다음 해당 표현식에서 나온 숫자가 소수점의 오른쪽에 있는 2자리를 넘지 않도록 해야 한다.

![사용률 보고서를 포함한 업무 균형자](assets/round03.png)

표현식은 ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2)와 같이 작성할 수 있습니다.
