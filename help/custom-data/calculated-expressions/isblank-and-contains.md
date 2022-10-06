---
title: ISBLANK 및 CONTAINS 표현식 사용
description: Adobe의 계산된 필드에서 ISBLANK 및 CONTAINS 표현식을 사용하고 만드는 방법을 알아봅니다 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# ISBLANK 및 CONTAINS 표현식 사용

CONTAINS 표현식과 ISBLANK 표현식은 모두 간단한 true 또는 false 값을 제공하는 데 사용됩니다. 차이점은 ISBLANK 표현식이 필드에 값이 전혀 있는지 확인한 후 CONTAINS 텍스트 표현식이 필드 내에서 특정 문자열을 찾습니다.

예를 들어 프로젝트에 설명이 있는지 확인하려면 ISBLANK 표현식을 사용합니다. 설명 필드가 비어 있으면 표현식이 true 값을 반환합니다. 설명 필드가 비어 있지 않으면 false 값을 반환합니다.

![사용률 보고서가 있는 작업 로드 밸런서](assets/isblank01.png)

&quot;자선 이벤트&quot;와 같이 설명에서 특정 값을 찾으려면 CONTAINS 텍스트 표현식을 사용합니다. 설명에서 &quot;자선 이벤트&quot;를 찾으면 계산된 필드에 &quot;true&quot;가 표시됩니다. 자선행사를 찾지 못하면 &quot;false&quot;로 표시됩니다.

![사용률 보고서가 있는 작업 로드 밸런서](assets/isblank02.png)

## ISBLANK

ISBLANK 텍스트 표현식에 표현식의 이름과 하나의 데이터 포인트가 포함됩니다.

**ISBLANK(데이터 포인트)**

![사용률 보고서가 있는 작업 로드 밸런서](assets/isblank03.png)

위의 예에서 프로젝트에 설명이 있는지 확인하려는 경우 표현식은 다음과 같습니다.

ISBLANK(설명)

## 포함

CONTAINS 텍스트 표현식에는 표현식 이름, 찾고 있는 단어 또는 구, 찾을 필드가 포함됩니다.

**CONTAINS(&quot;phrase&quot;,field)**

찾고 있는 단어나 구에 따옴표를 붙여야 합니다. 그렇지 않으면 표현식이 유효하지 않습니다.

위의 예에서(프로젝트 설명에서 &quot;자선 이벤트&quot;를 찾는) 표현식은 다음과 같습니다.

**CONTAINS(&quot;자선 이벤트&quot;,설명)**

![사용률 보고서가 있는 작업 로드 밸런서](assets/isblank04.png)

**참고**: CONTAINS 표현식은 대/소문자를 구분합니다. 예를 들어, &quot;자선 이벤트&quot;가 설명 필드에서 대문자로 시작하는 경우 표현식에서 해당 구문을 대문자로 표현하십시오.

**CONTAINS(&quot;Charity Event&quot;,Description)**

ISBLANK 및 CONTAINS 표현식은 값이 있는지 확인하려는 경우 사용할 수 있습니다. 그러나 실제로 그 값을 보거나 더 나은 통찰력을 제공하기 위해 어떤 종류의 설명자를 갖는 것이 값이 무엇인지 아는 것이 더 유용할 수 있습니다.

예를 들어 프로젝트가 요청에서 변환되었다는 것을 아는 대신 원래 요청의 이름을 알고 싶을 수 있습니다.

이 경우 IF 표현식과 함께 CONTAINS 표현식을 사용합니다.

ISBLANK 및 CONTAINS 텍스트 표현식은 IF 텍스트 표현식과 함께 사용되는 경우가 많습니다.
