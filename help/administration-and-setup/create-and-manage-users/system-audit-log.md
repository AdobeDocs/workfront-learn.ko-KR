---
title: 시스템 감사 로그 이해
description: 시스템 감사 로그를 사용하여 항목이 변경된 경우와 그 경우를 검토하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 100%

---

# 시스템 감사 로그 이해

시스템 감사 로그는 시스템 관리자가 [!DNL Workfront]에서 무슨 일이 일어나고 있는지 확인할 수 있는 가장 좋은 방법입니다. 누가 무엇을 언제 변경했는지에 대한 정보 소스로 로그를 간주합니다.

[!UICONTROL 설정] 영역의 [!UICONTROL 환경 설정] 섹션으로 이동하여 감사 로그에 액세스합니다. 기본적으로 지난 7일 동안의 데이터가 표시됩니다. 다른 날짜 범위의 데이터를 보려면 필터 조건을 변경합니다.

사용자가 특정 동작을 수행할 때 [!UICONTROL Workfront]는 이를 [!UICONTROL 설정] 영역의 [!UICONTROL 감사 로그] 섹션에 기록합니다.

[!UICONTROL 설정]](assets/admin-fund-audit-log-1.png)의 [!UICONTROL 감사 로그] 페이지에 있는 ![[!UICONTROL 로그 유형] 드롭다운 메뉴

기록되거나 로그된 각 작업은 다음을 표시합니다.

* 변경 일자 및 시간
* 로그 유형
* 작업을 완료한 사용자 이름
* 오브젝트
* 작업과 관련된 모든 세부 정보
* IP 주소

![[!UICONTROL 감사 로그] 목록](assets/admin-fund-audit-log-2.JPG)

## 감사 로그 내보내기

시스템 관리자는 감사 로그 데이터 내보내기를 통해 내부/외부 감사자 또는 보안 전문가와 정보를 공유할 수 있습니다. 일부 조직에서는 사이버 보안 규정을 준수하기 위해 특정 로그를 보관해야 합니다. 다른 조직에서는 분석을 위해 보안 시스템으로 가져온 정보가 필요합니다.

감사 로그는 스프레드시트 애플리케이션 또는 일반 텍스트 편집기에서 열 수 있는 CSV(쉼표로 구분된 값) 파일로 내보낼 수 있습니다. 내보내기는 한 번에 50,000개의 행으로 제한되므로 총 50,000개를 초과하는 경우, 필터를 사용하여 목록의 범위를 좁힙니다.

[!UICONTROL 감사 로그] 페이지의 ![[!UICONTROL 내보내기] 버튼](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
