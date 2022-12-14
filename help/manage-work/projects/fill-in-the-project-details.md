---
title: 프로젝트 세부 사항을 입력합니다
description: 12개의 프로젝트 세부 사항 필드를 알아봅니다 [!DNL  Workfront] 프로젝트를 만들 때 을 채우는 것이 좋습니다.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Intermediate
kt: 10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 1%

---

# 프로젝트 세부 사항을 입력합니다

걱정하지 마십시오 ...사용자가 만드는 각 프로젝트를 사용하여 프로젝트 세부 사항에 모든 필드와 확인란을 채우지 않아도 됩니다 [!DNL  Workfront]. 템플릿을 사용하여 정보를 미리 작성한 다음 아래 나열된 가장 중요한 프로젝트 세부 사항 필드 12개를 확인하십시오.

1. **이름**

   설명 프로젝트 이름은 모든 사람이 프로젝트의 목적을 식별하는 데 도움이 됩니다. 조직의 프로젝트 이름 지정 규칙을 따라야 하며, 프로젝트 이름(예: 참조 번호, 부서 이름 또는 카테고리 지표)에 특정 정보가 포함될 수 있습니다.

1. **설명**

   여러 사람이 한 프로젝트에서 작업하면 프로젝트 관리자가 모든 사람이 프로젝트의 목적과 예상에 따라 신속하게 작업할 수 있어야 합니다.

   기본 정보, 답변 질문을 제공하고 프로젝트 팀이 해당 작업을 계속 진행할 수 있도록 하는 프로젝트 설명으로 이 작업을 수행합니다. 예를 들어 &quot;매출 생성 작업을 50% 증가시키기 위한 캠페인&quot; 또는 &quot;부서 전체의 효율성을 향상시키기 위한 새로운 시스템 업그레이드&quot; 등이 있습니다.

   일부 Workfront 고객에는 프로젝트 템플릿에서 프로젝트 설명이 어떻게 표시되어야 하는지에 대한 샘플이 포함되어 있습니다.

1. **상태**

   Workfront에서 상태는 프로젝트가 워크플로우에서 어디에 있는지 또는 어느 단계에서 있는지를 나타내기 위해 사용됩니다. 상태는 작동 진행 방식을 추적하기 위해 많은 Workfront 보고서에서 사용됩니다.

   Workfront에서 프로젝트 계획을 종료하고 완료하는 동안 상태를 Planning으로 설정할 것을 권장합니다. Planning 상태의 주요 사항은 Workfront 알림이 이 상태에 있는 동안 프로젝트에 대한 작업 담당자에게 전송되지 않는다는 것입니다.

   그런 다음 프로젝트가 라이브로 전환될 준비가 되면 상태를 현재 로 변경합니다. 이는 Workfront이 자신에게 할당된 작업에 대한 알림을 적절한 사람에게 전송하는 때입니다.

   >[!TIP]
   >
   >  기한 변경과 같이 프로젝트를 변경할 때 상태를 다시 Planning으로 롤업하거나 자동 저장 기능을 해제하여 변경이 완료될 때까지 알림이 전송되지 않도록 할 수 있습니다.

   시스템 관리자가 계획 상태를 글로벌 Workfront 기본값으로 설정할 수 있습니다.

1. **일정 모드**

   Workfront 프로젝트는 시작 날짜 또는 완료 날짜부터 예약할 수 있습니다. 이 중요한 선택 사항은 각 작업의 계획 날짜를 계산하는 방법을 결정합니다.

   시작 날짜 옵션은 사용자가 입력한 프로젝트에 대한 시작 날짜와 각 작업의 기간 및 선행 작업을 사용하여 프로젝트의 완료 시점을 계산합니다. Workfront에서는 이 옵션이 가장 일반적이며 계획 프로젝트 날짜를 더 쉽게 만들 수 있으므로 이 옵션을 사용하는 것이 좋습니다.

   그러나 완료 일자를 사용할 수 있습니다. Workfront은 종료 날짜(사용자가 입력)와 수행할 작업(지속 시간 및 선행 작업을 기반으로)을 확인한 다음 뒤로 이동하여 프로젝트의 시작 날짜를 계산합니다. Workfront에서는 Workfront에서 특정 수준의 숙련도가 설정된 후 완료 날짜를 대기하도록 권장합니다.

   어떤 옵션을 선택하든 팝업 달력에서 날짜를 선택하는 것을 잊지 마십시오.

   템플릿에서 예약 모드 옵션을 설정할 수 있습니다.

1. **그룹**

   그룹은 종종 부서에 정렬되는 Workfront 조직 단위입니다. 이 필드는 프로젝트 템플릿에서 설정할 수 있습니다. 그렇지 않으면 프로젝트를 만드는 사람의 홈 그룹으로 필드가 자동으로 설정됩니다. 필요에 따라 그룹을 변경할 수 있습니다.

   일반적으로 프로젝트 작업자의 대부분은 이 그룹에서 가져옵니다. 그러나 이는 사람들이 프로젝트에서 작업하도록 다른 그룹으로부터 지정되는 것을 제한하지는 않습니다.

   프로젝트의 그룹은 프로젝트에서 사용할 프로젝트, 작업 및 문제 환경 설정도 결정합니다. 특정 그룹에 대한 사용자 정의 상태와 같은 이러한 기본 설정은 시스템 관리자나 그룹 관리자가 설정합니다.

   그룹 설정은 보고 기능을 통해 부서가 작업 중인 모든 프로젝트를 표시하는 편리한 방법입니다.

