---
title: 시스템 감사 로그 이해
description: 시스템 감사 로그를 사용하여 변경 사항과 항목 변경 시기를 검토하는 방법을 알아봅니다.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# 시스템 감사 로그 이해

시스템 감사 로그는 시스템 관리자가 진행 상황을 파악하는 가장 좋은 방법입니다 [!DNL Workfront]. 로그를 누가 언제 어떤 변화를 주었는지에 대한 진실의 소스로 생각하십시오.

로 이동하여 감사 로그에 액세스합니다. [!UICONTROL 환경 설정] 의 섹션 [!UICONTROL 설정] 영역입니다. 기본적으로 지난 7일의 데이터가 표시됩니다. 다른 날짜 범위의 데이터를 보려면 필터 기준을 변경하십시오.

사용자가 특정 작업을 수행할 때 [!UICONTROL Workfront] 다음 위치에 레코드: [!UICONTROL 감사 로그] 의 섹션 [!UICONTROL 설정] 영역입니다.

![[!UICONTROL 로그 유형] 드롭다운 메뉴 [!UICONTROL 감사 로그] 페이지 위치 [!UICONTROL 설정]](assets/admin-fund-audit-log-1.png)

기록되거나 기록된 각 작업은 다음을 표시합니다.

* 변경 날짜 및 시간
* 로그 유형
* 작업을 완료한 사용자의 이름
* 개체
* 작업과 관련된 모든 세부 정보
* IP 주소

![[!UICONTROL 감사 로그] 목록](assets/admin-fund-audit-log-2.JPG)

## 감사 로그 내보내기

감사 로그 데이터를 내보내면 시스템 관리자가 내부/외부 감사자 또는 보안 전문가와 정보를 공유할 수 있습니다. 일부 조직에서는 사이버 보안 규정을 준수하기 위해 특정 로그를 보존해야 합니다. 다른 이들은 분석을 위해 보안 시스템으로 가져온 정보가 필요합니다.

감사 로그를 CSV(쉼표로 구분된 값) 파일로 내보내고 스프레드시트 애플리케이션이나 일반 텍스트 편집기로 열 수 있습니다. 내보내기는 한 번에 50,000개의 행으로 제한되므로 합계가 50,000개를 초과하는 경우 필터를 사용하여 목록의 범위를 좁힙니다.

![[!UICONTROL 내보내기] 단추 [!UICONTROL 감사 로그] 페이지](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
