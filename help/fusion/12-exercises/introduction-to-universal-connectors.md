---
title: 범용 커넥터 소개
description: REST 유니버설 커넥터 작업 및 반환된 데이터 작업에 대한 이해를 넓힙니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# 범용 커넥터 소개

REST 유니버설 커넥터 작업 및 반환된 데이터 작업에 대한 이해를 넓힙니다.

## 연습 개요

스프레드시트에서 Pokemon 문자를 사용하여 HTTP 커넥터를 통해 Poke API를 호출하여 해당 문자에 대한 자세한 정보를 수집하고 게시합니다.

![Universal Connectors 소개 이미지 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## 따라야 할 단계

**Workfront에서 CSV 파일을 다운로드합니다.**

1. Workfront &quot;Fusion Exercise Files&quot; 폴더에서 &quot;_Fusion2020_Shipping Manifest.csv&quot;를 선택하고 문서 세부 정보 를 클릭합니다.
1. URL 주소에서 첫 번째 ID 번호를 복사합니다.
1. Workfront Fusion에서 새 시나리오를 만듭니다. 이름을 &quot;Using universal connectors&quot;로 지정합니다.
1. Workfront 앱에서 문서 다운로드 모듈로 시작합니다.
1. Workfront 연결을 설정하고 Workfront URL에서 복사한 문서 ID를 포함합니다.
1. 이 모듈의 이름을 &quot;배송 매니페스트 다운로드&quot;로 바꾸십시오.

   ![Universal Connectors 소개 이미지 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **배송 매니페스트 데이터를 구문 분석합니다.**

1. 다른 모듈을 추가하고 CSV 구문 분석을 선택합니다.
1. 11개 열에 대한 CSV 구문 분석을 설정합니다. CSV에 헤더 포함 상자를 선택합니다. 쉼표 구분 기호 유형을 선택하고 문서 다운로드 모듈의 데이터를 CSV 필드에 넣습니다.

   ![Universal Connectors 소개 이미지 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. 이 모듈의 이름을 &quot;Parse shipping manifest&quot;로 바꿉니다.
1. 시나리오를 저장하고 실행 을 한 번 클릭하면 다음 단계에서 CSV 파일의 데이터를 볼 수 있습니다.

   **범용 커넥터를 사용하여 포켓몬 데이터를 가져옵니다.**

1. HTTP 요청 만들기 모듈을 추가합니다.
1. URL 필드에서 `https://pokeapi.co/api/v2/pokemon/[Character]`, 여기서 [문자] 는 CSV 구문 분석 모듈에서 열 3에 매핑됩니다.
1. Parse response 확인란을 선택합니다.
1. 고급 설정 표시 를 선택한 다음 &quot;모든 상태를 오류로 평가&quot; 옆에 있는 상자를 선택합니다.
1. 확인 을 클릭하고 &quot;포켓몬 정보 가져오기&quot; 모듈의 이름을 변경합니다.

   **매핑 패널은 다음과 같아야 합니다.**

   ![Universal Connectors 소개 이미지 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **이 연습 부분에서는 CSV 파일의 행 1만 처리합니다.**

1. 포켓몬 정보 가져오기 모듈 앞에 필터를 추가합니다. 이름을 &quot;1행만&quot;으로 지정합니다.
1. ID 번호 1만 전달하도록 조건을 설정합니다. ID 번호 1은 행 1에 있고 ID 필드는 CSV 파일의 열 1에 있습니다.

   ![Universal Connectors 소개 이미지 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. 시나리오를 저장합니다.
1. 한 번 실행 을 클릭하고 HTTP 요청 만들기 모듈에서 수신하는 오류 메시지를 확인합니다.

   >[!IMPORTANT]
   >
   >입력 데이터 URL 필드에 문자 이름이 대문자로 표시됩니다. 문자 이름은 소문자여야 하므로 해당 API 호출을 만들 때는 작동하지 않습니다.

   ![Universal Connectors 소개 이미지 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. HTTP 요청 URL 만들기 필드의 매핑 패널을 사용하여 다음을 만듭니다. [문자] 필드를 만들 때 모든 소문자 **lower** 함수.

   ![Universal Connectors 소개 이미지 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **여러 변수 설정 모듈을 사용하여 API에서 정보를 다시 매핑합니다.**

1. 포켓몬 정보 가져오기 후에 여러 변수 설정 모듈을 추가합니다. 이름, 높이, 무게 및 능력을 매핑합니다.
1. Abilities 필드는 배열이므로 map 함수를 사용하여 배열에 있는 각 기능의 이름에 액세스해야 합니다.

   ![Universal Connectors 소개 이미지 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **필터 없이 시나리오를 실행하여 다른 오류를 찾아냅니다.**

1. CSV 파일의 모든 행을 처리하려면 1행만 이라는 필터를 삭제합니다.

   + 필터 아이콘을 클릭하여 편집합니다.
   + 필터 레이블을 삭제합니다.
   + 조건을 삭제합니다.
   + 확인을 클릭합니다.

1. 시나리오를 저장하고 실행 을 한 번 클릭합니다.
1. 포켓몬 정보 가져오기 모듈에 오류가 발생했습니다. 슈퍼히어로 캐릭터가 Pokemon API에 전달된 것을 볼 수 있습니다.

   >[!NOTE]
   >
   >라우터 연습에서는 슈퍼히어로를 처리하는 별도의 경로를 만들어 이 오류를 해결하는 방법에 대해 알아봅니다.

   ![Universal Connectors 소개 이미지 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
