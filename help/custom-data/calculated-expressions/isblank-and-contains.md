---
title: ISBLANK 및 CONTAINS 표현식 사용
description: Adobe의 계산된 필드에서 ISBLANK 및 CONTAINS 표현식을 사용하고 만드는 방법을 알아봅니다 [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# ISBLANK 및 CONTAINS 표현식 사용

CONTAINS 및 ISBLANK 표현식은 모두 간단한 true 또는 false 값을 제공하는 데 사용됩니다. 차이점은 ISBLANK 표현식이 필드에 값이 전혀 들어 있지 않은지, CONTAINS 텍스트 표현식이 필드 내에서 특정 문자열을 검색하는지 확인하는 것입니다.

예를 들어 프로젝트에 설명이 있는지 확인하려면 ISBLANK 표현식을 사용합니다. 설명 필드가 비어 있으면 이 표현식은 true 값을 반환합니다. 설명 필드가 비어 있지 않으면 false 값을 반환합니다.

![사용률 보고서를 포함한 업무 균형자](assets/isblank01.png)

&quot;자선 행사&quot;와 같은 설명에서 특정 값을 찾으려면 CONTAINS 텍스트 표현식을 사용합니다. 설명에서 &quot;자선 행사&quot;를 찾으면 계산된 필드에 &quot;참&quot;이라고 표시됩니다. &quot;자선 행사&quot;를 찾지 못하면 &quot;false&quot;로 표시됩니다.

![사용률 보고서를 포함한 업무 균형자](assets/isblank02.png)

## ISBLANK

ISBLANK 텍스트 표현식에는 표현식의 이름과 하나의 데이터 포인트가 포함됩니다.

**ISBLANK({data point})**

![사용률 보고서를 포함한 업무 균형자](assets/isblank03.png)

위의 예에서, 프로젝트에 설명이 있는지 알고 싶은 경우 표현식은 다음과 같습니다.

ISBLANK({description})

## 포함

CONTAINS 텍스트 표현식에는 표현식 이름, 찾고 있는 단어 또는 구 및 찾을 필드가 포함됩니다.

**CONTAINS(&quot;구문&quot;,{fields})**

찾고 있는 단어나 구 주위에 따옴표를 넣어야 합니다. 그렇지 않으면 표현식이 유효하지 않습니다.

위의 예에서(프로젝트 설명에서 &quot;자선 이벤트&quot;를 찾는 경우) 표현식은 다음과 같습니다.

**CONTAINS(&quot;자선 행사&quot;,{description})**

![사용률 보고서를 포함한 업무 균형자](assets/isblank04.png)

**참고**: CONTAINS 표현식은 대소문자를 구분합니다. 예를 들어 &quot;자선 이벤트&quot;가 설명 필드에 대문자로 표시된 경우 표현식에서 해당 구를 대문자로 표시합니다.

**CONTAINS(&quot;자선 이벤트&quot;,{description})**

값이 있는지 확인하려는 경우 ISBLANK 및 CONTAINS 표현식 모두 사용하는 것이 좋습니다. 그러나 값이 무엇인지 알고 실제로 보거나 더 나은 통찰력을 제공하기 위한 일종의 설명자를 갖는 것이 더 유용할 수 있습니다.

예를 들어, 프로젝트가 요청에서 전환되었다는 것만 알고 있는 대신 원래 요청의 이름을 알고 싶을 수 있습니다.

이 경우 IF 표현식과 함께 CONTAINS 표현식을 사용합니다.

ISBLANK 및 CONTAINS 텍스트 표현식은 IF 텍스트 표현식과 함께 사용되는 경우가 많습니다.
