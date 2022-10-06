---
title: 사용자 지정 양식 만들기 및 공유
description: 맞춤형 양식을 만들고, 양식에 고유한 필드를 추가하고, 섹션 및 논리를 사용하여 필드를 구성하고, 사용자와 양식을 공유하는 방법에 대해 알아보십시오.
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
thumbnail: 335172.png
kt: 8909
exl-id: b37334c7-67d0-4359-9537-dc26843582d1
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 5%

---

# 사용자 지정 양식 만들기 및 공유

이 비디오에서는 다음 방법을 배웁니다.

* 양식에 사용할 개체 결정
* 다양한 형식으로 고유한 필드 추가
* 섹션 및 논리를 사용하여 필드 구성
* 다른 사용자와 양식 공유

>[!VIDEO](https://video.tv.adobe.com/v/335172/?quality=12)

## 사용자 지정 양식은 여러 개체 유형에서 작동합니다

을(를) 클릭하면 [!UICONTROL 새 사용자 지정 양식] 단추를 사용하면 단일 사용자 지정 양식에 사용할 개체를 선택할 수 있습니다. 사용자 지정 양식이 첨부된 경우 선택한 개체에서 이 양식에 추가하는 모든 필드를 사용할 수 있습니다.

![을 보여주는 사용자 지정 양식 창 [!UICONTROL 새 사용자 지정 양식] 개체 옵션](assets/create-custom-form.png)

사용자 지정 양식을 편집하면 선택한 모든 개체 유형을 볼 수 있습니다. 이 목록에서 객체 유형을 추가하거나 삭제할 수 있습니다.

![양식 편집 중에 선택한 개체 유형을 보여주는 사용자 지정 양식 창](assets/edit-custom-form.png)

프로젝트 및 문제의 사용자 지정 양식을 만들 수 있습니다. 문제에 첨부된 경우 문제와 관련된 필드를 작성할 수 있습니다. 나중에 문제를 프로젝트로 전환하기로 결정하는 경우 사용자 지정 양식이 프로젝트에 자동으로 로드되고 문제 사용자 지정 양식의 필드에 입력하는 데이터는 프로젝트 사용자 지정 양식에서 보거나 편집할 수 있습니다.

## 사용자 지정 필드 옵션

**[!UICONTROL 레이블] 및 [!UICONTROL 이름] 필드**

다음 [!UICONTROL 레이블] 및 [!UICONTROL 이름] 사용자 지정 필드의 필드는 다른 용도로 사용됩니다. [!UICONTROL 레이블] 는 사용자가 볼 필드 이름입니다 [!DNL Workfront]. [!UICONTROL 이름] 는 API와 같은 통합에 사용할 수 있는 것입니다.

![표시되는 사용자 지정 양식 창 [!UICONTROL 레이블] 및 [!UICONTROL 이름] 필드](assets/custom-forms-field-label-and-name.png)

이렇게 하면 통합 또는 특정 필드 이름을 사용하는 기타 연결에 영향을 주지 않고 조직의 변경 사항과 일치하도록 사용자 지정 레이블을 변경할 수 있는 유연성을 제공합니다.

**[!UICONTROL 포맷이 지정된 텍스트 필드]**

다음 [!UICONTROL 서식이 있는 텍스트 필드 ]사용자가 사용자 지정 양식의 필드에 입력하는 동안 텍스트에 굵게, 기울임체 또는 밑줄을 추가할 수 있는 기본 텍스트 마크업 도구를 포함합니다.

![표시되는 사용자 지정 양식 창 [!UICONTROL 서식이 있는 텍스트 필드] 옵션](assets/custom-forms-text-field-with-formatting.png)

또한 이 필드에는 15,000자 제한이 있어 중요한 정보를 제공하고 서식으로 다른 사람이 쉽게 읽을 수 있습니다.

**[!UICONTROL Typeahead] 필드**

다음 [!UICONTROL Typeahead] 필드에서는 필드에 대해 선택한 개체를 기반으로 옵션 목록을 자동으로 채울 수 있습니다.

![표시되는 사용자 지정 양식 창 [!UICONTROL Typeahead] 필드 옵션](assets/custom-forms-typeahead-1.png)

예를 들어 [!UICONTROL Typeahead] &quot;Marketing Manager 승인 이름&quot;이라는 필드를 선택하고 [!UICONTROL 사용자] 참조된 개체 유형으로 사용자가 사용자 정의 양식의 해당 필드를 채울 때 사용자 이름 목록이 표시됩니다. 다음 [!UICONTROL Typeahead] 필드는 사용자 지정 데이터를 시스템에 캡처된 정보와 연결하며 드롭다운 필드에서 많은 옵션을 수동으로 유지 관리할 필요가 없도록 하기 위한 것입니다.

![표시되는 사용자 지정 양식 창 [!UICONTROL Typeahead] 드롭다운 메뉴](assets/custom-forms-typeahead-2.png)
