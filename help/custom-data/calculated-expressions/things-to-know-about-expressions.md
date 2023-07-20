---
title: 계산된 필드 표현식에 대해 알아야 할 사항
description: 에서 사용자 정의 계산된 필드로 작업할 때 알아 두면 좋은 개념 목록에서 희미하게 항목 가져오기 [!DNL Workfront].
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
source-wordcount: '959'
ht-degree: 0%

---

# 계산된 필드 표현식에 대해 알아야 할 사항

다음은 Workfront에서 사용자 정의 계산된 필드로 작업할 때 알아 두면 좋은 개념 목록입니다.

## 표현식 이름의 대/소문자 구분

표현명에 있어서는 대/소문자가 중요하다. 표현식 이름을 처음 작성할 때 대문자, 소문자 또는 두 가지를 혼합하여 사용할 수 있습니다.

![표현식 이름에 대소문자가 없는 오류 메시지](assets/T2K01.png)

단, 표현식을 모두 대문자로 작성해야 시스템이 표현식을 인식하고 필드를 저장할 수 있습니다.



## 시간은 분 단위로 저장됩니다.

Workfront 데이터베이스의 시간은 분 단위로 저장됩니다. 계획된 시간 또는 실제 시간과 같은 필드를 참조하는 경우 60으로 나누어서 분이 아닌 시간 단위로 표시합니다.

## 간격은 표현식에 영향을 주지 않습니다

표현식을 작성하는 데 권장되는 방법은 각 표현식 사이에 간격이 거의 없거나 전혀 없는 것입니다.

* IF(ISBLANK({description}),&quot;설명 없음&quot;,&quot;설명 있음&quot;)

![필드 간 간격이 없는 표현식](assets/T2K02.png)

그러나 간격이 현재 상황을 확인하는 데 도움이 되면 일부 간격을 표현식에 추가할 수 있습니다. 추가 공백은 식이 수집되거나 값을 계산하는 것을 방해해서는 안 됩니다 [!DNL Workfront].

* IF (ISBLANK ({description}), &quot;설명 없음&quot; , &quot;설명 있음&quot; )

![필드 간 간격이 있는 표현식](assets/T2K03.png)

이들 사이에 공백을 가질 수 없는 것은 필드와 중괄호뿐입니다. 그렇지 않으면 오류 메시지가 표시되고 필드 또는 사용자 정의 양식을 저장할 수 없습니다.

![필드 이름과 대괄호 사이의 간격에 오류 발생](assets/T2K04.png)

## 따옴표는 직선이어야 합니다.

표현식에서 따옴표를 사용할 때는 따옴표가 직선(&quot;)인지 확인하십시오. 따옴표가 곡선(&quot;)인 경우 [!DNL Workfront] 시스템은 &quot;잘못된 사용자 정의 표현식&quot; 메시지를 계속 표시합니다.

![곡선 따옴표 관련 오류](assets/T2K05.png)

## 양식 저장 및 개체 편집 시 계산 업데이트

이는 계산된 필드를 이해하는 데 중요한 측면입니다.

계산된 필드에 표시된 정보는 사용자 정의 양식을 다시 계산하지 않는 한 동일하게 유지되며 부실해집니다.

객체의 기타 메뉴에서 표현식 다시 계산 옵션을 사용하여 표현식을 새로 고칠 수 있습니다.

문제가 열린 일수를 확인하려고 합니다. DATEDIFF 표현식을 사용하여 &quot;열린 일수&quot;라는 계산된 필드를 만듭니다.

* 필드 이름 = 열린 일수
* 표현식 = DATEDIFF({entryDate},$$오늘)

저장되면 문제가 처음 생성되거나 Workfront에 입력된 시간과 오늘 날짜 사이의 일수가 오브젝트의 세부 정보 페이지 또는 보고서 보기에 표시될 수 있습니다.

다음 날 동일한 세부 정보 페이지 또는 보고서 보기를 볼 때 해당 숫자가 1씩 증가할 것으로 예상됩니다. 오늘 5번이면 내일 6번이 될 거예요. 다음 날은 7일, 8일 등이어야 합니다.

