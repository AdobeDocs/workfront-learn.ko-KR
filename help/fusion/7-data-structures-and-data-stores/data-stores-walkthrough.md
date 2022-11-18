---
title: 데이터 저장소 연습
description: 를 사용하여 회사 목록과 Workfront 간에 회사 이름을 동기화하는 데 데이터 저장소를 사용하는 방법을 알아봅니다 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 데이터 저장소 연습

## 개요

이 연습에서는 데이터 저장소를 사용하여 회사 목록과 Workfront 간에 회사 이름을 동기화합니다.

이는 Workfront과 일부 다른 시스템에서 회사의 일방향 동기화의 한 부분입니다. 지금은 CSV 파일과 Workfront 사이에만 동기화됩니다. 그러나 데이터 저장소에도 테이블이 유지되어 각 회사의 CSV 파일(CID)로 Workfront ID(WFID)와 회사 ID를 추적합니다. 이를 통해 미래의 어느 시점에서 양방향 동기화를 수행할 수 있습니다.

![Fusion 시나리오의 이미지](assets/data-structures-and-data-stores-2.png)

## 데이터 저장소 연습

Workfront에서는 자체 환경에서 연습을 다시 시도하기 전에 연습 연습 연습 비디오 를 시청하는 것이 좋습니다.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>이 연습을 완료하는 방법에 대한 단계별 지침은 [데이터 저장소 연습](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) 운동.


## 최종 참고 사항

이제 데이터 구조와 데이터 저장소에 대해 학습이 끝났기 때문에 &quot;언제 사용해야 합니까?&quot;라고 자문할 수 있습니다.

데이터 구조는 JSON, XML, CSV 등과 같은 데이터 형식을 직렬화 또는 구문 분석하는 데 가장 일반적으로 사용됩니다. 데이터 구조를 사용하면 데이터 구조를 제어하고 데이터를 확인할 수 있습니다. 데이터 구조를 사용하는 가장 일반적인 이유는 JSON 또는 XML이 필요한 API로 전송할 유효한 데이터를 만드는 것입니다. 이러한 경우 데이터 구조와 함께 JSON 또는 XML 앱을 사용하여 데이터가 올바른 포맷인지 확인해야 합니다.

데이터 저장소는 두 개 이상의 시나리오 실행에서 액세스해야 하는 영구 데이터를 저장하는 데만 사용해야 합니다. 예를 들어, 고급 사용 사례에 대해 처리된 마지막 레코드에 대한 메타데이터를 저장할 수 있으며, 처리를 정밀하게 제어해야 합니다.

데이터 저장소는 Data Warehouse 또는 로깅으로 사용하도록 설계되지 않았습니다. Workfront Fusion 외부에서 데이터 저장소는 액세스할 수 없으며, 대부분의 데이터 저장소는 Workfront Fusion 시나리오를 통해 액세스할 수 있습니다. 따라서 데이터 웨어하우스 및 로깅 사용 사례에 필요한 분석 또는 보고 도구에 데이터 저장소를 연결할 수 없습니다. 이러한 사용 사례에서 Workfront Fusion의 역할은 데이터를 구성하고 저장하는 데 적합한 시스템(예: SQL, MariaDB)을 채우는 것입니다.

## 자세한 내용 다음 사항을 권장합니다.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
