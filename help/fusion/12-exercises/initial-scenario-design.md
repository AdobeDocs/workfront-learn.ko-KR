---
title: 초기 시나리오 디자인
description: 첫 번째 시나리오를 빌드하고 Workfront Fusion에 처음 로그인할 때 사용할 몇 가지 기본 탐색 팁을 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---

# 초기 시나리오 디자인

첫 번째 시나리오를 빌드하고 Workfront Fusion에 처음 로그인할 때 사용할 몇 가지 기본 탐색 팁을 알아봅니다.

## 연습 개요

프로젝트 목록 CSV 파일의 각 행에 대해 Workfront에서 새 프로젝트를 만듭니다.

![초기 시나리오 디자인 이미지 1](../12-exercises/assets/initial-scenario-design-1.png)

## 수행할 단계

1. 시나리오 섹션에서 &quot;Fusion enablement 연습&quot;이라는 폴더를 만듭니다.
1. 폴더를 클릭한 다음 새 시나리오 만들기를 클릭합니다.

   ![초기 시나리오 디자인 이미지 2](../12-exercises/assets/initial-scenario-design-2.png)

1. 다음 페이지에서 Workfront을 검색하고 해당 앱을 선택합니다. 그런 다음 계속을 클릭합니다.
1. 시나리오 디자이너 화면의 왼쪽 상단에서 시나리오 이름을 &quot;초기 시나리오 디자인&quot;으로 변경합니다
1. 화면 가운데에 있는 빈 트리거 모듈을 클릭하고 Workfront 앱을 선택한 다음 문서 다운로드 모듈을 선택합니다.

   **Workfront 계정에 대한 모듈의 연결을 인증합니다.**

1. 처음으로 연결을 만들려면 추가 단추를 클릭합니다.

   ![초기 시나리오 디자인 이미지 3](../12-exercises/assets/initial-scenario-design-3.png)

1. 연결에 &quot;My Workfront 2020&quot;과 같은 이름을 지정합니다

   ![초기 시나리오 디자인 이미지 4](../12-exercises/assets/initial-scenario-design-4.png)

1. Workfront 인스턴스의 URL을 입력하고 다음 을 클릭합니다.

   ![초기 시나리오 디자인 이미지 5](../12-exercises/assets/initial-scenario-design-5.png)

1. 암호를 입력하고 로그인 을 클릭합니다.

   **연결이 설정되었습니다. 이제 Workfront에서 다운로드할 문서의 문서 ID를 입력합니다.**

   ![초기 시나리오 디자인 이미지 7](../12-exercises/assets/initial-scenario-design-7.png)

1. Workfront으로 돌아갑니다. &quot;Fusion Experience Files&quot; 폴더에서 &quot;_Fusion2020_Project List.csv&quot;를 선택하고 왼쪽 패널에서 문서 세부 정보 를 클릭합니다. URL 주소에서 문서 ID 번호를 복사합니다. URL에서 첫 번째 긴 숫자입니다.

   ![초기 시나리오 디자인 이미지 8](../12-exercises/assets/initial-scenario-design-8.png)

1. Fusion으로 돌아가서 문서 ID 필드에 숫자를 붙여 넣은 다음 확인을 클릭합니다.
1. 모듈을 만들 때 모듈의 이름을 바꾸는 것이 좋습니다. Workfront 모듈을 마우스 오른쪽 단추로 클릭하고 이름 변경을 선택합니다. 모듈 이름을 &quot;Get project list&quot;로 지정합니다.

   **그런 다음 방금 다운로드한 CSV 파일을 구문 분석하여 파일의 각 행에 액세스할 수 있습니다. 각 행에서 프로젝트를 만들 때 이 정보를 사용합니다.**

1. 다른 모듈을 추가하려면 Workfront 모듈 오른쪽을 클릭합니다. CSV 앱을 검색하고 CSV 구문 분석 모듈을 선택합니다.
1. 6개의 열에 대해 CSV 구문 분석을 설정하고, CSV에는 헤더, 쉼표 구분 기호, 유형이 포함되어 있으며, 데이터를 CSV 필드에 넣습니다. 그런 다음 확인 을 클릭합니다.

   ![초기 시나리오 디자인 이미지 9](../12-exercises/assets/initial-scenario-design-9.png)

1. 이 모듈 이름을 &quot;프로젝트 목록 구문 분석&quot;으로 바꿉니다.
1. 시나리오 디자이너 하단에서 저장 을 클릭하여 시나리오를 저장합니다.
1. 한 번 실행 을 클릭하여 출력을 확인합니다.

   >[!NOTE]
   >
   >변압기가 마지막 모듈이 아니어야 한다는 경고를 무시하십시오(이는 true이지만 이 테스트에는 중요하지 않음). 실행을 클릭합니다.

   ![초기 시나리오 디자인 이미지 10](../12-exercises/assets/initial-scenario-design-10.png)

