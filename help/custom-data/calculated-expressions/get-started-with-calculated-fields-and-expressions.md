---
title: 계산된 필드 및 표현식 시작
description: 계산된 필드에서 표현식을 만들어 조직에 대해 수행되는 작업에 대한 고유한 사용자 지정 데이터를 수집하는 방법에 대해 알아봅니다.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 계산된 필드 및 표현식 시작

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

Workfront은 여러 비즈니스 영역에 걸쳐 공통적이고 정기적으로 작업 관리에 사용되는 다양한 필드를 제공합니다. 계획된 완료 일자, 프로젝트 예산, 작업 할당자 이름 등의 필드.

그러나 각 조직에는 회사 목표가 충족되고 있는지 파악하기 위해 수집해야 하는 업계 및 회사별 데이터가 있습니다. 예를 들어 조직에서 다음 사항을 추적하려고 합니다.

* 프로젝트가 기여할 사업 부문.
* 자금 조달이 공급자, 내부 또는 둘 다에서 이루어지는 경우.
* 사용된 이미지에 필요한 해상도입니다.

이러한 필드는 기본적으로 다음과 같은 형태로 만들어지지 않습니다. [!DNL Workfront], 사용자 정의 양식을 통해 사용자 정의 데이터 입력 필드 및 미리 채워진 다중 선택 답변 필드를 만들 수 있습니다.

이 학습 경로는 계산된 필드에 초점을 맞춥니다. 계산된 필드가 무엇인지, 데이터 표현식을 통해 계산된 필드로 가져올 수 있는 다양한 유형의 정보, 이러한 계산된 필드를 작성하여 데이터 수집 및 보고를 향상시키는 방법에 대해 알아봅니다.

![리소스 관리 설정 1페이지](assets/GS01.png)

## 계산된 필드란 무엇입니까?

계산된 필드에는 데이터 표현식과 기존 Workfront 필드를 사용하여 생성된 사용자 지정 데이터가 포함됩니다.

![사용률 보고서를 포함한 업무 균형자](assets/GS02.png)

예를 들어, 조직에는 다음을 포함하는 특정 프로젝트 번호 또는 작업 번호 시스템이 있습니다.

* 프로젝트가 생성된 연도,
* 프로젝트 소유자의 이니셜 및
* 다음 [!DNL Workfront] 프로젝트 참조 번호.


계산된 필드에서 표현식을 사용하여에 이미 저장된 각 정보를 가져올 수 있습니다 [!DNL Workfront] 고유한 프로젝트 ID 또는 작업 번호를 만들어 다음과 같이 보고서에 추가할 수 있습니다.

![사용률 보고서를 포함한 업무 균형자](assets/GS03.png)

필요한 특정 데이터에 따라 계산된 필드는 한 개 또는 두 개의 표현식을 사용하여 단순하거나 여러 개의 포함된 표현식을 사용하여 보다 복잡할 수 있습니다. Workfront은 계산된 필드에 대해 이미 저장되었거나 시스템으로 가져온 데이터만 사용할 수 있습니다.

## 텍스트 표현식

텍스트 표현식에서 찾은 정보를 검색, 해부 및 결합 [!DNL Workfront] 보다 의미 있는 데이터를 만들거나 조직에 대해 수행되는 작업에 대한 통찰력을 얻으십시오.

예를 들어 텍스트 표현식을 사용하여 다음을 수행할 수 있습니다.

* 프로젝트 비용이 5,000달러 이상인 경우 &quot;5,000달러 이상&quot;을 표시하고, 그 미만인 경우 &quot;5,000달러 미만&quot;을 프로젝트 보기 열에 표시합니다.

* 프로젝트가 생성된 연도, 프로젝트의 을 포함하는 고유한 번호를 각 프로젝트에 지정합니다.  [!DNL Workfront] 참조 번호, 프로젝트 이름 및 프로젝트 소유자의 이니셜입니다.

* 관리자 모임에서 사용할 수 있도록 포트폴리오 및/또는 프로그램에 할당되지 않은 모든 프로젝트를 나열하는 보고서를 작성하십시오.

사용자 정의 필드에서 텍스트 표현식을 사용하여 Workfront에서 이러한 유형의 검색 및 조합을 수행할 수 있습니다.

가능한 텍스트 표현식을 보면 몇 가지 옵션이 있습니다.

![리소스 관리 설정 1페이지](assets/TE01.png)

가장 자주 사용되는 6개의 텍스트 표현식이 있습니다.

* CONCAT
* 왼쪽 / 오른쪽
* 포함
* IF
* ISBLANK