---
title: 전환 함수
description: 전환 함수를 사용하여 전환 기능을 사용하는 방법에 대해 알아봅니다.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '234'
ht-degree: 100%

---

# 전환 함수

전환 함수를 사용하여 전환 기능을 사용하는 방법에 대해 알아봅니다.

## 연습 개요

간단한 데이터 변경의 경우, 전환 함수를 사용하여 모듈 필드 내에서 하나의 값을 다른 값으로 변환합니다. 이 연습에서는 두 글자로 된 키를 이메일로 보낼 프로젝트 진행 상태의 실제 이름으로 변경합니다.

![전환 함수 이미지 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 따라야 할 단계

1. “라우팅 경로 간 변수 공유”라는 시나리오를 복제합니다.
1. 새 시나리오의 이름을 “라우팅 경로 간 변수 공유 - 전환”으로 지정합니다.
1. 트리거 모듈을 클릭하고 출력 섹션에 진행 상태를 추가합니다.
1. 이메일 보내기 모듈에서 콘텐츠 필드에 진행 상태를 추가합니다.

   + 검색 모듈에서 들어오는 값을 매핑하면 진행 상태에 대한 두 글자로 된 코드가 표시됩니다.
   + 가능한 각 진행 상태의 전체 이름에 대한 코드를 “전환”하려면 일반 기능 탭에서 “전환” 함수를 사용합니다.

1. 전환 함수는 진행 상태 값 또는 표현식을 키로 사용한 다음, 해당 키를 기반으로 출력 값을 반환합니다.

   + 키 값은 두 번째 위치(“Late”)에서 정의된 해당 출력과 함께 진행 상태(“LT”) 뒤의 첫 번째 위치에서 정의됩니다.
   + 다음 키 값은 원하는 만큼 많은 키에 대해 세 번째 위치에 정의되고 해당 출력은 네 번째 위치에 정의됩니다.

     ![전환 함수 이미지 2](../12-exercises/assets/switch-function-walkthrough-2.png)
