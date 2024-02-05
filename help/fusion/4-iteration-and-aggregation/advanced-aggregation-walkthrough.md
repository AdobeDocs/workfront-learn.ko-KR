---
title: 고급 집계 워크스루
description: ' [!DNL Adobe Workfront Fusion]에서 웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역별로 그룹화된 인구를 확인하는 방법을 알아봅니다.'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '278'
ht-degree: 100%

---

# 고급 집계 워크스루

웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역별로 그룹화된 모든 국가의 총 인구를 확인합니다.

![Fusion 시나리오의 이미지](assets/iteration-and-aggregation-3.png)

## 고급 집계 워크스루

Workfront에서는 연습 워크스루 비디오를 시청한 다음, 사용자 개인의 환경에서 연습 내용을 재현할 것을 권장합니다.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## 연습용 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>워크스루 완료에 대한 단계별 지침을 보려면 [고급 집계 워크스루](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=ko-KR)를 참조하십시오.

## 집계 원칙 강화

모듈이 여러 번들을 출력할 때마다 이후의 모든 모듈이 각 번들을 실행합니다.

이를 방지하려면 잠재적으로 여러 번들을 생성하는 모듈 뒤에 집계기를 추가합니다.

시나리오의 **시작-반복기**&#x200B;에서 **끝-집계기**&#x200B;까지 모든 세그먼트를 둘러싸는 그림자를 볼 수 있습니다. 이렇게 하면 Workfront Fusion 시나리오에서 해당 세그먼트를 쉽게 찾을 수 있습니다.

## 사용자 차례

>[!NOTE]
>
>실습 및 과제는 옵션이며 Fusion 교육을 완료하는 데 필수는 아닙니다.

이 실습은 워크스루에서 배운 내용을 기반으로 하나, 해결 방법은 제공되지 않습니다.

마케팅 포트폴리오의 프로젝트에서 작업에 로그온한 모든 시간을 합산하는 새 시나리오를 만듭니다. 그런 다음 “귀하의 {Project 이름} 프로젝트 팀이 총 {계획된 시간} 시간 중 {합산된 시간}을 기록하여 계획의 {백분율}에 도달했습니다”라는 이메일을 보냅니다.

**과제:** 올해 기록된 시간 동안만 동일한 작업을 수행할 수 있는지 확인합니다.

## 자세히 알아보고 싶으신가요? 다음을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=ko-KR)
