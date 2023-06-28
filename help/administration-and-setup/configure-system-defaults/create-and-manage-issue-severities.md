---
title: 문제 심각도 만들기 및 관리
description: 문제 심각도를 설정하고 관리하는 방법에 대해 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# 문제 심각도 만들기 및 관리

## 문제 심각도 소개

심각도는 문제가 얼마나 심각한지 또는 진행 중인 작업에 어떤 영향을 미칠 수 있는지 나타내는 데 사용할 수 있습니다.

![[!UICONTROL 심각도] 의 메뉴 [!UICONTROL 문제 세부 정보] 창](assets/admin-fund-severity-issue-details.png)

다음 [!UICONTROL 심각도] 필드는에서 액세스할 수 있습니다. [!UICONTROL 문제 세부 정보]. 목록의 열 보기 및 사용자 지정 보고서에 포함될 수도 있습니다.

[!DNL Workfront] 에는 5개의 기본 심각도가 있습니다.

* [!UICONTROL 표시용]
* [!UICONTROL 혼란 야기]
* [!UICONTROL 해결 방법이 있는 버그]
* [!UICONTROL 해결 방법이 없는 버그]
* [!UICONTROL 치명적인 오류]

시스템 관리자는 필요한 경우 이러한 기본 심각도의 이름을 바꾸거나 새 심각도를 만들 수 있습니다.

심각도는 의 문제에만 사용할 수 있습니다. [!DNL Workfront].

## 문제 심각도 만들기 및 관리

시스템 관리자는 필요한 경우 새 심각도를 만들어 문제의 워크플로를 완료할 수 있습니다.

![[!UICONTROL 심각도] 페이지 위치 [!UICONTROL 설정]](assets/admin-fund-severity-section.png)

1. 클릭 **[!UICONTROL 설정]** 다음에서 **[!UICONTROL 메인 메뉴]**.
1. 확장 **[!UICONTROL 프로젝트 환경 설정]** 왼쪽 메뉴 패널에서 섹션으로 이동하십시오.
1. 선택 **[!UICONTROL 심각도]**.
1. 클릭 **[!UICONTROL 새 심각도 추가]**.
1. 심각도에 의도한 용도와 일치하는 이름을 지정합니다.
1. 다음 **[!UICONTROL 중요도]** 이 숫자는 문제의 심각도와 일치합니다. 가장 높은 숫자는 가장 높은 심각도와 일치합니다. 다음 [!UICONTROL 중요도] 숫자는 고유해야 합니다.
1. 우선 순위의 색상을 선택합니다. 차트 보고서 및 의 다른 위치에 사용됩니다. [!DNL Workfront].
1. 심각도 옵션 중 하나를 로 지정 **[!UICONTROL 기본 심각도]**. 이 기능은 Workfront의 모든 새로운 문제에 자동으로 적용됩니다.
1. 사용 방법 등 심각도에 대한 설명을 포함합니다.
1. 필드 외부를 클릭하여 저장합니다.

![[!UICONTROL 심각도] 목록](assets/admin-fund-severity-new.png)

### 심각도 수정

심각도가 더 이상 문제 워크플로우와 관련이 없는 경우 이름을 바꾸거나, 숨기거나, 삭제할 수 있습니다.

심각도가 더 이상 필요하지 않으면 [!DNL Workfront] 에서는 심각도를 숨기는 것을 권장합니다(다음 클릭) [!UICONTROL 숨기기] 설정 영역에서 상자 옆에 있습니다. 이렇게 하면 문제에 대한 드롭다운 메뉴에서 심각도 옵션이 제거되지만, 내역 데이터의 심각도가 유지되므로 보고 목적으로 계속 사용할 수 있습니다.

![[!UICONTROL 숨기기] 강조 표시된 열 [!UICONTROL 심각도] 페이지 위치 [!UICONTROL 설정]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] 다음을 권장합니다. **금지** 지난 문제에 사용된 심각도를 삭제합니다. 심각도를 삭제하면 다른 심각도로 대체하라는 메시지가 표시됩니다. 이렇게 하면 내역 데이터가 변경되고 보고에 영향을 줄 수 있습니다.

![심각도 삭제 창](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