1. **프로젝트 소유자**

   프로젝트 소유자는 프로젝트 관리자의 Workfront 용어입니다. 프로젝트의 계획 및/또는 관리를 담당하는 담당자입니다.

   프로젝트 소유자는 프로젝트에 대한 전체 관리 권한이 있으므로 계획 라이센스가 있어야 합니다.

   일반적으로 이 필드는 템플릿에 비워 두고 프로젝트를 작성하는 사람의 이름으로 자동으로 채워집니다. 템플릿에 이름을 입력하면 프로젝트의 기본 소유자가 됩니다.

1. **프로젝트 스폰서**

   프로젝트 스폰서는 일반적으로 프로젝트를 요청한 사람입니다. 이는 종종 관리자 또는 경영자와 같은 내부 이해 관계이며 프로젝트에 대한 전반적인 책임이 있습니다.

   스폰서에는 프로젝트에 대한 보기 권한이 자동으로 부여되며 Workfront 라이선스 사용자여야 합니다.

   템플릿에서 프로젝트 스폰서를 설정할 수 있습니다.

1. **리소스 관리자**

   이 필드에 나열된 Workfront 사용자는 나열된 특정 프로젝트에 대해 Workfront의 리소스 계획 및 관리 도구를 사용할 수 있습니다. 리소스 관리자 필드에 최대 30개의 이름을 나열할 수 있으며 각각 계획 라이센스가 있어야 합니다.

   템플릿에서 리소스 관리자 필드를 설정할 수 있습니다.

1. **사용자 정의 양식**

   Workfront에서는 프로젝트 이름 및 시작 날짜와 같은 기본 필드를 제공합니다. 하지만 프로젝트 매니저로서 필요하거나 프로젝트 팀이 필요로 하는 추가 정보가 있습니다. 고유한 데이터가 마찬가지로 중요하며 이러한 양식에 쉽게 저장할 수 있습니다. 발행 날짜, 자산 크기, 배달 채널 등과 같은 세부 사항입니다.

   사용자 지정 양식은 이 정보를 캡처할 수 있으며 Workfront의 목록 및 보고서에 포함할 수 있으므로 정보를 쉽게 보고 편집할 수 있습니다.

   미리 템플릿에 사용자 지정 양식을 첨부할 수 있습니다.

1. **일정**

   전 세계 많은 회사들이 직원을 보유하고 있기 때문에, 24시간 근무가 이루어집니다.

   Workfront을 사용하면 프로젝트에 공통 일정을 적용할 수 있습니다. 이러한 정보는 시스템 관리자가 생성합니다. 일정은 팀의 근무 일수와 시간을 반영하며, 사원이 근무하지 않을 일(휴일 등)도 반영합니다.

   계획자로서 올바른 일정을 올바른 프로젝트에 적용하고 있는지 확인합니다. 일정 설정은 시간 및 시간대를 고려하여 타임라인 계산에 영향을 줍니다.

   프로젝트에 지정된 일정은 대부분의 작업 할당자에게 적용되는 스케줄이어야 합니다. 프로젝트에 지정된 일정이 없으면 기본값으로 표시된 일정이 사용됩니다.

   일정은 템플릿에서 설정할 수 있습니다.

1. **리소스 풀**

   리소스 풀은 조직에서 프로젝트를 완료하기 위해 동시에 필요한 Workfront 사용자의 컬렉션입니다. 리소스 풀을 여러 프로젝트에 할당할 수 있으므로 리소스를 위한 프로젝트가 있을 수 있습니다.

   프로젝트에 자원 풀이 할당되어 있는 것은 Workfront의 리소스 플래너와 기타 리소스 관리 도구를 사용하기 위한 전제 조건입니다.

   템플릿에서 기본 리소스 풀을 설정할 수 있습니다.

1. **뷰어 및 기여자를 위한 프로젝트에 대한 액세스**

   프로젝트에 대한 액세스 권한을 받을 경우 프로젝트가 실시간으로 진행될 때 기본적으로 제공되는 세 가지 권한 수준(보기, 기여도 및 관리)이 있습니다. 각 권한 수준에서는 프로젝트를 보고 특정 작업을 수행할 수 있습니다.

   예를 들어 프로젝트에 액세스할 수 있지만 재무 정보는 볼 수 없는 사람이 있습니다. 따라서 뷰어 및 기여자에 대한 재무 보기 옵션을 끌 수 있습니다.

   개별 프로젝트에서 이러한 권한 설정을 언제든지 세부 조정할 수 있습니다. 그러나 프로젝트가 Planning에서 현재 상태로 이동되면 프로젝트 공유를 통해 권한 기반 조정을 수행해야 합니다.

   액세스 설정은 템플릿에서 설정할 수 있습니다.
