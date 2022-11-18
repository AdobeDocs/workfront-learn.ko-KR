---
title: 실행, 주기 및 번들 탐색
description: 시나리오의 실행 기록을 사용하여 실행, 주기 및 번들이 작동하는 방식을 이해합니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11050
thumbnail: KT1101.png
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 실행, 주기 및 번들 탐색

시나리오의 실행 기록을 사용하여 실행, 주기 및 번들이 작동하는 방식을 이해합니다.

## 연습 개요

실행 및 주기를 사용하여 탐색하기 위해 다양한 시나리오 구성을 사용하는 연습을 수행합니다.

![실행 주기 및 번들 이미지 1 탐색](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## 수행할 단계

1. &quot;라우팅 경로 간 변수 공유&quot;라는 시나리오를 복제합니다. 새 시나리오의 이름을 &quot;라우팅 경로 간 변수 공유 - 주기 테스트&quot;로 지정합니다.
1. 이 테스트에 필요하지 않으므로 이메일 보내기 모듈을 제거합니다.

   **실행 당 3개의 주기를 처리하도록 시나리오를 설정합니다. 각 사이클에 5개의 프로젝트를 처리합니다.**

1. 트리거 모듈을 클릭하고 최대 필드를 5로 변경하여 각 사이클에서 5개의 프로젝트만 처리됩니다.
1. 검색 조건에서 검색을 단일 프로젝트로 제한하는 두 번째 필터를 제거합니다.
1. 확인 을 클릭합니다.

1. Fusion 도구 모음에서 Scenario 설정을 열고 Max Number of cycles 필드를 1에서 3으로 변경합니다.
1. 확인 을 클릭합니다.

   ![실행 주기 및 번들 이미지 1 탐색](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **매분 동안 실행할 시나리오를 예약합니다.**

1. 트리거 모듈 옆에 있는 시계 아이콘을 클릭하고 분 필드를 1분으로 변경합니다.

   ![실행 주기 및 번들 이미지 2 탐색](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. 그런 다음 한 번 실행 단추 아래의 예약 전환을 켜기로 전환합니다. 시나리오를 저장합니다.

   ![실행 주기 및 번들 이미지 3 탐색](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. 시나리오에 대한 실행 내역으로 이동하여 다음 분 내에 새 기록 레코드가 표시되는 것을 확인합니다. 페이지를 새로 고쳐야 할 수 있습니다.

   ![실행 주기 및 번들 이미지 1 탐색](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. 실행의 Details 단추를 누릅니다. Workfront Fusion Training의 실행 기록 부분에서 수행한 것과 유사한 오른쪽 패널의 단순 로그를 클릭합니다.
1. 처리된 작업의 기록은 사이클로 구분됩니다.

   ![실행 주기 및 번들 Image 5 탐색](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. 창 오른쪽 상단의 드롭다운 메뉴를 사용하면 매번 실행되도록 설정한 3개의 주기 중 하나를 선택할 수 있습니다.

   ![실행 주기 및 번들 이미지 6 탐색](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
