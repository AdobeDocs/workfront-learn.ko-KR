---
title: 고급 집계 연습
description: 웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역별로 그룹화된 인구를 확인합니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
recommendations: noDisplay,noCatalog
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '493'
ht-degree: 100%

---

# 고급 집계 연습

집계할 때 그룹화를 사용하는 방법을 이해합니다.

## 연습 개요

웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고, 하위 지역별로 그룹화된 모든 국가의 총 인구를 확인합니다.

![고급 집계 이미지 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## 따라야 할 단계

**국가 세부 정보를 가져옵니다.**

![고급 집계 이미지 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. 새 시나리오를 만들고 이름을 “고급 집계”로 지정합니다.
1. 트리거 모듈을 HTTP - 요청 만들기 모듈로 설정합니다.
1. 스페인어를 사용하는 모든 국가 목록이 있는 해당 URL(`https://restcountries.com/v2/lang/es`)을 사용합니다.
1. 메서드를 가져오기로 둡니다.
1. 응답 구문 분석 확인란을 클릭합니다.
1. 이 모듈의 이름을 “국가 가져오기”로 바꿉니다.
1. 저장을 클릭하고 한 번 실행을 클릭합니다.

   **출력은 단일 번들이지만, 각 스페인어 사용 국가에 대해 하나씩 24개의 컬렉션이 있는 배열로 제공됩니다.**

   ![고급 집계 이미지 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **각 국가에 대한 하위 지역 정보를 수집해야 하므로 추가 HTTP 요청을 수행해야 합니다.**

1. 하위 지역 정보를 얻으려면 다른 요청을 추가합니다. 첫 번째 국가만 반환하지만 지금은 괜찮습니다. 다른 HTTP 추가 요청 모듈을 만들고 해당 URL(`https://restcountries.com/v2/name/{country name}`)을 사용합니다.
1. 첫 번째 국가의 이름을 얻으려면 매핑 패널로 이동하고 데이터를 클릭한 다음 배열에서 이름을 클릭합니다. 데이터 필드의 [1]은 배열의 첫 번째 항목을 반환한다는 의미입니다.

   + 필요한 경우 숫자를 클릭하고 색인을 변경하지만, 이 경우에는 첫 번째 항목만 해당합니다.

![고급 집계 이미지 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. 매핑 패널에서 응답 구문 분석을 선택한 후 확인을 클릭합니다.
1. 이 이름을 “국가 세부 정보 가져오기”로 바꿉니다.
1. 저장을 클릭한 다음 한 번 실행을 클릭합니다.

   + 출력은 단일 국가에 대한 정보입니다.

1. 다른 국가를 가져오려면 배열을 반복해야 합니다. 항목 목록을 가져오고 목록의 각 항목에 대한 번들을 출력하는 반복기를 추가합니다.

   **반복기와 집계기를 추가합니다.**

1. HTTP 모듈 사이를 마우스 오른쪽 버튼으로 클릭하고 반복기 흐름 제어 모듈을 추가합니다.
1. 배열 필드에서 국가 가져오기 모듈의 데이터를 선택합니다.

   ![고급 집계 이미지 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. 국가 세부 정보 가져오기 모듈에서 URL 필드를 업데이트하여 국가 가져오기 모듈 대신 반복기에서 이름 필드를 가져옵니다.

   ![고급 집계 이미지 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. 이제 국가 세부 정보 가져오기 뒤에 숫자 집계기를 추가하여 인구를 그룹화하여 합산합니다.
1. 소스 모듈은 반복기 모듈입니다.
1. 집계 함수는 SUM입니다.
1. 값은 국가 세부 정보 가져오기 모듈의 [데이터:인구]입니다.
1. 국가 세부 정보 가져오기 모듈에서 하단의 고급 설정 표시 옵션을 클릭하고 [데이터:하위 영역]을 그룹화합니다.

   ![고급 집계 이미지 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **텍스트 집계기로 마무리하여 숫자 집계기 내에서 그룹화한 항목을 집계합니다.**

1. 끝에 텍스트 집계기를 추가합니다.
1. 소스 모듈은 숫자 집계기입니다.
1. 텍스트 영역에 “[키]의 총 인구가 [결과값]입니다”를 삽입합니다

   ![고급 집계 이미지 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. 저장하고 한 번 실행을 클릭합니다.

   + 최종 모듈의 출력을 검토합니다.
