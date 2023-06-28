---
title: 데이터 저장소
description: 두 시스템 간에 회사 이름을 동기화하는 방법을 알아봅니다. (60~160자 사이여야 하지만 59자임)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# 데이터 저장소

두 시스템 간에 회사 이름을 동기화하는 방법을 알아봅니다.

## 연습 개요

이는 Workfront과 다른 시스템의 회사 간 단방향 동기화의 첫 번째 부분입니다. 현재는 Fusion 데이터 저장소와 Workfront 간에만 동기화됩니다. 데이터 저장소의 테이블은 각 회사에 대한 CSV 파일(CID)에서 Workfront ID(WFID)와 회사 ID를 추적합니다. 이렇게 하면 미래의 어느 시점에서 양방향 동기화가 가능합니다.

![데이터 저장소 이미지 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## 따라야 할 단계

**Workfront에서 파일을 다운로드합니다.**

1. Workfront &quot;Fusion Exercise Files&quot; 폴더에서 &quot;_Companies.csv&quot;를 선택하고 문서 세부 정보 를 클릭합니다.
1. URL 주소에서 첫 번째 ID 번호를 복사합니다.
1. Fusion에서 &quot;데이터 저장소를 사용하여 데이터 동기화&quot;라는 새 시나리오를 만듭니다.
1. 트리거 모듈의 경우, Workfront 다운로드 문서 모듈을 선택합니다.
1. Workfront 연결을 설정하고 Workfront URL에서 복사한 문서 ID를 포함합니다.
1. 이 모듈의 이름을 &quot;회사 파일 가져오기&quot;로 지정합니다.
1. 이제 CSV 구문 분석 모듈을 추가합니다.
1. 열 개수 필드에 2를 입력합니다.
1. 다운로드 문서 모듈의 데이터를 CSV 필드에 매핑합니다.
1. 이 모듈의 이름을 &quot;회사 파일 구문 분석&quot;으로 지정합니다.
1. 시나리오를 저장하고 실행 을 한 번 클릭합니다.

   **데이터 저장소 및 데이터 구조를 만듭니다.**

1. 데이터 저장소 검색 레코드 모듈을 추가합니다.
1. &quot;회사 동기화&quot;라는 새 데이터 저장소를 만듭니다.
1. 데이터 저장소 내에서 &quot;Company sync(struc)&quot;라는 데이터 구조를 만듭니다.
1. 4개의 필드를 만듭니다.

   + CID - CSV 파일의 회사 ID
   + 회사 이름
   + WFID - Workfront 회사 ID
   + 만든 날짜 - 데이터 유형이 날짜인지 확인합니다.

   ![데이터 저장소 이미지 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. 데이터 구조에서 저장 을 클릭한 다음 데이터 저장소 크기를 1로 설정하고 데이터 저장소를 저장합니다.
1. 데이터 저장소 모듈에서 계속하여 CID가 구문 분석 CSV 모듈(1열)의 회사 ID와 동일한 필터를 설정합니다.
1. 고급 설정 표시 를 클릭하고 옵션을 선택하여 &quot;이 모듈이 결과 없이 반환되더라도 시나리오 또는 경로의 실행을 계속합니다.&quot;를 선택합니다.

   ![데이터 저장소 이미지 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. 이 모듈의 이름을 &quot;Matching companies&quot;로 바꿉니다.
1. Workfront 검색 레코드 모듈을 추가합니다.
1. 레코드 유형으로 회사를 선택합니다.
1. 검색 기준은 Workfront 내의 회사 이름이 CSV 파일의 회사 이름과 같다는 것입니다.
1. 출력의 경우 회사 이름과 ID를 선택합니다.

   ![데이터 저장소 이미지 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. 확인 을 클릭하고 이 모듈의 이름을 &quot;Matching companies&quot;로 변경합니다.

   **회사가 Workfront 또는 데이터 저장소 내에 존재하는지 여부에 따라 다른 경로를 만듭니다.**

   **라우팅 경로 1 - 회사를 만듭니다.**

1. Workfront 검색 레코드 모듈 오른쪽에 라우터 모듈을 추가합니다.
1. 상단 경로에 Workfront 레코드 만들기 모듈을 추가합니다.
1. 레코드 종류를 회사로 설정합니다.
1. 매핑할 필드에서 이름 을 선택합니다. 이름 필드를 CSV 구문 분석 모듈의 출력에 매핑합니다(2열).
1. 이 모듈의 이름을 &quot;회사 만들기&quot;로 바꿉니다.

   ![데이터 저장소 이미지 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. 아직 Workfront에 없는 경우에만 회사를 만들려면 라우터 뒤에 필터를 추가하십시오. 이름을 &quot;Workfront에 없음&quot;으로 지정합니다.
1. 조건을 Workfront 검색 모듈의 ID로 설정하고 이(가) 없습니다.

   ![데이터 저장소 이미지 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **다음 경로에서 데이터 저장소 업데이트를 준비합니다.**

1. 상단 경로 끝에 변수 설정 모듈을 추가합니다.
1. 변수 이름을 &quot;Workfront ID&quot;로 설정합니다.
1. 변수 값을 회사 만들기 모듈에서 ID로 설정합니다.
1. 이 모듈의 이름을 &quot;Workfront ID 설정&quot;으로 바꿉니다.

   **라우팅 경로 2 - 데이터 저장소를 업데이트합니다.**

1. 라우팅 경로 2에 필터를 만듭니다. 이름을 &quot;데이터 저장소에 없음&quot;으로 지정합니다.

1. 조건을 데이터 저장소 모듈의 키로 설정하고 이(가) 없습니다.

   ![데이터 저장소 이미지 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. 이 경로의 첫 번째 모듈은 변수 가져오기 모듈입니다.
1. 변수 이름을 &quot;Workfront ID&quot;로 설정합니다.
1. 이 모듈의 이름을 &quot;Workfront ID 가져오기&quot;로 바꿉니다.
1. 데이터 스토어 앱에서 다른 모듈을 추가하고, 레코드를 추가/바꿉니다.
1. 데이터 저장소 필드에서 회사 동기화를 선택합니다. 이전에 만든 데이터 저장소입니다.
1. 키 필드를 비워 둡니다.
1. CSV 구문 분석 모듈의 열 1에 있는 CID 필드를 매핑합니다.
1. CSV 구문 분석 모듈의 열 2에 있는 회사 이름 필드를 매핑합니다.
1. Workfront ID 가져오기 모듈에서 WFID 필드를 매핑합니다.
1. 만든 날짜 필드의 경우 날짜 및 시간 탭에서 formatDate 함수를 사용하여 현재 날짜의 형식을 YYYY/MM/DD로 지정합니다.

   ![데이터 저장소 이미지 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. 확인 을 클릭하고 이 모듈의 이름을 &quot;회사 항목 만들기&quot;로 바꿉니다.

   **라우팅 경로 3-시스템 간에 데이터 저장소를 동기화합니다.**

1. 먼저 라우팅 경로 3에 필터를 만듭니다. 이름을 &quot;Company exists, not in data store.&quot;로 지정합니다.
1. 데이터 저장소 검색 레코드 모듈에서 조건을 키로 설정하고 이(가) 없습니다.
1. AND 규칙 추가 단추를 클릭하고 CSV 파일(2열)의 회사 이름이 Workfront 검색 모듈에 있는 회사의 이름과 같도록 지정합니다.

   ![데이터 저장소 이미지 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. 이제 라우팅 경로 2의 끝에 있는 레코드 모듈을 복제하여 다른 레코드 추가/바꾸기를 추가합니다.
1. 복제된 모듈을 라우팅 경로 3 끝에 있는 위치로 드래그합니다. 거기에 있었던 빈 모듈을 삭제합니다.
1. 복제된 모듈을 클릭합니다. WFID 필드를 제외한 모든 필드는 동일하게 유지되어야 합니다. 일치 회사 검색 모듈에서 매핑합니다.

   ![데이터 저장소 이미지 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. 확인 을 클릭하고 이 모듈의 이름을 &quot;회사 항목 만들기&quot;로 바꿉니다.
