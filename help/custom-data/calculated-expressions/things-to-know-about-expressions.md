---
title: 계산된 필드 표현식에 대해 알아야 할 사항
description: ' [!DNL Workfront]에서 사용자 정의 계산 필드로 작업할 때 알아 두면 좋은 개념 목록을 살펴봅니다.'
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 100%

---

# 계산된 필드 표현식에 대해 알아야 할 사항

Workfront에서 사용자 정의 계산 필드로 작업할 때 알아 두면 좋은 개념 목록입니다.

## 표현식 이름의 대소문자 구분

표현식 이름은 대소문자를 구분합니다. 표현식 이름을 처음 작성할 때 대문자, 소문자 또는 둘을 혼합하여 사용할 수 있습니다.

![표현식 이름에 대문자가 없는 오류 메시지](assets/T2K01.png)

그러나 시스템에서 표현식을 인식하고 필드를 저장하려면 표현식을 모두 대문자로 작성해야 합니다.



## 시간은 분 단위로 저장

Workfront 데이터베이스의 시간은 분 단위로 저장됩니다. 계획된 시간 또는 실제 근로시간과 같은 필드를 참조하는 경우 60으로 나누어 시간을 분 단위가 아닌 시간 단위로 표시하십시오.

## 공백은 표현식에 영향을 주지 않음

표현식을 작성할 때 권장하는 방법은 각 표현식 사이에 공백이 거의 없거나 전혀 없도록 하는 것입니다.

* IF(ISBLANK({description}),&quot;No Description&quot;,&quot;Has Description&quot;)

![필드 사이에 공백이 없는 표현식](assets/T2K02.png)

그러나 공백이 진행 상황을 파악하는 데 도움이 되는 경우 표현식에 일부 공백을 추가할 수 있습니다. 여분의 공백은 [!DNL Workfront]에서 표현식이 값을 수집하거나 계산하는 데 방해가 되지 않습니다.

* IF (ISBLANK ({description}), &quot;No Description&quot; , &quot;Has Description&quot; )

![필드 사이에 공백이 있는 표현식](assets/T2K03.png)

공백이 있어서는 안 되는 유일한 곳은 필드와 중괄호 사이입니다. 둘 사이에 공백이 있으면 오류 메시지가 표시되며 필드 또는 사용자 정의 양식을 저장할 수 없습니다.

![필드 이름과 중괄호 사이의 공백 오류](assets/T2K04.png)

## 큰따옴표는 곧은 따옴표여야 함

표현식에 큰따옴표를 사용할 때 곧은 따옴표(&quot;)여야 합니다. 둥근 큰따옴표의 경우(“) [!DNL Workfront] 시스템에서 “사용자 정의 표현식이 잘못됨” 메시지를 계속 표시합니다.

![둥근 큰따옴표 오류](assets/T2K05.png)

## 양식 저장 및 오브젝트 편집 시 계산 업데이트

계산된 필드에서 이해해야 하는 중요한 측면입니다.

계산된 필드에 표시되는 정보는 사용자 정의 양식을 다시 계산하지 않는 한 동일하게 유지되며 시간이 지나면 정확도가 떨어집니다.

오브젝트의 ‘더 보기’ 메뉴에 있는 ‘표현식 다시 계산’ 옵션을 사용하여 표현식을 새로 고칠 수 있습니다.

문제가 개시되어 지속된 일수를 확인하려고 합니다. DATEDIFF 표현식을 사용하여 “지속 일수”라는 계산된 필드를 만듭니다.

* 필드 이름 = 지속 일수
* 표현식 = DATEDIFF({entryDate},$$TODAY)

저장하면 문제가 처음 만들어지거나 Workfront에 입력된 일자와 오늘 일자 사이의 일수가 오브젝트의 세부 정보 페이지 또는 보고서 보기에 표시될 수 있습니다.

다음 날 동일한 세부 정보 페이지 또는 보고서 보기를 볼 때 해당 숫자가 1씩 증가해야 합니다. 오늘 숫자가 5라면 내일은 6이어야 합니다. 다음 날은 7, 그 다음 날은 8과 같이 이어져야 합니다.

