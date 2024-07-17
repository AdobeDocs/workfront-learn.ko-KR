---
title: 계산된 필드 및 표현식 시작하기
description: 조직에서 수행 중인 작업에 대한 고유한 사용자 정의 데이터를 수집하기 위해 계산된 필드에서 표현식을 만드는 방법을 알아봅니다.
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
source-wordcount: '503'
ht-degree: 100%

---

# 계산된 필드 및 표현식 시작하기

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

Workfront는 여러 비즈니스 영역에서 공통으로 사용되며 업무 관리에 정기적으로 사용되는 다양한 필드를 제공합니다. 계획된 완료 일자, 프로젝트 예산, 작업 할당자 이름 등과 같은 필드

그러나 각 조직에는 회사 목표가 충족되고 있는지 이해하기 위해 수집해야 하는 업계 및 회사 고유의 데이터가 있습니다. 예를 들어 조직에서 다음을 추적하려고 합니다.

* 프로젝트가 영향을 줄 비즈니스 라인
* 공급업체, 내부 또는 둘 다에서 자금을 조달하는지 여부
* 사용된 이미지에 필요한 해상도

이러한 필드는 기본적으로 [!DNL Workfront]에 내장되어 있지는 않지만, 사용자 정의 양식을 통해 사용자 정의 데이터 입력 필드와 미리 입력된 다중 선택 답변 필드를 만들 수 있습니다.

이 학습 경로는 계산된 필드에 중점을 둡니다. 계산된 필드의 정의, 데이터 표현식을 통해 계산된 필드로 가져올 수 있는 다양한 유형의 정보, 데이터 수집 및 보고를 개선하기 위해 이러한 계산된 필드를 작성하는 방법을 배웁니다.

![리소스 관리로 하나의 호출기 설정](assets/GS01.png)

## 계산된 필드란 무엇입니까?

계산된 필드에는 데이터 표현식과 기존 Workfront 필드를 사용하여 만든 사용자 정의 데이터가 있습니다.

![활용성 보고서가 포함된 워크로드 밸런서](assets/GS02.png)

예를 들어 조직에는 다음을 포함하는 특정 프로젝트 번호 매기기 또는 작업 번호 시스템이 있습니다.

* 프로젝트가 생성된 연도
* 프로젝트 소유자의 이니셜
* [!DNL Workfront] 프로젝트 참조 번호


계산된 필드의 표현식을 사용하여 [!DNL Workfront]에 이미 저장된 각 정보를 가져와서 고유한 프로젝트 ID 또는 작업 번호를 생성할 수 있으며, 다음과 같이 보고서에 추가할 수 있습니다.

![활용성 보고서가 포함된 워크로드 밸런서](assets/GS03.png)

필요한 특정 데이터에 따라 계산된 필드는 하나 또는 두 개의 표현식을 사용하여 단순하거나, 여러 임베드된 표현식을 사용하여 복잡할 수 있습니다. Workfront는 계산된 필드에 대해 시스템에 이미 저장되었거나 가져온 데이터만 사용할 수 있다는 점을 명심하십시오.

## 텍스트 표현식

텍스트 표현식은 [!DNL Workfront]에서 찾을 수 있는 정보를 검색, 분석 및 결합하여 보다 의미 있는 데이터를 만들거나 조직에서 수행 중인 작업에 대한 더 많은 인사이트를 얻을 수 있습니다.

예를 들어 텍스트 표현식을 사용하여 다음과 같은 작업을 수행할 수 있습니다.

* 프로젝트 보기 열에서 프로젝트 비용이 $5,000를 초과하면 “$5,000 초과”를 표시하고 비용이 그 이하이면 “$5,000 이하”를 표시합니다.

* 각 프로젝트에 프로젝트가 생성된 연도, 프로젝트의 [!DNL Workfront] 참조 번호, 프로젝트 이름 및 프로젝트 소유자의 이니셜이 포함된 고유 번호를 지정합니다.

* 관리자 회의에서 사용할 수 있도록 포트폴리오 및/또는 프로그램에 할당되지 않은 모든 프로젝트를 나열하는 보고서를 빌드합니다.

Workfront에서 이러한 유형의 검색 및 조합을 수행하기 위해 사용자 정의 필드에 텍스트 표현식을 사용할 수 있습니다.

가능한 텍스트 표현을 살펴보면 몇 가지 옵션을 찾을 수 있습니다.

![리소스 관리로 하나의 호출기 설정](assets/TE01.png)

가장 자주 사용되는 여섯 개의 텍스트 표현식은 다음과 같습니다.

* CONCAT
* LEFT / RIGHT
* 포함
* IF
* ISBLANK