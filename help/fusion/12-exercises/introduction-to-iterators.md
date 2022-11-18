---
title: 반복기 소개
description: 반복 방식의 앱을 사용하고 각 정보 번들에 대해 작업을 수행하는 방법을 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 반복기 소개

반복 방식의 앱을 사용하고 각 정보 번들에 대해 작업을 수행하는 방법을 알아봅니다.

## 연습 개요

Workfront에서 특정 프로젝트를 보고 해당 프로젝트 내의 모든 작업을 확인합니다. 증분 도구 모듈을 사용하여 프로젝트 내의 작업 수를 계산합니다. 마지막으로, 변수 설정 모듈을 사용하여 개설 문제 수에서 하위 수를 빼서 각 작업 번들에 대한 숫자 값을 생성합니다.

![반복기 이미지 1 소개](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## 수행할 단계

**프로젝트 및 관련 작업을 읽어 보십시오.**

1. 새 시나리오를 시작합니다. 이름을 &quot;반복 소개&quot;로 지정합니다.
1. Workfront을 트리거 모듈로 선택하고 레코드 읽기를 선택합니다.
1. 레코드 유형에 대해 프로젝트를 선택합니다.
1. 출력에 대해 ID, 이름 및 설명을 선택합니다.
1. ID 필드에 Workfront 테스트 드라이브 인스턴스에서 Northstar Fashioning Extender Booth 프로젝트의 프로젝트 ID를 넣습니다.
1. 이 모듈 이름을 &quot;WF 프로젝트 찾기&quot;로 바꾸십시오.
1. 다른 Workfront 모듈을 추가하여 이 프로젝트와 관련된 작업을 읽습니다. 관련 레코드 읽기 모듈을 선택합니다.
1. 레코드 유형에 대해 프로젝트를 선택합니다.
1. 상위 레코드 ID의 경우 레코드 읽기 모듈에서 ID를 선택합니다.
1. 컬렉션에서 작업을 선택합니다.
1. 출력에 대해 ID, 이름, 설명, 하위 수, 미해결 문제 수 및 작업을 선택합니다.
1. 이 모듈의 이름을 &quot;프로젝트 작업 읽기&quot;로 바꿉니다.
1. 시나리오를 저장한 다음 실행 을 한 번 클릭하여 출력을 확인합니다.

   + 실행 관리자를 클릭하면 한 번들을 입력(프로젝트)으로 표시하고 28개의 번들을 출력(작업)으로 볼 수 있습니다.

   **카운트 및 프로세스 반복 번들.**

1. 관련 레코드 읽기 후에 다른 모듈을 추가합니다. 증분 함수 도구 모듈을 선택합니다.

   + 값 재설정 필드를 사용 안 함으로 두고 확인 을 클릭합니다.

1. 이 모듈의 이름을 &quot;작업 수 계산&quot;으로 바꿉니다.
1. 변수 설정 모듈을 추가합니다. 변수 이름을 &quot;Random Math&quot;로 설정합니다.
1. 변수 값 필드에서 열린 opTasks 수에서 열린 1차 하위 구성요소 수를 뺀 것입니다.

   **다음과 같이 표시되어야 합니다.**

   ![반복기 이미지 2 소개](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. 이 모듈의 이름을 &quot;Random Math&quot;로 변경합니다.
1. 시나리오를 저장하고 실행 을 한 번 클릭합니다.

Read Related Records Interperator 모듈에서 생성한 각 작업에 대해 Workfront Fusion이 28개의 실행을 수행했습니다. 이러한 28 번들은 루프를 닫기 위해 집계를 추가하지 않는 한 시나리오 전체에서 계속 처리됩니다.
