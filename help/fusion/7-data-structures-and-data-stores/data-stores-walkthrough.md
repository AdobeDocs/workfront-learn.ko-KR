---
title: 데이터 저장소 워크스루
description: ' [!DNL Adobe Workfront Fusion]을 사용하여 회사 목록과 Workfront 간에 회사 이름을 동기화하기 위해 데이터 저장소를 사용하는 방법을 알아봅니다.'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 데이터 저장소 워크스루

이 연습에서는 데이터 저장소를 사용하여 회사 목록과 Workfront 간에 회사 이름을 동기화합니다.

Workfront 및 일부 다른 시스템에 있는 회사를 단방향 동기화하는 작업의 일부분입니다. 현재 CSV 파일과 Workfront 간에만 동기화됩니다. 그러나 각 회사의 CSV 파일(CID)에서 Workfront ID(WFID)와 회사 ID를 추적하는 데이터 저장소의 테이블도 유지 관리됩니다. 이를 통해 향후 어느 시점에서 양방향 동기화로 만들 수 있습니다.

![Fusion 시나리오의 이미지](assets/data-structures-and-data-stores-2.png)

## 데이터 저장소 워크스루

Workfront에서는 연습 워크스루 비디오를 시청한 다음, 사용자 개인의 환경에서 연습 내용을 재현할 것을 권장합니다.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on)



## 최종 참고 사항

데이터 구조 및 데이터 저장소에 대한 학습을 마친 지금, “언제 사용해야 할까?”라는 질문을 할 수 있습니다.

데이터 구조는 JSON, XML, CSV 등과 같은 데이터 형식을 직렬화하거나 구문 분석하는 데 가장 일반적으로 사용됩니다. 데이터 구조를 통해 데이터의 구조를 제어하고 나아가 데이터를 검증할 수 있습니다. 데이터 구조를 사용하는 가장 일반적인 이유는 JSON 또는 XML을 예상하는 API로 보낼 유효한 데이터를 만들기 위해서입니다. 이러한 경우 데이터가 올바른 형식인지 확인하기 위해 데이터 구조와 함께 JSON 또는 XML 앱을 사용할 수 있습니다.

데이터 저장소는 둘 이상의 시나리오 실행에서 액세스해야 하는 영구 데이터를 저장하는 데만 사용해야 합니다. 예를 들어 처리를 정밀하게 제어해야 하는 고급 사용 사례를 위해 처리된 마지막 레코드에 대한 메타데이터를 저장할 수 있습니다.

데이터 저장소는 데이터 웨어하우스 또는 로깅 용도로 설계되지 않았습니다. 데이터 저장소는 Workfront Fusion 외부에서 액세스할 수 없으며 데이터 저장소와의 상호 작용 중 대부분은 Workfront Fusion 시나리오를 통해 이루어집니다. 결과적으로 데이터 웨어하우스 및 로깅 사용 사례에 대해 예상되는 분석 또는 보고 도구에 데이터 저장소를 연결할 수 없습니다. 이와 같은 사용 사례에서 Workfront Fusion의 역할은 데이터(예: SQL, MariaDB)를 구성하고 저장하는 데 적합한 시스템을 채우는 것입니다.

## 자세히 알아보고 싶으신가요? 다음 자료를 참조하십시오.

[Workfront Fusion 설명서](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=ko-KR)
