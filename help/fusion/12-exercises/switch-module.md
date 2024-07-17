---
title: 전환 모듈 연습
description: 더 복잡하거나 동적인 데이터 변환을 수행해야 하는 경우, 전환 모듈을 사용하는 방법을 이해합니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
recommendations: noDisplay,noCatalog
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 100%

---

# 전환 모듈 연습

더 복잡하거나 동적인 데이터 변환을 수행해야 하는 경우, 전환 모듈을 사용하는 방법을 이해합니다.

## 연습 개요

테스트 드라이브에서 다이렉트 메일 프로젝트를 검색한 다음 프로젝트에 연결된 사용자 정의 필드에서 선택한 값을 기반으로 각 프로젝트의 이름을 변경합니다.

![전환 모듈 이미지 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## 따라야 할 단계

1. 새 시나리오를 만들고 이름을 “전환 모듈 사용”으로 지정합니다.
1. 트리거 모듈의 경우 Workfront 검색 모듈을 사용합니다.
1. Workfront 연결을 설정하고 레코드 유형을 ‘프로젝트’로 설정합니다.
1. ‘검색 기준’에서 ‘채널’ 사용자 정의 필드에 값이 있는 프로젝트만 표시되도록 지정합니다.
1. 출력의 경우 ‘ID’, ‘이름’, ‘참조 번호’ 및 ‘채널’ 사용자 정의 필드를 선택합니다.

   ![전환 모듈 이미지 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. ‘도구’에서 스위치 모듈을 추가합니다.
1. ‘입력’ 필드의 경우 검색 모듈에서 ‘채널’ 사용자 정의 필드를 매핑합니다.

   ![전환 모듈 이미지 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. 다음으로 ‘채널’ 사용자 정의 필드에서 오는 각 가능한 값에 대한 사례를 추가합니다. 가능한 값은 ‘패턴’ 필드에 있습니다. 출력 필드에 특정 3자 코드, 프로젝트 참조 번호, 프로젝트 이름을 순서대로 포함시키고자 합니다.

   **매핑 패널은 다음과 같아야 합니다.**

   ![전환 모듈 이미지 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. 필요에 따라 여러 추가 사례를 추가할 수 있습니다. 하단에는 ‘기타’ 필드가 있습니다. 입력 값이 어떤 사례와도 일치하지 않는 경우에 이 필드를 사용합니다.

   **Workfront에서 프로젝트 이름을 업데이트합니다.**

   ![전환 모듈 이미지 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Workfront 레코드 업데이트 모듈을 추가합니다.
1. ‘ID’ 필드에서 트리거 모듈의 ID에 매핑합니다.
1. ‘레코드 유형’을 ‘프로젝트’로 설정합니다.
1. ‘매핑할 필드 선택’ 섹션에서 ‘이름’ 필드를 선택하고 전환 모듈의 출력에 매핑합니다.
1. 시나리오를 저장하고 ‘한 번 실행’을 진행합니다. 테스트 드라이브에서 업데이트된 프로젝트 이름을 봅니다.
