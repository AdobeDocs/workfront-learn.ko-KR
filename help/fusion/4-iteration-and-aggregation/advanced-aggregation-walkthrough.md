---
title: 고급 집계 워크스루
description: 웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역별로 그룹화된 모집단을 식별하는 방법을 알아봅니다. [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# 고급 집계 워크스루

## 개요

웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역으로 그룹화된 모든 국가의 총 인구를 식별합니다.

![Fusion 시나리오의 이미지](assets/iteration-and-aggregation-3.png)

## 고급 집계 워크스루

Workfront에서는 연습 연습 비디오를 시청한 후 자신의 환경에서 연습을 다시 만들 것을 권장합니다.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## 운동 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>이 연습을 완료하는 방법에 대한 단계별 지침은 [고급 집계 워크스루](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) 연습.

## 응집 원리의 강화

모듈이 여러 번들을 출력할 때마다 그 이후의 모든 모듈은 각 번들을 실행합니다.

이를 방지하려면 잠재적으로 여러 번들을 생성하는 모듈 뒤에 집계를 추가합니다.

시나리오에서 세그먼트 주위의 그림자를 볼 수 있습니다. **시작 반복자** (으)로 **종료 집계**. 이렇게 하면 Workfront Fusion 시나리오에서 이러한 세그먼트를 쉽게 찾을 수 있습니다.

## 당신 차례입니다

>[!NOTE]
>
>연습 연습과 과제는 선택 사항이며 Fusion 교육을 완료하는 데 필요하지 않습니다.

이 연습 연습은 연습에서 배운 내용을 기반으로 하지만 해결 방법은 제공되지 않습니다.

마케팅 포트폴리오의 프로젝트에서 로그온한 모든 시간을 합산하는 새 시나리오를 만듭니다. 그런 다음 &quot;{Project Name} 프로젝트 팀이 총 {planned hours} 계획 시간 중 {summit hours}을 기록하여 플랜의 {percentage}에 배치했습니다.&quot;라는 이메일을 보내십시오.

**과제:** 올해에 기록된 시간만 제외하고 동일한 작업을 수행할 수 있는지 확인하십시오.

## 자세히 알아보시겠습니까? 다음 사항을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
