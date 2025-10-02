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
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 90%

---

# 고급 집계 워크스루

웹 서비스를 호출하여 여러 국가에 대한 세부 정보를 반환하고 하위 지역별로 그룹화된 모든 국가의 총 인구를 확인합니다.

![Fusion 시나리오의 이미지](assets/iteration-and-aggregation-3.png)

## 고급 집계 워크스루

Workfront에서는 연습 워크스루 비디오를 시청한 다음, 사용자 개인의 환경에서 연습 내용을 재현할 것을 권장합니다.

>[!VIDEO](https://video.tv.adobe.com/v/3417306/?quality=12&learn=on&enablevpops=1&captions=kor)

## 연습용 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## 집계 원칙 강화

모듈이 여러 번들을 출력할 때마다 이후의 모든 모듈이 각 번들을 실행합니다.

이를 방지하려면 잠재적으로 여러 번들을 생성하는 모듈 뒤에 집계기를 추가합니다.

시나리오의 **시작-반복기**&#x200B;에서 **끝-집계기**&#x200B;까지 모든 세그먼트를 둘러싸는 그림자를 볼 수 있습니다. 이렇게 하면 Workfront Fusion 시나리오에서 해당 세그먼트를 쉽게 찾을 수 있습니다.

## 사용자 차례

>[!NOTE]
>
>실습 및 과제는 옵션이며 Fusion 교육을 완료하는 데 필수는 아닙니다.

이 실습은 워크스루에서 배운 내용을 기반으로 하나, 해결 방법은 제공되지 않습니다.

마케팅 포트폴리오의 프로젝트에서 작업에 로그온한 모든 시간을 합산하는 새 시나리오를 만듭니다. 그런 다음 &quot;내 {Project Name} 프로젝트 팀이 계획된 총 {summed hours}시간 중 {planned hours}시간을 기록하여 플랜의 {percentage}을(를) 달성했습니다.&quot;라는 전자 메일을 보냅니다.

**과제:** 올해 기록된 시간 동안만 동일한 작업을 수행할 수 있는지 확인합니다.

## 자세히 알아보고 싶으신가요? 다음 자료를 참조하십시오.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
