---
title: 고급 보고 시작
description: 사용 방법을 알아봅니다 [!UICONTROL API 탐색기] 및 텍스트 모드를 사용하여 [!UICONTROL 보고 UI].
activity: use
feature: Reports and Dashboards
thumbnail: 3409632.png
type: Tutorial
role: User
level: Experienced
team: Technical Marketing
kt: 11198
source-git-commit: e2b5115d03e0eaa47cba3397b0aeb01044441083
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 고급 보고 시작

사용 방법을 알아봅니다 [[!UICONTROL API 탐색기]](https://developer.adobe.com/workfront/api-explorer/) 및 텍스트 모드를 사용하여 [!UICONTROL 보고 UI].

3개의 자습서가 고급 보고를 구성합니다. 고급 보고 부품 1, 2 및 3입니다. 합하면 5시간 33분 훈련한다.

비디오 외에 [고급 보고 설명서](/help/assets/advanced-reporting-manual.pdf) 참조 및 연습용.

**고급 보고 파트 1** 에는 보고서 작성 검토, [!UICONTROL API 탐색기] 텍스트 모드 및 텍스트 모드 필터에 대한 심층적인 연구

**고급 보고 파트 2** 텍스트 모드 보기에 대한 심도 있는 연구, 텍스트 모드 구조에 대한 자세한 내용, 계산된 사용자 지정 데이터 및 계산된 열을 포함합니다.

**고급 보고 파트 3** 텍스트 모드 그룹화, 계산된 집계 및 계산된 그룹에 대한 심층적인 연구를 포함합니다.

## 전제 조건

이러한 자습서를 시청하기 전에 다음을 수행해야 합니다.

* Workfront 사용에 대한 이해. 즉, 최소 3~6개월 동안 심각한 Workfront 사용자였습니다.
* 보고서에 포함할 개체를 잘 이해합니다.
* 사용자 지정 양식 사용, 특히 계산된 사용자 지정 필드를 잘 이해합니다.
* A [!UICONTROL 계획] 보고서 및 필터를 만들 수 있는 권한이 있는 라이선스 유형입니다.
* 이 파일을 가져와야 합니다. [[!UICONTROL 기본 보고 요소]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-1-reporting.html) 물론, [[!UICONTROL 사용자 지정 보고서 및 대시보드 만들기]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-3-reporting.html) 교육 과정 및 [[!UICONTROL 중간 필터 만들기]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-2-reporting.html) 물론이죠.

## Target 대상

이러한 자습서의 target 대상은 다음과 같습니다 [!UICONTROL 계획] 현재 사용자 지정 보고서를 만들고 보고 사용자 인터페이스보다 더 많은 작업을 수행하기 위해 텍스트 모드를 사용하는 방법을 알고 싶은 사용자를 라이선스 사용자.

## 이러한 자습서는 어디에서 제공됩니까?

이 자습서는 2018년 2월에 3일 동안 제공되는 라이브 클래스 레코딩입니다. 비디오에서 이전 UI를 볼 수 있지만, 제공된 컨텐츠의 정확성이나 관련성에 영향을 주지 않습니다.

에서 연습할 테스트 드라이브 계정을 가져오는 데 대한 참조 정보도 표시됩니다. Adobe Experience League은 테스트 드라이브 계정을 제공하지 않지만 걱정하지 마십시오. 프로덕션 계정에서는 연습할 수 있습니다. 마지막으로, 보고란 개체를 만들거나 삭제하는 것이 아니라 Workfront에서 개체를 보는 것에 대한 것입니다. 물론 보고서를 만들 필요는 없습니다. 그러나 시스템 관리자 외에 사용자가 보고서를 공유하기로 결정하지 않는 한 작성한 보고서를 볼 수 있는 유일한 사용자입니다.

