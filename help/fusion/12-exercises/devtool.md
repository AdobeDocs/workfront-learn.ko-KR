---
title: 개발 도구
description: DevTool을 사용하여 시나리오 문제를 해결하고 복잡한 구성을 용이하게 하는 기능을 개선합니다.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11057
thumbnail: KT11057.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---


# 개발 도구

시나리오 문제를 해결하고 개발 도구를 사용하여 복잡한 구성을 용이하게 하는 기능을 개선합니다.

## 연습 개요

Workfront 개발 도구에서 다양한 영역을 설치하고 사용하여 만든 요청/응답 및 고급 시나리오 디자인 트릭을 자세히 살펴봅니다.

>[!NOTE]
>
>Workfront Fusion Dev 도구는 [Chrome 개발자 도구](https://developer.chrome.com/docs/devtools/).

![Devtool 이미지 1](../12-exercises/assets/devtool-walkthrough-1.png)

## 수행할 단계

**개발 도구를 설치합니다.**

1. 테스트 드라이브의 Fusion Experience Files 폴더에 있는 &quot;workfront-fusion-devtool.zip&quot; 문서를 다운로드하십시오.
1. 폴더에 Zip 파일을 추출합니다.
1. Chrome에서 탭을 열고 를 입력합니다. **chrome://extensions**.
1. 오른쪽 상단의 스위치를 사용하여 개발자 모드를 전환한 다음 왼쪽 상단에 표시되는 &quot;압축 해제 로드&quot; 단추를 클릭합니다. 개발 도구가 들어 있는 폴더를 선택합니다(이 위치에서 압축을 푼 경우).

   ![Devtool 이미지 2](../12-exercises/assets/devtool-walkthrough-2.png)

1. 압축을 풀면 개발 도구가 다른 확장 중에 표시됩니다.

   ![Devtool 이미지 3](../12-exercises/assets/devtool-walkthrough-3.png)

   **라이브 스트림을 사용합니다.**

1. 먼저 &quot;데이터를 동기화하기 위해 데이터 저장소 사용&quot; 시나리오를 엽니다.
1. F12 또는 함수 F12를 입력하여 개발 도구를 엽니다. 또는 Chrome 주소 표시줄에서 3개 점 메뉴를 클릭하고 개발자 도구로 이동할 수 있습니다.

   ![Devtool 이미지 4](../12-exercises/assets/navigate-to-devtools.png)

1. Workfront Fusion 탭을 클릭한 다음 왼쪽 목록에서 라이브 스트림 을 선택합니다.
1. 한 번 실행 을 클릭하여 이벤트가 발생하는 것을 확인합니다.
1. 이벤트를 클릭하면 요청 헤더, 요청 본문, 응답 헤더 및 응답 본문에 대한 오른쪽에 있는 탭이 표시됩니다.

   ![Devtool 이미지 4](../12-exercises/assets/devtool-walkthrough-4.png)

   **시나리오 디버거 사용**

1. 시나리오 디버거 를 선택하고 모듈을 클릭하여 해당 모듈의 작업에 대한 정보를 확인합니다.

   ![Devtool 이미지 5](../12-exercises/assets/devtool-walkthrough-5.png)

1. 작업 내역 탭으로 이동합니다. 특정 실행을 위해 모듈 작업 세부 사항을 검사하려면 실행에 대한 세부 정보 를 클릭합니다.

   ![Devtool 이미지 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **도구 사용**

1. 시나리오 디자이너로 돌아가서 개발 도구에서 도구를 선택합니다. 사용 가능한 도구가 표시됩니다.

   ![Devtool 이미지 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ 모듈 포커스 지정 - 모듈 ID를 사용하여 모듈을 빠르게 찾고 엽니다.
+ 매핑으로 모듈 찾기 - 키워드를 사용하여 시나리오를 검색하여 모듈에서 매핑된 값 및/또는 키를 찾습니다.
+ 앱 메타데이터 가져오기 - 시나리오에서 선택한 앱에 대한 메타데이터를 참조하십시오.
+ 매핑 복사 - 한 모듈에서 다른 모듈로의 매핑을 복사합니다. 디자이너에서 모듈을 복제할 수도 있습니다.
+ 필터 복사 - 필터를 복사합니다. 필터가 항상 오른쪽의 모듈에 할당됩니다.
+ 연결 교체 - 이 도구는 선택한 모듈에서 연결을 가져오고 시나리오에서 동일한 앱의 모든 모듈에 동일한 연결을 설정합니다. 이 기능은 완료된 시나리오 전체에서 연결을 변경해야 하는 경우에 유용합니다. 이 도구를 사용하면 모든 매핑과 시간을 절약할 수 있습니다.
+ 변수 교체 - 전체 시나리오 또는 한 모듈에서 지정된 변수의 모든 발생 항목을 찾아 새 변수로 바꿉니다. 와일드카드는 지원되지 않습니다. 전체 시나리오에 실수로 값을 매핑한 경우 이 값을 사용하여 올바른 값을 쉽게 바꿀 수 있습니다.
+ 앱 교체 - 지정된 앱을 다른 앱으로 교체합니다.
+ 기본 64 - 입력한 데이터를 Base64로 인코딩하거나 Base64를 디코딩합니다. 인코딩된 요청에서 특정 데이터를 검색하려는 경우 유용합니다.
+ 모듈 이름 복사 - 선택한 모듈 이름을 클립보드에 복사합니다.
+ 소스 다시 매핑 - 매핑 소스를 한 모듈에서 다른 모듈로 변경합니다. 먼저 시나리오의 경로에 소스 모듈로 사용할 모듈을 추가해야 합니다.
+ OS 마이그레이션 - Google 시트(레거시) 모듈을 최신 Google 시트 버전으로 업그레이드하기 위해 특별히 만들었습니다. 시나리오 경로에서 모듈의 이전 버전 바로 뒤에 새로운 모듈 버전이 추가됩니다.
