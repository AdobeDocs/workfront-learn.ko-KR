---
title: 고급 집계
description: 웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역으로 그룹화된 모집단을 식별합니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 고급 집계

집계할 때 그룹화를 사용하는 방법을 이해합니다.

## 연습 개요

웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역별로 그룹화된 모든 국가의 총 인구를 식별합니다.

![고급 집계 이미지 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## 따라야 할 단계

**국가 세부 정보를 가져옵니다.**

![고급 집계 이미지 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. 새 시나리오를 만들고 이름을 &quot;Advanced aggregation&quot;으로 지정합니다.
1. 트리거 모듈을 HTTP로 설정 - 요청 모듈을 만듭니다.
1. 이 URL 사용, `https://restcountries.com/v2/lang/es`스페인어를 사용하는 모든 국가의 목록을 제공합니다.
1. 메서드를 Get으로 둡니다.
1. 응답 구문 분석 확인란을 클릭합니다.
1. 이 모듈의 이름을 &quot;Get Countries&quot;로 바꿉니다.
1. 저장 후 실행을 한 번 클릭합니다.

   **출력은 단일 번들이지만 스페인어 사용 국가별로 하나씩 24개의 컬렉션이 제공됩니다.**

   ![고급 집계 이미지 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **각 국가에 대한 하위 지역 정보를 수집해야 하므로 추가 HTTP 요청을 수행해야 합니다.**

1. 다른 요청을 추가하여 하위 영역 정보를 가져옵니다. 첫 번째 국가만 반환하지만 지금은 괜찮습니다. 다른 HTTP 요청 만들기 모듈을 추가하고 URL을 사용합니다 `https://restcountries.com/v2/name/{country name}`.
1. 첫 번째 국가의 이름을 가져오려면 매핑 패널로 이동하여 데이터 를 클릭한 다음 배열에서 이름 을 클릭합니다. 다음 [1] 데이터 필드에서 는 배열의 첫 번째 항목을 반환함을 의미합니다.

   + 숫자를 클릭하고 필요한 경우 색인을 변경합니다. 이 경우 첫 번째 항목만 원하는 것입니다.

![고급 집계 이미지 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. 매핑 패널에서 구문 분석 응답을 선택한 다음 확인을 클릭합니다.
1. 이 이름을 &quot;국가 세부 정보 가져오기&quot;로 바꿉니다.
1. 저장, 실행을 차례로 누릅니다.

   + 산출물은 단일 국가에 대한 정보입니다.

1. 다른 국가로 이동하려면 배열을 반복해야 합니다. 사물 목록을 가져와서 목록의 각 항목에 대한 번들을 출력하는 반복기를 추가합니다.

   **반복자 및 집계를 추가합니다.**

1. HTTP 모듈 사이를 마우스 오른쪽 단추로 클릭하고 Iterator 흐름 제어 모듈을 추가합니다.
1. Array 필드의 Get Countries 모듈에서 Data 를 선택합니다.

   ![고급 집계 이미지 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. Get Country Details 모듈에서 Get Countries 모듈 대신 반복기에서 이름 필드를 가져오도록 URL 필드를 업데이트합니다.

   ![고급 집계 이미지 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. 이제 [국가 세부 사항 가져오기] 뒤에 숫자 집계기를 추가하여 모집단을 그룹화하고 합합니다.
1. 소스 모듈은 반복자 모듈입니다.
1. 집계 함수는 SUM입니다.
1. 값은 입니다. [data:population] Get Country Details 모듈에서
1. 맨 아래에 있는 고급 설정 표시 옵션을 클릭하고 그룹화 기준 [data:subregion] Get Country Details 모듈에서

   ![고급 집계 이미지 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **숫자 집계 내에서 그룹화한 내용을 집계하려면 텍스트 집계기로 완료합니다.**

1. 끝에 텍스트 집계기를 추가합니다.
1. 소스 모듈은 숫자 집계기입니다.
1. 텍스트 영역에 &quot;Total population of [키] 은(는) [결과].&quot;

   ![고급 집계 이미지 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. 한 번 저장 및 실행.

   + 최종 모듈에서 출력을 검토합니다.
