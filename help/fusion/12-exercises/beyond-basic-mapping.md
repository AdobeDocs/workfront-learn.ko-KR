---
title: 추가 기본 매핑 연습
description: 매핑 패널 공식을 사용하여 모듈로 전송된 필드를 조작하거나 전환하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,noCatalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 100%

---

# 추가 기본 매핑 연습

매핑 패널 공식을 사용하여 모듈로 전송된 필드를 조작하거나 전환하는 방법을 알아봅니다.

## 연습 개요

매핑 패널 수식을 사용하여 추가 기본 매핑 워크스루에서 프로젝트 이름, 계획된 시작 일자 및 우선 순위를 변경합니다.

![추가 기본 매핑 이미지 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## 따라야 할 단계

**초기 시나리오 디자인 시나리오의 복제본을 만듭니다.**

1. 아래와 같이 시나리오 섹션에서 초기 시나리오 디자인 오른쪽에 있는 복제 옵션을 선택합니다. 이름을 “추가 기본 매핑”으로 지정합니다.

   ![추가 기본 매핑 이미지 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **이제 Workfront 만들기 프로젝트 모듈의 매핑 패널을 사용하여 프로젝트 이름, 계획된 시작 일자 및 우선 순위 필드를 구성합니다.**

1. Workfront 프로젝트 만들기 모듈을 클릭하여 설정을 편집합니다. 매핑 패널을 사용하여 이름 필드를 “[스폰서]별 [내 프로젝트 이름]”으로 바꿉니다.

   + [내 프로젝트 이름]은 CSV 구문 분석 모듈의 1열이고, [스폰서]는 6열입니다. “별”이라는 단어는 둘 사이에 입력됩니다.

1. 다음으로 계획된 시작 일자로 이동하고 addDays 수식을 사용하여 추가 기본 매핑 워크스루 비디오에 설명된 대로 필드에 15일을 추가합니다.
1. 우선 순위 필드를 찾아 필드 오른쪽 상단에 있는 지도 버튼을 전환합니다. 선택 목록 메뉴가 숫자로 변경됩니다. CSV 파일 신뢰도 등급이 100 미만인 경우 프로젝트에 높음(4) 우선 순위로 레이블을 지정하는 if 문을 만들고, 그렇지 않으면 보통(2)이 될 수 있습니다.

   + 신뢰도 등급은 열 4에 있습니다.

   **이 시점에서 매핑 패널은 다음과 같아야 합니다.**

   ![추가 기본 매핑 이미지 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. 확인을 클릭한 다음 한 번 실행을 클릭합니다.
1. Workfront 인스턴스에서 프로젝트를 찾아 모든 것이 올바르게 매핑되었는지 확인합니다.
1. 시나리오를 저장합니다.
