---
title: 기존 Adobe Workfront 인스턴스 구현 관리
description: 새로운 시스템 또는 그룹 관리자로서 Workfront 인스턴스를 평가하고, 이해하고, 최적화하기 위한 주요 단계를 알아봅니다.
feature: System Setup and Administration
type: Tutorial
role: Admin
level: Beginner,Intermediate,Experienced
activity: use
jira: KT-11747
team: Technical Marketing
thumbnail: null
exl-id: ad900f59-319b-49ee-bc23-e816edc2de24
source-git-commit: ed631261fc3ad4eb72b59e1ca5b3a79951d8645b
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 100%

---

# 기존 Adobe Workfront 인스턴스 구현 관리

Workfront의 놀라운 점은 사용자 정의가 가능하다는 것입니다. Workfront의 어려운 점은 사용자 정의가 가능하다는 것입니다. 기존 Workfront 인스턴스를 인수하는 새로운 시스템 또는 그룹 관리자인 경우, 원래 구성 및 설정 방법을 파악하는 것이 어려울 수 있습니다.

그러나 상속된 인스턴스 체크리스트를 통해 인스턴스에 대해 알아야 할 모든 것을 배울 수 있습니다.

![상속된 인스턴스 체크리스트 이미지](assets/wf-inherited-instance-image.png)
<br></br>

상속된 인스턴스 체크리스트에서 포괄적인 질문, 리소스 및 링크를 검토하여 구성 방법을 명확하게 이해할 수 있습니다.

체크리스트는 Workfront 블루프린트와 다운로드 가능한 Excel 스프레드시트로 작성되었습니다. Workfront에서 바로 작업을 관리하고 문서화하려면 블루프린트를 사용하는 것이 좋습니다.

블루프린트와 스프레드시트 모두 타임라인이 아닌 주제별로 구성되어 있어 귀하와 귀하의 조직에 가장 적합한 방식으로 진행할 수 있습니다. 제공된 기간은 예시이며 특정 요구 사항에 맞게 조정해야 합니다. 이 모든 것을 한 번에 완료할 필요는 없습니다!

가능하면 조직의 다른 사람들과 협력하여 이러한 요소를 검토 및 문서화하고 주요 변경 사항이 있는 경우 문서화를 최신 상태로 유지하는 것이 좋습니다. 미래의 인스턴스 관리자가 감사할 것입니다!

* <b>블루프린트를 다운로드하려면</b> Workfront 인스턴스에서 메인 메뉴로 이동하여 ‘블루프린트’를 선택합니다. Find the Blueprint titled “상속된 인스턴스 기본 사항 | 체크리스트”라는 블루프린트를 찾아 ‘설치’를 클릭합니다. 프로덕션 또는 샌드박스 환경을 선택하고 계속해서 구성합니다. 블루프린트 설치 및 구성에 대한 자세한 내용은 [여기](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/blueprints/blueprints-install.html?lang=ko)를 참조하십시오.

* <b>Excel 체크리스트를 다운로드하려면</b> [여기](assets/adobe-workfront-system-admin-playbook-inherited-instance.xlsx)를 클릭하십시오.

블루프린트 체크리스트를 사용하든 Excel 체크리스트를 사용하든 이 프로세스는 검색, 감사, 문서화라는 3가지 주요 단계로 생각할 수 있습니다. 설명과 이상적인 결과는 다음과 같습니다.

<br>
</br>

## 1단계: 학습 및 검색

<b>권장 일정: 4주</b>

가장 먼저 해야 할 일은 현재 Workfront 인스턴스가 어떻게 설정되어 있는지 파악하는 것입니다.

여기에는 조직 내 다양한 그룹이 Workfront를 활용하는 방법을 이해하기 위해 관련자 인터뷰를 수행하고 기존 문서를 검토하는 작업이 포함됩니다.

기술적 관점에서 Workfront에 익숙하지 않은 경우, 시스템 관리자 교육을 받으십시오. 이를 통해 Workfront에서 다양한 설정의 작동 방식과 각 도구와 잠재적으로 각 사용자에게 미치는 영향에 대해 필요한 인사이트를 얻을 수 있습니다.

이 단계를 마치면 다음을 갖추게 됩니다.

* 조직에서 Workfront를 사용하는 이유에 대한 명확한 이해

* 주요 사용 사례를 포함하여 인스턴스 상태에 대한 전반적인 인지

* 작동 현황과 프로세스 및 사용자 요구에 따른 문제 및/또는 격차를 설명하는 문서
<br>
</br>

## 2단계: 시스템 감사

<b>권장 일정: 4주 </b>

초기 검색 후에는 인스턴스에 대해 보다 기술적인 감사를 수행하는 것이 좋습니다. 현재 설정 및 구성이 비즈니스 요구 사항을 충족하는지 확인하기 위해 수행해야 할 변경 사항 또는 개선 사항을 결정해야 합니다.

이 단계를 마치면 다음을 갖추게 됩니다.

* 현재 인스턴스 상태에 자세히 확인

* 비즈니스 요구 사항을 해결하기 위해 인스턴스에 수행할 변경 사항 또는 개선 사항을 확인합니다.
<br>
</br>

## 3단계: 설명서 및 최적화

<b>권장 일정: 초기 = 2주, 지속적인 업데이트 </b>

1단계와 2단계에서 배운 내용을 기반으로 인스턴스를 생성 또는 업데이트하고 문서화하고 로드맵을 개발하여 전략적 및 프로그램 수준 문제를 해결하고자 할 것입니다.

이 단계가 진행되는 동안 다음이 있어야 합니다.

* 이 문서의 여러 탭에서 질문에 답변하는 서면으로 된 중앙 집중식 설명서

* 최우선 순위 워크플로, 자동화 및 통합의 시각적 다이어그램

* 조직 및 전략적 문제를 개선하기 위해 향후 개선 사항을 문서화하는 백로그 또는 로드맵

<br>
각 단계를 거치고 상속된 인스턴스 체크리스트를 사용하여 새 시스템 또는 그룹 관리자로서 Workfront 인스턴스의 구성 방식, 필요한 조정 또는 개선 사항을 보다 잘 이해하고 조직의 Workfront 환경을 최적화하기 위한 설명서를 강화해야 합니다.

<br>
</br>

추가 정보는 아래에서 확인할 수 있습니다.
* [웨비나: 상속된 인스턴스 인수를 위한 팁](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/webinar-system-admin-essentials-tips-for-taking-over-an-existing/td-p/571873?profile.language=ko)
* [Workfront 구현을 위한 목표 정의](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/get-started-administration/define-wf-goals-objectives.html?lang=ko)
* [블로그 게시물: 리더십에 대한 후원 및 가치](https://experienceleaguecommunities.adobe.com/t5/workfront-blogs/customer-success-tips-executive-sponsorship-and-value-to/ba-p/518353?profile.language=ko)
* [블로그 게시물: Adobe Workfront KPI 소개](https://experienceleaguecommunities.adobe.com/t5/workfront-blogs/kpi-dashboards-in-the-new-workfront-experience-introduction-to/ba-p/549001?profile.language=ko)
