---
title: 고급 보고 시작
description: 사용 방법 알아보기 [!UICONTROL API 탐색기] 및 텍스트 모드를 통해 고급 필터, 보기 및 그룹화 만들기 [!UICONTROL 보고 UI].
activity: use
feature: Text Mode Reporting
thumbnail: 3409632.png
type: Tutorial
role: User
level: Experienced
team: Technical Marketing
jira: KT-11198
exl-id: 3baec042-1c1c-4075-b8ff-b1537758ef37
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 고급 보고 시작

사용 방법 알아보기 [[!UICONTROL API 탐색기]](https://developer.adobe.com/workfront/api-explorer/) 및 텍스트 모드를 통해 고급 필터, 보기 및 그룹화 만들기 [!UICONTROL 보고 UI].

세 가지 튜토리얼이 고급 보고를 구성합니다. 고급 보고 1, 2 및 3부 이를 합하면 5시간 33분의 교육이 이루어집니다.

비디오 외에 을(를) 다운로드합니다. [고급 보고 설명서](/help/assets/advanced-reporting-manual.pdf) 참고 및 연습을 위해.

**고급 보고 1부** 보고서 작성에 대한 검토 및 소개 [!UICONTROL API 탐색기] 및 텍스트 모드, 그리고 텍스트 모드 필터에 대한 심층 연구.

**고급 보고 2부** 텍스트 모드 보기, 텍스트 모드 구조에 대한 추가 세부 정보, 계산된 사용자 정의 데이터 및 계산된 열에 대한 심층적인 연구가 포함되어 있습니다.

**고급 보고 3부** 텍스트 모드 그룹화, 계산된 집계 및 계산된 그룹화에 대한 심층적인 연구가 포함되어 있습니다.

## 전제 조건

이 튜토리얼을 시청하기 전에 다음을 수행해야 합니다.

* Workfront 사용에 대한 적절한 이해. 이는 최소 3개월에서 6개월 동안 Workfront의 진지한 사용자였음을 의미합니다.
* 보고서에 포함할 객체를 잘 이해합니다.
* 사용자 정의 양식, 특히 계산된 사용자 정의 필드 사용에 대한 올바른 이해.
* A [!UICONTROL 플랜] 보고서 및 필터를 만들 수 있는 권한이 활성화된 라이선스 유형입니다.
* 다음을 실행했어야 합니다. [[!UICONTROL 기본 보고 요소]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-1-reporting.html) 과정, [[!UICONTROL 사용자 정의 보고서 및 대시보드 만들기]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-3-reporting.html) 강의 및 [[!UICONTROL 중간 필터 만들기]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-2-reporting.html) 당연하지

## Target 대상

이러한 자습서의 타겟 대상은 다음과 같습니다 [!UICONTROL 플랜] 현재 사용자 정의 보고서를 만들고 텍스트 모드를 사용하여 보고 사용자 인터페이스보다 더 많은 작업을 수행하는 방법을 알고 싶은 사용자에게 라이선스를 제공할 수 있습니다.

## 이 튜토리얼의 출처는 무엇입니까?

이 튜토리얼은 2018년 2월, 3일 동안 제공되는 라이브 클래스 녹화입니다. 비디오에서 이전 UI를 확인할 수 있지만, 이는 제공된 콘텐츠의 정확성이나 관련성에 영향을 미치지 않습니다.

또한 연습할 테스트 드라이브 계정을 가져오는 방법에 대한 몇 가지 언급도 들을 수 있습니다. Adobe Experience League은 테스트 드라이브 계정을 제공하지 않지만 걱정하지 마십시오. 프로덕션 계정에서 연습할 수 있습니다. 결국, 보고는 Workfront에서 개체를 보는 것이지 개체를 만들거나 삭제하는 것이 아닙니다. 물론 보고서를 직접 작성하는 것만 제외하고 나머지 작업은 수행할 수 있습니다. 그러나 시스템 관리자 외에 사용자가 만든 보고서를 공유하지 않으면 해당 보고서를 볼 수 있는 사람은 귀하뿐입니다.
