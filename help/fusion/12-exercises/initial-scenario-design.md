---
title: 초기 시나리오 디자인
description: Workfront Fusion에 처음 로그인할 때와 첫 번째 시나리오 빌드에 대한 몇 가지 기본 탐색 팁에 대해 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: e639d3391ea6a8b46592dd18cf57b9eed50fbf8c
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 0%

---

# 초기 시나리오 디자인

Workfront Fusion에 처음 로그인할 때와 첫 번째 시나리오 빌드에 대한 몇 가지 기본 탐색 팁에 대해 알아봅니다.

## 전제 조건

1. 이 연습을 수행하려면 Workfront 테스트 드라이브가 필요합니다. 작성하셔서 요청하시면 됩니다 [이 양식](https://forms.office.com/r/f1J8HRGrNY). 양식에 액세스할 수 없는 경우 이름, 이메일 주소 및 회사 이름을 wfttstdr@adobe.com으로 보내십시오.
1. Fusion 연습에서는 연습에 해당하는 연습 비디오를 시청했다고 가정합니다. 이 경우에는 [초기 시나리오 디자인 연습](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/understand-the-basics/initial-scenario-design-walkthrough.html?lang=en).


## 연습 개요

프로젝트 목록 CSV 파일의 각 행에 대해 Workfront에서 새 프로젝트를 만듭니다.

![초기 시나리오 디자인 이미지 1](../12-exercises/assets/initial-scenario-design-1.png)

## 따라야 할 단계

1. 시나리오 섹션에 &quot;Fusion Enablement Exercents&quot;라는 폴더를 만듭니다.
1. 폴더를 클릭한 다음 새 시나리오 만들기를 클릭합니다.

   ![초기 시나리오 디자인 이미지 2](../12-exercises/assets/initial-scenario-design-2.png)

1. 다음 페이지에서 Workfront을 검색하고 해당 앱을 선택합니다. 그런 다음 계속을 클릭합니다.
1. 시나리오 디자이너 화면의 왼쪽 상단에서 시나리오 이름을 &quot;초기 시나리오 디자인&quot;으로 바꿉니다.
1. 화면 중앙에 있는 빈 트리거 모듈을 클릭하고 Workfront 앱을 선택한 다음 문서 다운로드 모듈을 선택합니다.

   **Workfront 계정에 대한 모듈의 연결을 인증합니다.**

1. 연결을 처음 만들려면 추가 단추를 클릭합니다.

   ![초기 시나리오 디자인 이미지 3](../12-exercises/assets/initial-scenario-design-3.png)

1. 연결에 &quot;My Workfront 2020&quot;과 같은 이름을 지정합니다.

   ![초기 시나리오 디자인 이미지 4](../12-exercises/assets/initial-scenario-design-4.png)

1. URL 입력 **Workfront 인스턴스**&#x200B;을 클릭하고 다음 을 클릭합니다.

   ![초기 시나리오 디자인 이미지 5](../12-exercises/assets/initial-scenario-design-5.png)

1. 암호를 입력하고 로그인 을 클릭합니다.

   **연결이 설정됩니다. 이제 Workfront에서 다운로드할 문서의 문서 ID를 입력합니다.**

   ![초기 시나리오 디자인 이미지 7](../12-exercises/assets/initial-scenario-design-7.png)

1. Workfront으로 돌아갑니다. &quot;Fusion Exercise Files&quot; 폴더에서 &quot;_Fusion2020_Project List.csv&quot;를 선택하고 왼쪽 패널에서 문서 세부 정보(Document Details)를 클릭합니다. URL 주소에서 문서 ID 번호(URL에서 첫 번째 긴 번호)를 복사합니다.

   ![초기 시나리오 디자인 이미지 8](../12-exercises/assets/initial-scenario-design-8.png)

1. Fusion으로 돌아가서 문서 ID 필드에 번호를 붙여 넣고 [확인]을 클릭합니다.
1. 가장 좋은 방법은 모듈을 만들 때 모듈 이름을 바꾸는 것입니다. Workfront 모듈을 마우스 오른쪽 단추로 클릭하고 이름 바꾸기를 선택합니다. 모듈 이름을 &quot;프로젝트 목록 가져오기&quot;로 지정합니다.

   **이제 방금 다운로드한 CSV 파일을 구문 분석하여 파일의 각 행에 액세스할 수 있습니다. 각 행에서 프로젝트를 만들 때 이 정보를 사용합니다.**

1. Workfront 모듈의 오른쪽을 클릭하여 다른 모듈을 추가합니다. CSV 앱을 검색하고 CSV 구문 분석 모듈을 선택합니다.
1. 6개 열에 대한 CSV 구문 분석 을 설정하고 CSV에 헤더, 쉼표 구분 기호 유형을 포함하고 데이터를 CSV 필드에 넣습니다. 그런 다음 확인을 클릭합니다.

   ![초기 시나리오 디자인 이미지 9](../12-exercises/assets/initial-scenario-design-9.png)

1. 이 모듈의 이름을 &quot;프로젝트 목록 구문 분석&quot;으로 바꿉니다.
1. 시나리오 디자이너 하단에서 저장 을 클릭하여 시나리오를 저장합니다.
1. 실행 을 한 번 클릭하여 출력을 확인합니다.

   >[!NOTE]
   >
   >변환기가 마지막 모듈이 아니어야 한다는 경고를 무시합니다(true이지만 이 테스트에는 문제가 되지 않음). 실행을 클릭합니다.

   ![초기 시나리오 디자인 이미지 10](../12-exercises/assets/initial-scenario-design-10.png)

1. CSV 구문 분석 모듈에서 실행 관리자를 열어 모듈의 입력 및 출력을 확인합니다. 입력으로서 번들(CSV 파일)이 한 개 있고 출력으로서 번들(CSV 파일의 각 행에 대해 번들 한 개)이 여러 개 있습니다. 다음과 같이 표시되어야 합니다.

   ![초기 시나리오 디자인 이미지 11](../12-exercises/assets/initial-scenario-design-11.png)

   **CSV 파일의 각 행에 대한 프로젝트를 만드는 모듈을 추가합니다.**

1. 다른 모듈을 추가합니다. Workfront 앱을 선택하고 레코드 만들기 모듈을 선택합니다.
1. 레코드 유형을 프로젝트로 설정합니다.

   >[!TIP]
   >
   >다음과 같은 몇 가지 문자를 입력하여 검색합니다. *프로젝트*&#x200B;바로 이동하십시오.

1. 그런 다음 Cmd/Ctrl+G를 사용하여 이름(프로젝트 이름)을 찾습니다. 이름 옆에 있는 상자를 선택합니다. 필드가 아래에 나타납니다.
1. 이제 계획된 시작 일자 및 우선 순위 옆에 있는 상자를 선택합니다.
1. 매핑 패널이 나타나도록 이름 필드를 클릭합니다. CSV 구문 분석 모듈에서 열 1 필드를 클릭하여 이름 필드에 추가합니다. CSV 파일의 프로젝트 이름입니다.
1. 계획된 시작 일자에 대해 CSV 구문 분석 모듈에서 5열을 누릅니다.
1. 우선 순위의 경우 드롭다운 메뉴에서 일반 을 선택합니다.

   **매핑 패널은 다음과 같아야 합니다.**

   ![초기 시나리오 디자인 이미지 12](../12-exercises/assets/initial-scenario-design-12.png)

1. 확인을 클릭합니다.

   >[!NOTE]
   >
   >확인을 클릭하지 않고 실수로 디자이너를 다시 클릭하면 작업이 저장되지 않고 다시 매핑해야 합니다.

1. Workfront 모듈을 마우스 오른쪽 단추로 클릭하고 이름을 &quot;Workfront 프로젝트 만들기&quot;로 바꿉니다.
1. 시나리오를 저장하고 한 번 실행 버튼을 클릭합니다.
1. 마지막 모듈의 오른쪽 상단에 있는 실행 관리자를 클릭합니다.

   + 20개의 작업이 수행되었음을 알 수 있습니다. 각 작업은 CSV 파일에서 한 행을 의미하는 번들을 입력으로 취하여 한 번들을 출력했습니다. 이 번들은 Workfront에서 만든 프로젝트였습니다. 생성된 프로젝트의 프로젝트 ID가 출력 번들과 함께 표시됩니다.

   ![초기 시나리오 디자인 이미지 13](../12-exercises/assets/initial-scenario-design-13.png)

   **메모 사용**

1. 참고는 시나리오 설계에 대한 가시성을 높이는 데 도움이 됩니다. Workfront 프로젝트 만들기 모듈에 메모를 추가하려면 마우스 오른쪽 단추를 클릭하고 메모 추가를 선택합니다. 모듈에 메모를 추가할 수 있도록 디자이너 창의 오른쪽에 있는 패널이 팝업됩니다. &quot;CSV 파일에서 이름, 계획된 시작 일자 및 우선순위가 매핑된 프로젝트 만들기&quot;를 입력합니다.
1. 트리거 모듈(첫 번째 Workfront 모듈)이 수행하는 작업을 설명하는 다른 메모를 추가합니다.
1. 오른쪽 상단의 X를 클릭하여 메모 패널을 닫습니다.

   + 아래쪽 도구 모음에서 메모 버튼을 클릭하거나 모듈을 마우스 오른쪽 버튼으로 클릭하고 새 메모를 추가하여 메모에 다시 액세스합니다.
   + 음표는 역시간 순서로 정렬됩니다.
   + 메모가 추가되면 메모 단추에 주황색 점이 나타납니다.

   ![초기 시나리오 디자인 이미지 14](../12-exercises/assets/initial-scenario-design-14.png)

1. 컨트롤 도구 모음에서 저장 단추를 클릭하여 시나리오를 저장합니다.
1. Workfront 인스턴스에서 만든 프로젝트를 볼 수 있습니다.