그러나 필드에는 매일 5개가 계속 표시됩니다. 필드를 &quot;다시 실행&quot;하거나 다시 계산하여 정보를 새로 고쳐야 합니다.

표현식 재계산 옵션을 사용하여 필드를 갱신하려면

* 개체 이름을 클릭하여 엽니다.
* 기타 메뉴를 클릭합니다.
* 목록에서 표현식 재계산을 선택합니다.

![오브젝트의 표현식 옵션 다시 계산](assets/T2K06.png)

목록 또는 보고서에서 &quot;일괄 편집&quot; 기능을 사용하여 여러 표현식을 동시에 다시 계산할 수도 있습니다. 열에 표시된 진행 중 일수 계산과 관련된 문제 목록을 표시하는 보고서를 생성했다고 가정합니다. 모든 문제를 한 번에 다시 계산하려는 경우:

* 보고서에서 모든 문제를 선택합니다.
* 선택한 모든 문제를 일괄 편집하려면 편집 옵션을 선택합니다.
* 왼쪽의 사용자 정의 Forms 레이블을 클릭하여 사용자 정의 양식 섹션으로 스크롤합니다.
* 사용자 지정 Forms 섹션 하단에 있는 사용자 지정 표현식 다시 계산 상자를 선택합니다.
* 변경 내용 저장을 클릭합니다.

![여러 객체에 대한 표현식 옵션 다시 계산](assets/T2K07.png)

화면이 새로 고침되어 계산된 필드에 업데이트된 정보가 표시됩니다.

**참고**: 계산된 필드에서 표현식을 업데이트하거나 다시 계산하는 다른 방법이 있지만 이 방법이 가장 빠르고 쉬운 방법입니다.

## 계산은 동일한 필드 내에서 양식마다 다를 수 있습니다

계산된 필드가 사용자 정의 양식에 저장되고 나면 해당 계산된 필드가 필드 라이브러리에 추가되므로 다른 사용자 정의 양식에서 사용할 수 있습니다.

그러나 양식 A에 계산된 필드가 있고 양식 B에 동일한 계산된 필드가 있다면 초기 생각은 계산이 정확히 동일하다는 것입니다. 항상 그런 것은 아니다. 양식 A의 계산된 필드는 양식 B에서 완전히 다른 방법을 계산할 수 있다.

필드 라이브러리에서 계산된 사용자 정의 필드를 선택하여 사용자 정의 양식에 추가하면 필드가 추가되지만 계산은 비어 있습니다. 이렇게 되는 한 가지 이유는 다른 객체 유형에 대해 존재하지 않는 필드를 계산할 수 있기 때문입니다.

예를 들어 프로젝트에서 작업을 완료하는 데 걸린 시간을 결정하는 계산된 필드인 &quot;완료 일수&quot;를 만들었습니다.

* WEEKDAYDIFF({actualStartDate},{actualCompletionDate})

반복에 대해서도 동일한 작업을 하려고 합니다. 동일한 표현식을 사용할 수 있지만 작업 객체에 사용할 수 있는 필드를 반복 객체에 항상 사용할 수 있는 것은 아닙니다. So [!DNL Workfront] 를 사용하면 올바른 개체 필드를 사용하여 계산을 작성할 수 있습니다.

**Pro-팁**: 사용자 지정 필드를 만들 때 계산 상자의 계산된 표현식을 지침 필드에 복사합니다. 계산된 사용자 정의 필드가 필드 라이브러리의 사용자 정의 양식에 추가되면 이 필드가 지워지지 않습니다.

필요에 따라 사용자 정의 양식의 계산된 필드는 매우 간단하거나 복잡할 수 있습니다. 표현식은 다른 표현식과 값을 포함하거나 중첩하여 조직에서 수행되는 작업과 관련된 상황을 더 잘 파악하는 데 필요한 세부 정보 수준을 제공할 수 있습니다.

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you're ready to start building your own calculated custom fields.-->
