---
title: 이메일 경고 및 교정쇄 알림 이해
description: ' [!DNL  Workfront]에서 이메일 경고 및 교정쇄 알림 간의 차이점을 알아봅니다.'
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:07:01.396Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 100%

---

# 이메일 경고 및 교정쇄 알림 이해

이메일 경고는 교정쇄 알림 이메일과 다릅니다. 검토할 새 교정쇄가 할당되었거나, 교정쇄가 지연되었거나, 검토할 새 버전의 교정쇄가 있는 경우, 교정쇄 알림 이메일을 받게 됩니다.

![검토할 새 교정쇄가 있음을 나타내는 교정쇄 알림 이메일의 이미지.](assets/email-alert-1.png)

교정쇄를 업로드할 때 알림 옵션을 끄면 [!DNL Workfront]로부터 검토할 새 교정쇄가 있다는 것에 대한 통신을 받지 못합니다.

이메일 경고는 검토자/승인자별로 설정되며, 대부분 교정쇄가 업로드될 때 설정됩니다. 기본 이메일 경고 유형은 교정쇄 수신자에게 할당될 수 있으므로 교정쇄를 업로드할 때마다 설정할 필요가 없습니다. 이러한 기본값을 설정하는 방법에 대해서는 시스템 관리자에게 문의하십시오.

![교정쇄에 대한 결정이 내려졌고 검토할 댓글이 있음을 나타내는 이메일 경고 이미지.](assets/email-alert-2.png)

이메일 경고가 [!UICONTROL 비활성화됨]으로 설정된 경우에도 교정쇄 수신자는 새 교정쇄 또는 버전에 대한 알림을 받습니다.

## 모범 사례

| 모범 사례 | 이유 |
|---|---|
| Workfront 설정에서 “교정쇄에 대한 댓글이 제시되면 Workfront에서 이메일 보내기” 설정을 비활성화합니다. | 이 설정이 활성화되면(기본적으로 활성화됨) 사용자는 교정 기능에서 하나, Workfront 자체에서 하나 등 교정쇄에 대한 각 댓글에 대해 여러 이메일 알림을 받을 수 있습니다. 이러한 중복 알림은 이메일 알림 중단 및 혼란뿐만 아니라 전체 이메일 받은 편지함으로 이어져 궁극적으로는 사용자가 받은 교정쇄 알림을 무시할 수 있습니다. 이로 인해 기한을 놓칠 수도 있습니다. <br> <br>메모: 이 설정은 Workfront 메인 메뉴 > 설정 > 이메일 > 검토 및 승인에서 확인할 수 있습니다. |