그러나 필드에는 매일 5가 계속 표시됩니다. 정보를 새로 고치려면 필드를 “다시 실행”하거나 다시 계산해야 합니다.

‘표현식 다시 계산’ 옵션을 사용하여 필드를 업데이트하는 방법은 다음과 같습니다.

* 오브젝트 이름을 클릭하여 엽니다.
* ‘더 보기’ 메뉴를 클릭합니다.
* 목록에서 ‘표현식 다시 계산’을 선택합니다.

![오브젝트의 표현식 다시 계산 옵션](assets/T2K06.png)

목록 또는 보고서에서 “일괄 편집” 기능을 사용하여 동시에 여러 표현식을 다시 계산할 수도 있습니다. 열에 표시되는 ‘지속 일수’ 계산과 함께 문제 목록을 표시하는 보고서를 만들었다고 가정해 보겠습니다. 모든 문제를 한 번에 다시 계산하려면 다음 작업을 수행하십시오.

* 보고서의 모든 문제를 선택합니다.
* 선택한 모든 문제를 일괄 편집하는 편집 옵션을 선택합니다.
* 왼쪽의 ‘사용자 정의 양식’ 레이블을 클릭하여 사용자 정의 양식 섹션까지 아래로 스크롤합니다.
* ‘사용자 정의 양식’ 섹션 하단에 있는 ‘사용자 정의 표현식 다시 계산’ 상자를 선택합니다.
* ‘변경 내용 저장’을 클릭합니다.

![여러 오브젝트에 대한 표현식 다시 계산 옵션](assets/T2K07.png)

화면이 새로 고쳐져 계산된 필드에 업데이트된 정보가 표시됩니다.

**참고**: 계산된 필드에서 식을 업데이트하거나 다시 계산하는 다른 방법이 있기는 하지만 이것이 가장 빠르고 쉬운 방법입니다.

## 계산은 동일한 필드에서 양식마다 다를 수 있음

계산된 필드를 사용자 정의 양식에서 저장하고 이 사용자 정의 양식을 저장하면 계산된 필드가 필드 라이브러리에 추가되어 다른 사용자 정의 양식에서 사용할 수 있습니다.

그런데 양식 A에 계산된 필드가 있고 양식 B에 이 계산된 필드가 그대로 있는 경우 가장 먼저 드는 생각은 두 계산이 완전히 동일하다는 것입니다. 그러나 항상 그렇지는 않습니다. 양식 A의 계산된 필드는 양식 B에서 완전히 다른 방식으로 계산될 수 있습니다.

필드 라이브러리에서 계산된 사용자 정의 필드를 선택하고 사용자 정의 양식에 추가하면 필드가 추가되지만 계산은 비어 있습니다. 이런 경우가 발생하는 이유 중 하나는 계산이 다른 오브젝트 유형에 대해 존재하지 않는 필드를 참조하기 때문입니다.

예를 들어 프로젝트에서 작업을 완료하는 데 걸리는 시간을 확인하기 위해 “완료까지 소요 일수”라는 계산된 필드를 만들었습니다.

* WEEKDAYDIFF({actualStartDate},{actualCompletionDate})

반복에 대해 동일한 작업을 수행하려고 합니다. 이때 같은 표현식을 사용할 수 있습니다. 그러나 작업 오브젝트에 사용할 수 있는 필드가 반복 오브젝트에 항상 사용 가능한 것은 아닙니다. 그래서 [!DNL Workfront]에서는 올바른 오브젝트 필드를 사용하여 계산을 작성할 수 있도록 합니다.

**프로 팁**: 사용자 정의 필드를 만들 때 ‘계산’ 상자에서 계산된 표현식을 ‘지침’ 필드로 복사하십시오. 계산된 사용자 정의 필드가 필드 라이브러리에서 사용자 정의 양식에 추가될 때 이 필드는 지워지지 않습니다.

필요에 따라 사용자 정의 양식의 계산된 필드는 매우 단순하거나 매우 복잡할 수 있습니다. 표현식은 다른 표현식과 값을 임베드하거나 중첩하여 조직에서 수행 중인 작업을 더 잘 파악하는 데 필요한 세부 수준을 제공할 수 있습니다.

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you're ready to start building your own calculated custom fields.-->
