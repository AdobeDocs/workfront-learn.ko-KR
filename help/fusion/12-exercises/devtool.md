---
title: 개발 도구
description: DevTool을 사용하여 시나리오 문제를 해결하고 복잡한 구성을 간소화할 수 있는 기능을 향상시킵니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11057
thumbnail: KT11057.png
exl-id: 13080212-26cf-4e5f-8f0b-fc59a6f66eb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 개발 도구

개발 도구를 사용하여 시나리오 문제를 해결하고 복잡한 구성을 간소화할 수 있는 기능을 향상시킵니다.

## 연습 개요

Workfront 개발 도구의 여러 영역을 설치하고 사용하여 수행된 요청/응답 및 고급 시나리오 디자인 기법을 자세히 살펴봅니다.

>[!NOTE]
>
>Workfront Fusion Dev 도구는 을 사용할 때 Chrome 브라우저에서만 사용할 수 있습니다. [Chrome 개발자 도구](https://developer.chrome.com/docs/devtools/).

![Devtool 이미지 1](../12-exercises/assets/devtool-walkthrough-1.png)

## 따라야 할 단계

**개발 도구를 설치합니다.**

1. 테스트 드라이브의 Fusion Exercise Files 폴더에 있는 &quot;workfront-fusion-devtool.zip&quot; 문서를 다운로드합니다.
1. 폴더에 Zip 파일의 압축을 풉니다.
1. Chrome에서 탭을 열고 다음을 입력합니다. **chrome://extensions**.
1. 오른쪽 상단의 스위치를 사용하여 개발자 모드를 전환한 다음 왼쪽 상단에 나타나는 &quot;압축 해제된 로드&quot; 단추를 클릭합니다. 개발 도구가 들어 있는 폴더를 선택합니다(이 위치에서 압축을 풉니다).

   ![Devtool 이미지 2](../12-exercises/assets/devtool-walkthrough-2.png)

1. 압축을 해제하면 개발 도구가 다른 확장 프로그램에 나타납니다.

   ![Devtool 이미지 3](../12-exercises/assets/devtool-walkthrough-3.png)

   **라이브 스트림을 사용합니다.**

1. 먼저 &quot;데이터 저장소를 사용하여 데이터 동기화&quot; 시나리오를 엽니다.
1. F12 또는 함수 F12를 입력하여 개발 도구를 엽니다. 또는 Chrome 주소 표시줄에서 점 3개 메뉴를 클릭하고 개발자 도구로 이동할 수 있습니다.

   ![Devtool 이미지 4](../12-exercises/assets/navigate-to-devtools.png)

1. Workfront Fusion 탭을 클릭한 다음 왼쪽의 목록에서 라이브 스트림 을 선택합니다.
1. 이벤트가 발생할 때 확인하려면 실행 을 한 번 클릭합니다.
1. 요청 헤더, 요청 본문, 응답 헤더 및 응답 본문에 대한 오른쪽의 탭을 보려면 이벤트를 클릭합니다.

   ![Devtool 이미지 4](../12-exercises/assets/devtool-walkthrough-4.png)

   **시나리오 디버거 사용**

1. Scenario Debugger를 선택하고 모듈을 클릭하여 해당 모듈의 작업에 대한 정보를 봅니다.

   ![Devtool 이미지 5](../12-exercises/assets/devtool-walkthrough-5.png)

1. 내역 탭으로 이동합니다. 특정 실행에 대한 모듈 작업 세부 사항을 검사하려면 실행 세부 정보 를 클릭합니다.

   ![Devtool 이미지 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **도구 사용**

1. 시나리오 디자이너로 돌아가서 개발 도구에서 도구를 선택합니다. 사용 가능한 도구가 표시됩니다.

   ![Devtool 이미지 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ 모듈 포커스 - 모듈 ID를 사용하여 모듈을 빠르게 찾아 엽니다.
+ 매핑으로 모듈 찾기 - 키워드로 시나리오를 검색하여 모듈의 매핑된 값 및/또는 키를 찾습니다.
+ 앱 메타데이터 가져오기 - 선택한 앱에 대한 메타데이터 시나리오를 참조하십시오.
+ 복사 매핑 - 한 모듈에서 다른 모듈로 매핑을 복사합니다. 디자이너에서 모듈을 복제할 수도 있습니다.
+ 필터 복사 - 필터를 복사합니다. 필터는 항상 오른쪽에 있는 모듈에 할당됩니다.
+ 연결 교체 - 이 도구는 선택한 모듈에서 연결을 가져오고 시나리오에서 동일한 앱의 모든 모듈에 동일한 연결을 설정합니다. 이 기능은 완료된 시나리오 전체에서 연결을 변경해야 하는 경우에 유용합니다. 이 도구를 사용하면 모든 매핑이 손실되지 않고 시간을 절약할 수 있습니다.
+ 변수 교체 - 전체 시나리오 또는 한 모듈에서 주어진 변수의 모든 발생 항목을 찾아 새 변수로 바꿉니다. 와일드카드는 지원되지 않습니다. 전체 시나리오에서 실수로 값을 매핑한 경우 올바른 값으로 쉽게 교환할 수 있습니다.
+ 앱 교체 - 지정된 앱을 다른 앱으로 교체합니다.
+ Base 64 - 입력한 데이터를 Base64로 인코딩하거나 Base64를 디코딩합니다. 인코딩된 요청에서 특정 데이터를 검색하려는 경우에 유용합니다.
+ 모듈 이름 복사 - 선택한 모듈 이름을 클립보드에 복사합니다.
+ 소스 다시 매핑 - 매핑 소스를 한 모듈에서 다른 모듈로 변경합니다. 시나리오에서는 소스 모듈로 사용할 모듈을 경로에 먼저 추가해야 합니다.
+ OS 마이그레이션 - 특히 Google Sheets(이전) 모듈을 최신 Google Sheets 버전으로 업그레이드하기 위해 수행됩니다. 시나리오 경로에서 모듈의 이전 버전 바로 뒤에 새 버전의 모듈이 추가됩니다.
