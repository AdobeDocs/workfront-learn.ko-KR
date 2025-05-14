---
title: 고급 보고 소개
description: '[!UICONTROL API Explorer] 및 텍스트 모드를 사용하여 [!UICONTROL 보고 UI]의 기능을 능가하는 고급 필터, 보기 및 그룹화를 만드는 방법에 대해 알아봅니다.'
activity: use
feature: Reports and Dashboards
thumbnail: 3409632.png
type: Tutorial
role: User
level: Experienced
team: Technical Marketing
jira: KT-11198
exl-id: 3baec042-1c1c-4075-b8ff-b1537758ef37
source-git-commit: f03518b568cc24ad39b32f6dbfd763400529cf0f
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 100%

---

# 고급 보고 소개

[[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/) 및 텍스트 모드를 사용하여 [!UICONTROL 보고 UI]의 기능을 능가하는 고급 필터, 보기 및 그룹화를 만드는 방법에 대해 알아봅니다.

고급 보고는 세 가지 튜토리얼로 구성되어 있습니다. 바로 고급 보고 1부, 2부 및 3부입니다. 모두 합쳐 5시간 33분의 교육으로 구성됩니다.

비디오 외에도 [고급 보고 매뉴얼](/help/assets/advanced-reporting-manual.pdf)을 다운로드하여 참조 및 연습에 활용할 수 있습니다.

**고급 보고 1부**&#x200B;에는 보고서 작성 검토, [!UICONTROL API Explorer] 및 텍스트 모드 소개, 텍스트 모드 필터에 대한 심층 연구에 대해 나와 있습니다.

**고급 보고 2부**&#x200B;에는 텍스트 모드 보기에 대한 심층 연구, 텍스트 모드 구조에 대한 추가 세부 정보, 계산된 사용자 정의 데이터 및 계산된 열에 대해 나와 있습니다.

**고급 보고 3부**&#x200B;에는 텍스트 모드 그룹화, 계산된 집계 및 계산된 그룹화에 대한 심층 연구에 대해 나와 있습니다.

## 전제 조건

이 튜토리얼을 시청하기 전에 다음을 갖추어야 합니다.

* Workfront 사용에 대해 숙지합니다. 이는 적어도 3~6개월 동안 열성적인 Workfront 사용자였음을 의미합니다.
* 보고서에 포함하려는 오브젝트에 대해 숙지합니다.
* 사용자 정의 양식, 특히 계산된 사용자 정의 필드 사용에 대해 숙지합니다.
* 보고서 및 필터를 활성화하는 권한이 있는 [!UICONTROL 플랜] 라이선스 유형입니다.
* 지금까지 다음과 같은 과정을 수료하셨습니다.
   * [[!UICONTROL 기본 보고 요소]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-1-reporting.html)
   * [[!UICONTROL 사용자 정의 보고서 및 대시보드 만들기]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-3-reporting.html)
   * [[!UICONTROL 중간 필터 만들기]](https://experienceleague.adobe.com/docs/courses/using/workfront-u-1-2022-2-reporting.html)
* 다음 튜토리얼도 살펴보셨습니다.
   * [[!UICONTROL 보기의 기본 텍스트 모드 이해]](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-views.html?lang=ko-KR)
   * [[!UICONTROL 그룹화의 기본 텍스트 모드 이해]](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=ko-KR)

## 타깃 대상자

이 튜토리얼의 타깃 대상자는 현재 사용자 정의 보고서를 작성하고 텍스트 모드를 사용하여 보고 사용자 인터페이스가 의도한 것 이상의 작업을 수행하는 방법을 알고 싶은 [!UICONTROL 플랜] 라이선스 사용자입니다.

## 이 튜토리얼의 출처는 어디입니까?

이 튜토리얼은 2018년 2월에 3일 동안 제공된 실시간 수업을 녹화한 것입니다. 비디오에서 이전 UI를 볼 수 있지만, 제공된 콘텐츠의 정확성이나 관련성에 영향을 미치지 않습니다.

또한 연습할 테스트 드라이브 계정을 얻는 방법에 대한 몇 가지 언급도 있습니다. Adobe Experience League는 테스트 드라이브 계정을 제공하지 않지만 걱정하지 않으셔도 됩니다. 프로덕션 계정에서 연습할 수 있습니다. 결국 보고는 오브젝트를 생성하거나 삭제하는 것이 아니라 Workfront에서 오브젝트를 보는 것입니다. 물론 보고서 자체를 만드는 작업은 제외합니다. 귀하가 보고서를 공유하기로 결정하지 않는 한, 시스템 관리자 외에 귀하가 작성한 보고서를 볼 수 있는 유일한 사람은 귀하입니다.
