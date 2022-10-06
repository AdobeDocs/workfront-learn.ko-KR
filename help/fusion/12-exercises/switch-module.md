---
title: 스위치 모듈
description: 보다 복잡하거나 동적 데이터 변환을 수행해야 할 때 스위치 모듈을 사용하는 방법을 이해합니다.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11052
thumbnail: KT11052.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# 스위치 모듈

보다 복잡하거나 동적 데이터 변환을 수행해야 할 때 스위치 모듈을 사용하는 방법을 이해합니다.

## 연습 개요

테스트 드라이브에서 DM 프로젝트를 검색한 다음 프로젝트에 첨부된 사용자 지정 필드에서 선택한 값을 기준으로 각 프로젝트의 이름을 변경합니다.

![스위치 모듈 이미지 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## 수행할 단계

1. 새 시나리오를 만들고 이름을 &quot;스위치 모듈 사용&quot;으로 지정합니다.
1. 트리거 모듈의 경우 Workfront 검색 모듈을 사용합니다.
1. Workfront 연결을 설정하고 레코드 유형을 Project로 설정합니다.
1. 검색 기준에서 채널 사용자 지정 필드에 값이 있는 프로젝트만 표시하도록 지정합니다.
1. 출력에 대해 ID, 이름, 참조 번호 및 채널 사용자 지정 필드를 선택합니다.

   ![스위치 모듈 이미지 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. 도구에서 스위치 모듈을 추가합니다.
1. 입력 필드의 경우 검색 모듈에서 채널 사용자 지정 필드를 매핑합니다.

   ![스위치 모듈 이미지 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. 채널 사용자 지정 필드에서 발생할 수 있는 각 값에 대해 다음 추가 사례를 추가합니다. 가능한 값은 패턴 필드에 있습니다. 출력 필드에 특정 3자 코드와 프로젝트 참조 번호, 프로젝트 이름을 포함하게 합니다.

   **매핑 패널은 다음과 같아야 합니다.**

   ![스위치 모듈 이미지 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. 원하는 수만큼 추가 사례를 추가할 수 있습니다. 맨 아래에 Else 필드가 있습니다. 입력 값이 대/소문자를 구분하지 않는 경우에 사용됩니다.

   **Workfront에서 프로젝트 이름을 업데이트합니다.**

   ![스위치 모듈 이미지 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Workfront 업데이트 레코드 모듈을 추가합니다.
1. ID 필드에서 트리거 모듈의 ID에 매핑합니다.
1. 레코드 유형을 프로젝트로 설정합니다.
1. 매핑할 필드 선택 섹션에서 이름 필드를 선택하고 스위치 모듈의 출력에 매핑합니다.
1. 시나리오를 저장하고 한 번 실행합니다. 테스트 드라이브에서 업데이트된 프로젝트 이름을 봅니다.
