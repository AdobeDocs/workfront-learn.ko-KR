---
title: 우수 사례 - 텍스트 모드 보고
description: Workfront 텍스트 모드 보고 설정, 관리 및 사용에 대한 Adobe Workfront 전문가의 우수 사례 권장 사항을 살펴보십시오.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
kt: 10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# 우수 사례 - 텍스트 모드 보고

## Adobe Workfront &quot;모범 사례&quot;란 무엇입니까?

모범 사례는 효과적이고 효율적인 작업 과정을 나타내는 지침입니다. 는 사용자와 회사의 사용자가 쉽게 채택할 수 있습니다. 또한 조직 전반에 걸쳐 성공적으로 복제할 수 있습니다.

이러한 권장 사항을 검토할 때 일부 Workfront 우수 사례는 일반적이지만, 다른 권장 사항은 주제에 더 구체적일 수 있음을 유의하십시오. 이러한 우수 사례를 프레임워크로 사용하여 Workfront 시스템 설정 및 사용을 안내할 수 있습니다.

## 이 페이지 탐색

이 페이지를 스크롤하면 먼저 주제에 대한 모든 우수 사례 목록이 표시됩니다. 이렇게 하면 &quot;이유&quot;의 세부 사항으로 이동하지 않고 권장 사항을 검토할 수 있습니다.

&quot;이러한 우수 사례는 무엇입니까?&quot;가 상위 수준 목록 다음에 있는 영역은 일부 우수 사례에 더 자세한 정보를 제공하고 프로세스, 도구 등으로 간주되는 이유를 Workfront 인스턴스로 구현하는 것이 좋습니다.

</br>
</br>

## 텍스트 모드 보고 우수 사례

* 목록 보고서 열에서 가능한 한 계산된 사용자 지정 필드 대신 텍스트 모드 값 표현식을 사용합니다.

* 보고서의 설명에 텍스트 모드 계산에 사용된 계산을 넣습니다.

</br>
</br>

## 이러한 우수 사례는 무엇입니까?

**우수 사례**

목록 보고서 열에서 가능한 한 계산된 사용자 지정 필드 대신 텍스트 모드 값 표현식을 사용합니다.



**이유가 여기에 있습니다**

텍스트 모드 값 표현식은 보고서가 실행될 때 계산되며 보고서를 새로 고칠 때마다 다시 계산됩니다. 즉, 항상 최신 데이터와 정확한 보고서를 가질 수 있습니다.



Workfront에 데이터가 표시될 때 계산된 사용자 지정 필드(사용자 지정 양식에서 사용됨)가 자동으로 업데이트되지 않습니다. 대신 Workfront에 저장된 최신 계산 결과를 표시합니다. 즉, 해당 값이 지정된 시간에 &quot;부실&quot; 또는 오래된 것일 수 있습니다. 계산된 사용자 지정 필드는 표현식을 다시 계산하거나 계산된 필드가 포함된 개체를 편집하고 저장하여 수동으로 새로 고쳐야 합니다. 이것은 하는 것을 잊어버리기 쉬울 뿐만 아니라 시간이 걸릴 수 있다.


</br>
</br>

**우수 사례**

보고서의 설명에 텍스트 모드 계산에 사용된 계산을 넣습니다.



**이유가 여기에 있습니다**

보고서의 설명에 텍스트 모드 계산을 포함하는 것은 다른 사람이 계산이 어떻게 만들어졌는지 그리고 어떤 종류의 정보를 표시해야 하는지를 이해하는 데 도움이 됩니다. 또한 시스템 관리자에게 향후 업데이트가 필요한 경우 보고서가 어떻게 작성되었는지 알려줍니다.
