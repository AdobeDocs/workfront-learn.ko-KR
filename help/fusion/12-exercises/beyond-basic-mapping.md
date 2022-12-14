---
title: 기본 매핑 이상의 기능
description: 매핑 패널 공식을 사용하여 모듈로 전송된 필드를 조작하거나 변환하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 기본 매핑 이상의 기능

매핑 패널 공식을 사용하여 모듈로 전송된 필드를 조작하거나 변환하는 방법을 알아봅니다.

## 연습 개요

매핑 패널 공식을 사용하여 기본 매핑 이외의 연습에서 프로젝트 이름, 계획 시작 날짜 및 우선순위를 변경합니다.

![기본 매핑 이미지 1 이상의 기능](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## 수행할 단계

**초기 시나리오 디자인 시나리오를 복제합니다.**

1. 아래 표시된 대로 시나리오 섹션의 초기 시나리오 디자인 오른쪽에 있는 복제 옵션을 선택합니다. 이름을 &quot;기본 매핑 이상의&quot;으로 지정합니다.

   ![기본 매핑 이미지 2의 이점](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **이제 Workfront 프로젝트 만들기 모듈의 매핑 패널을 사용하여 프로젝트 이름, 계획된 시작 날짜 및 우선순위 필드를 구성하겠습니다.**

1. Workfront 프로젝트 만들기 모듈을 클릭하여 설정을 편집합니다. 매핑 패널을 사용하여 이름 필드를 &quot;로 변경합니다.[내 프로젝트 이름] by [스폰서].&quot;

   + 다음 [내 프로젝트 이름] 는 CSV 구문 분석 모듈의 열 1입니다. [스폰서] 는 열 6입니다. &quot;by&quot;라는 단어는 두 단어 사이에 방금 입력되어 있다.

1. 다음으로 계획 시작 날짜로 이동하고 추가Days 공식을 사용하여 기본 매핑 연습 비디오에 설명된 대로 필드에 15일을 추가합니다.
1. 우선순위 필드를 찾아 필드의 오른쪽 상단에 있는 맵 단추를 전환합니다. 선택 목록 메뉴가 숫자로 바뀝니다. CSV 파일 신뢰도 등급이 100보다 작은 경우 프로젝트에 높은(4) 우선 순위로 레이블을 지정하는 if 문을 만듭니다. 그렇지 않으면 일반(2)일 수 있습니다.

   + 신뢰도 등급은 열 4입니다.

   **이때 매핑 패널은 다음과 같아야 합니다.**

   ![기본 매핑 이미지 3 이상의 기능](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. 확인 을 클릭한 다음 실행 을 한 번 클릭합니다.
1. Workfront 인스턴스에서 프로젝트를 찾아 모든 것이 올바르게 매핑되었는지 확인합니다.
1. 시나리오를 저장합니다.