1. Parse CSV 모듈에서 실행 관리자를 열어 모듈의 입력 및 출력을 확인합니다. 입력으로 하나의 번들(CSV 파일)과 출력(CSV 파일의 각 행에 대해 하나의 번들)이 있습니다. 다음과 같이 표시되어야 합니다.

   ![초기 시나리오 디자인 이미지 11](../12-exercises/assets/initial-scenario-design-11.png)

   **CSV 파일의 각 행에 대한 프로젝트를 만드는 모듈을 추가합니다.**

1. 다른 모듈을 추가합니다. Workfront 앱을 선택하고 레코드 만들기 모듈을 선택합니다.
1. 레코드 유형을 프로젝트로 설정합니다.

   >[!TIP]
   >
   >다음과 같은 몇 개의 문자를 입력하여 검색합니다. *proj*&#x200B;바로 사용할 수 있습니다.

1. 그런 다음 Cmd/Ctrl+G를 사용하여 이름(프로젝트 이름)을 찾습니다. 이름 옆에 있는 상자를 선택합니다. 필드가 아래에 나타납니다.
1. 이제 계획 시작 일자 및 우선순위 옆에 있는 상자를 선택합니다.
1. 이름 필드를 클릭하여 매핑 패널이 나타납니다. CSV 구문 분석 모듈에서 열 1 필드를 클릭하여 이름 필드에 추가합니다. CSV 파일의 프로젝트 이름입니다.
1. 계획된 시작 날짜에 대해 CSV 구문 분석 모듈에서 열 5 를 클릭합니다.
1. [우선 순위]의 드롭다운 메뉴에서 [일반]을 선택합니다.

   **매핑 패널은 다음과 같아야 합니다.**

   ![초기 시나리오 디자인 이미지 12](../12-exercises/assets/initial-scenario-design-12.png)

1. 확인 을 클릭합니다.

   >[!NOTE]
   >
   >확인 을 클릭하지 않고 실수로 다시 디자이너로 클릭하면 작업이 저장되지 않고 다시 매핑해야 합니다.

1. Workfront 모듈을 마우스 오른쪽 단추로 클릭하고 &quot;Workfront 프로젝트 만들기&quot;의 이름을 변경합니다.
1. 시나리오를 저장하고 한 번 실행 단추를 클릭합니다.
1. 마지막 모듈의 오른쪽 상단에 있는 실행 관리자를 클릭합니다.

   + 20개의 작업이 수행되었습니다. 각 작업은 CSV 파일에서 한 행을 의미하는 번들을 입력 및 출력했으며, 이 번들은 Workfront에서 만들어진 프로젝트입니다. 생성된 프로젝트의 프로젝트 ID가 출력 번들과 함께 표시됩니다.

   ![초기 시나리오 디자인 이미지 13](../12-exercises/assets/initial-scenario-design-13.png)

   **참고 사용**

1. 참고는 시나리오 디자인에 대한 더 많은 가시성을 만드는 데 도움이 됩니다. Workfront 프로젝트 만들기 모듈에 메모를 추가하려면 마우스 오른쪽 단추를 클릭하고 메모 추가 를 선택합니다. 디자이너 창 오른쪽의 패널이 표시되며 모듈에 메모를 추가할 수 있습니다. CSV 파일에서 매핑되는 이름, 계획 시작 날짜 및 우선 순위를 사용하여 프로젝트 만들기 를 입력합니다.
1. 트리거 모듈(첫 번째 Workfront 모듈)에서 수행하는 작업을 설명하는 다른 메모를 추가합니다.
1. 오른쪽 상단 모서리에서 X 를 클릭하여 노트 패널을 닫습니다.

   + 하단 도구 모음에서 메모 버튼을 클릭하거나 모듈을 마우스 오른쪽 단추로 클릭하고 새 메모를 추가하여 참고에 다시 액세스합니다.
   + 메모는 시간 순서대로 정렬됩니다.
   + 노트가 추가되면 노트 단추에 주황색 점이 나타납니다.

   ![초기 시나리오 디자인 이미지 14](../12-exercises/assets/initial-scenario-design-14.png)

1. 컨트롤 도구 모음에서 저장 단추를 클릭하여 시나리오를 저장합니다.
1. Workfront 인스턴스에서 만든 프로젝트를 볼 수 있습니다.
