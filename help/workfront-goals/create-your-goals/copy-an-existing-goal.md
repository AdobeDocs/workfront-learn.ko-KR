---
title: 기존 목표 복사
description: ' [!DNL Workfront Goals]에서 기존 목표를 복사하는 방법에 대해 알아봅니다.'
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 100%

---

# 기존 목표 복사

분기가 끝나 다음 기간에 대한 기존 목표를 다시 만들고 싶다고 가정해 보겠습니다. 또는 목표를 완료하지 못하여 다음 기간으로 연장해야 하는 경우가 있습니다. 해당 목표를 만드는 최선의 옵션은 무엇일까요? 바로 기존 목표를 복사하여 수정하는 것입니다.

기존 목표를 복사하는 것은 여러 팀원이 비슷한 목표를 보유하고 있고 각 팀원에 대해 하나의 목표를 만들어야 하는 경우에도 유용합니다.

<!--
Pro-tips graphic
-->

다음은 목표를 복사하기 전에 고려해야 할 몇 가지 사항입니다.

* 목표 기간(과거이기 때문)을 제외한 원래 목표의 모든 정보가 복사됩니다.
* 기존 목표의 결과를 복사할 수 있으며 이 결과가 새 목표로 전송됩니다.
* 복사된 결과는 기본적으로 동일한 소유자에게 할당됩니다.
* 기존 목표의 진행 상황은 새 목표로 복사할 수 없습니다.
* 목표를 복사할 때 목표의 활동은 복사할 수 없습니다.

## 목표를 복사하는 방법

1. 목표 이름을 클릭하여 **[!UICONTROL 목표 세부 정보]** 패널을 엽니다.
1. 점 3개 아이콘을 클릭한 다음 **[!UICONTROL 복사]**&#x200B;를 선택합니다.
1. 복사된 목표에 대해 다음 정보를 업데이트합니다.
   * **새 목표**- 새 목표의 이름입니다. 기본값은 원래 목표의 이름입니다.
   * **기간**- 목표를 달성하고자 하는 기간입니다. 드롭다운 메뉴에서 기간을 선택하거나 ‘사용자 정의 일자 정의’를 클릭하여 사용자 정의 기간을 지정합니다. 기본 기간은 항상 현재 분기입니다.
   * **소유자** - 목표의 소유자입니다. 사용자, 팀, 그룹 또는 회사일 수 있습니다. 기본값은 원래 목표의 소유자입니다.
   * **설명** - 목표에 대한 추가 정보입니다.

1. 원래 목표에 추가된 결과가 있고 이를 새 목표에 복사하려는 경우 **[!UICONTROL 결과 복사]** 상자를 선택합니다. 복사된 목표의 결과는 원래 목표의 결과와 소유자, 이름 및 측정 값이 동일합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 복사된 목표는 초안 상태로 저장됩니다.

   ![[!DNL Workfront Goals]의 [!UICONTROL 목표 세부 정보] 패널에서 [!UICONTROL 복사] 옵션이 표시된 이미지](assets/03-workfront-goals-copy-a-goal.png)

1. **[!UICONTROL 활성화]**&#x200B;를 클릭하여 목표 상태를 활성으로 업데이트합니다. “활성화”하려면 목표에 연결된 활동 또는 결과가 있어야 합니다.

1. [!UICONTROL 목표 세부 정보] 패널의 오른쪽 상단에 있는 **X**&#x200B;를 클릭하여 닫습니다.

이전 기간에 완료되지 않은 목표를 복사했고 다음 기간에 계속 작업하려면 다음을 수행합니다.

1. **[!UICONTROL 목표 목록]**, **[!UICONTROL 체크인]** 섹션 또는 **[!UICONTROL 펄스]** 섹션에서 원래 목표로 이동합니다.
1. 목표가 복사되었고 최신 목표가 생성되었음을 나타내기 위해 목표에 댓글을 남깁니다.
1. 원래 기간 동안의 진행 상황이 유지되도록 원래 목표를 닫습니다. **[!UICONTROL 목표 세부 정보]** 패널에서 점 3개 아이콘을 클릭하고 메뉴에서 **[!UICONTROL 닫기]**&#x200B;를 선택합니다.
1. 이전 결과의 **[!UICONTROL 대상]** 값과 일치하도록 새 결과의 [!UICONTROL 초기] 값을 업데이트합니다. 이렇게 하면 새 목표 진행률이 이전 기간에 달성한 지점부터 계산하기 시작합니다.
