---
title: 문제 심각도 만들기 및 관리
description: 문제 심각도를 설정하고 관리하는 방법을 알아봅니다.
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
ht-degree: 100%

---

# 문제 심각도 만들기 및 관리

## 문제 심각도 소개

심각도를 사용하여 문제의 심각도 정도 또는 수행 중인 작업에 미치는 영향을 나타낼 수 있습니다.

[!UICONTROL 문제 세부 정보] 창의 ![[!UICONTROL 심각도] 메뉴](assets/admin-fund-severity-issue-details.png)

[!UICONTROL 심각도] 필드는 [!UICONTROL 문제 세부 정보]에서 액세스할 수 있습니다. 목록의 열 보기 및 사용자 정의 보고서에도 포함될 수 있습니다.

[!DNL Workfront]에는 다섯 가지 기본 심각도가 있습니다.

* [!UICONTROL 표시용]
* [!UICONTROL 혼란 야기]
* [!UICONTROL 해결 방법이 있는 버그]
* [!UICONTROL 해결 방법이 없는 버그]
* [!UICONTROL 치명적인 오류]

시스템 관리자는 이러한 기본 심각도의 이름을 변경하거나 필요하다면 새 심각도를 만들 수 있습니다.

심각도는 [!DNL Workfront]의 문제에 대해서만 사용할 수 있습니다.

## 문제 심각도 만들기 및 관리

필요한 경우 시스템 관리자는 문제의 워크플로를 완료하기 위해 새 심각도를 만들 수 있습니다.

[!UICONTROL 설정]](assets/admin-fund-severity-section.png)의 ![[!UICONTROL 심각도] 페이지

1. **[!UICONTROL 메인 메뉴]**&#x200B;에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. 왼쪽 메뉴 패널에서 **[!UICONTROL 프로젝트 환경 설정]** 섹션을 확장합니다.
1. **[!UICONTROL 심각도]**&#x200B;를 선택합니다.
1. **[!UICONTROL 새 심각도 추가]**&#x200B;를 클릭합니다.
1. 용도와 일치하는 심각도에 이름을 지정합니다.
1. **[!UICONTROL 중요도]** 숫자는 문제의 심각성과 일치합니다. 가장 높은 숫자는 가장 높은 심각도에 해당합니다. [!UICONTROL 중요도] 숫자는 고유해야 합니다.
1. 우선 순위의 색상을 선택합니다. [!DNL Workfront]의 차트 보고서 및 기타 위치에서 사용됩니다.
1. 심각도 옵션 중 하나를 **[!UICONTROL 기본 심각도]**&#x200B;로 지정합니다. 이는 Workfront의 모든 새로운 문제에 자동 적용됩니다.
1. 사용 방법과 같은 심각도에 대한 설명을 포함합니다.
1. 필드 외부를 클릭하여 저장합니다.

![[!UICONTROL 심각도] 목록](assets/admin-fund-severity-new.png)

### 심각도 수정

심각도가 더 이상 문제 워크플로와 관련이 없으면 이름을 바꾸거나 숨기거나 삭제할 수 있습니다.

더 이상 심각도가 필요하지 않은 경우, [!DNL Workfront]는 심각도를 숨길 것을 권장합니다(설정 영역의 옆에 있는 [!UICONTROL 숨기기] 상자 클릭). 이렇게 하면 문제의 드롭다운 메뉴에서 심각도 옵션이 제거되지만, 내역 데이터의 심각도는 유지되므로 보고용으로 계속 사용할 수 있습니다.

[!UICONTROL 설정]](assets/admin-fund-severity-hide.png)의 [!UICONTROL 심각도] 페이지에 강조 표시된 ![[!UICONTROL 숨기기] 열

[!DNL Workfront]는 이전 문제에 사용된 심각도는 삭제하지 **않을** 것을 권장합니다. 심각도를 삭제하면 다른 심각도를 대체할지 묻는 메시지가 표시됩니다. 이는 내역 데이터를 변경하고 보고에 영향을 줄 수 있습니다.

![심각도 창 삭제](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
