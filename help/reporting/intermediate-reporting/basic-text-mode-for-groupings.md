---
title: 그룹화에 대한 기본 텍스트 모드 이해
description: 텍스트 모드, 카멜 표기법 및 Workfront의 그룹화에 사용할 수 있는 몇 가지 기본 "플러그인 및 재생" 텍스트 모드를 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
source-git-commit: 21fb81fcb4b1468059e571a87e201fa48fb64ff7
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# 그룹화에 대한 기본 텍스트 모드 이해

>[!IMPORTANT]
>
>전제 조건:
>
>* 보고 요소 이해
>* 보고 구성 요소 이해
>* 기본 그룹 만들기


이 비디오에서는 다음을 학습합니다.

* 텍스트 모드는 무엇입니까?
* 낙타의 예는 무엇인가요
* 그룹화에 사용할 수 있는 몇 가지 기본적인 &quot;플러그 앤 플레이&quot; 텍스트 모드

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12)

## 작업 - 상위 4개 그룹

다음 텍스트 모드는 최대 4가지 상위 수준을 기준으로 작업을 그룹화하고 존재하지 않는 부모를 비워 둡니다.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![4명의 부모별로 그룹화된 프로젝트 작업을 보여주는 화면 이미지입니다](assets/4-parents-grouping.png)


## 작업 - 전체 그룹 비율

다음 텍스트 모드는 완료율을 기준으로 작업을 그룹화합니다. 작업은 그룹화할 때 다음 범주 중 하나로 분류됩니다.

* 0%
* 1%~25%
* 26%~50%
* 51%~75%
* 76%~99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![완료율별로 그룹화된 프로젝트 작업을 보여주는 화면 이미지입니다](assets/percent-complete-grouping.png)

## 작업 - statusEqualsWith, then 상태

다음 텍스트 모드에서는 statusEquatesWith를 기준으로 작업을 그룹화한 다음 상태별로 그룹화합니다.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![statusEquatesWith로 그룹화된 프로젝트 작업을 보여주는 화면 이미지입니다.](assets/status-equates-with.png)


## 증명 승인 - 프로젝트 이름별 그룹

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![프로젝트 이름별로 그룹화된 증명 승인을 보여주는 화면 이미지입니다](assets/proof-approvals-grouped-by-project-name.png)

