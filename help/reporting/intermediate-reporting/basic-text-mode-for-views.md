---
title: 보기의 기본 텍스트 모드 이해
description: 텍스트 모드가 무엇인지, 카멜 표기법이 무엇인지, Workfront 보기에서 사용할 수 있는 몇 가지 기본 "플러그 앤 플레이" 텍스트 모드에 대해 알아봅니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 보기의 기본 텍스트 모드 이해


>[!IMPORTANT]
>
>사전 요구 사항:
>
>* 보고 요소 이해
>* 보고 구성 요소 이해
>* 기본 보기 만들기

>[!TIP]
>
>* 텍스트 모드를 더 깊이 있게 이해하려면 기록된 웨비나 이벤트를 시청하는 것이 좋습니다 [전문가에게 문의 - 텍스트 모드 보고 소개](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en): 1시간 길이입니다.
>* 텍스트 모드에 대해 더 자세히 알아보려면 [고급 보고](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) 총 5시간 30분 분량의 튜토리얼.

이 비디오에서는 다음 사항에 대해 알아봅니다.

* 텍스트 모드
* 낙타 케이스는 무엇입니까?
* 보기에서 사용할 수 있는 몇 가지 기본 &quot;플러그 앤 플레이&quot; 텍스트 모드

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12&learn=on)

## 작업 - 상위 4개 보기

먼저 작업 이름 및 상위 이름에 대한 열을 만든 다음 다음 다음 텍스트 모드를 사용하여 다른 세 개의 열을 만듭니다.

### 작업 - 상위 이름의 상위

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

### 작업 - 상위 이름의 상위

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

### 작업 - 상위 이름의 상위 항목

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![4개의 상위 보기를 보여 주는 화면 이미지](assets/4-parents-view.png)

## 사용자 - 사용자 보기의 목록을 표시하는 반복

### 사용자 - 모든 작업 역할

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### 사용자 - 기본을 표시하는 모든 작업 역할

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### 사용자 - 모든 팀

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>UI를 통해 액세스할 수 있는 팀 필드가 있으며, 이 필드는 모든 팀을 쉼표로 구분해서 표시하지만, 위의 텍스트 모드를 사용하면 각 팀이 별도의 줄에 표시됩니다.


### 사용자 - 모든 그룹

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### 사용자 - 홈 그룹을 표시하는 모든 그룹

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### 사용자 - 부하 직원

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### 사용자 - 향후 유급휴가

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![사용자 목록 보기를 보여 주는 화면 이미지](assets/user-lists-view-large.png)

## 작업 - 작업 할당 및 작업 중 상태를 표시하는 방법

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![할당 및 상태 보기를 보여 주는 화면 이미지](assets/assignments-and-status-view.png)


## 작업 - 여러 작업 할당에 대한 역할 및 할당을 표시하는 방법

### 작업 - 역할 + 시간

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### 작업 - 할당 + 비율 할당

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![할당 및 역할 보기를 보여주는 화면 이미지](assets/assignments-roles-and-percent-view.png)

## 작업 - 프로젝트 간 전임 작업 및 후임 작업

### 작업 필터(선택 사항)

**프로젝트 간 전임 작업이 하나 이상 있는 모든 작업 표시**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### 작업 - 전임 작업 이름 및 프로젝트 전임 작업이 포함된 위치 표시

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

### 작업 - 후임 작업 이름과 프로젝트 후임 작업이 포함된 위치 표시

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

### 작업 - 전임 작업의 예상 완료 일자 표시

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

### 작업 - 전임 작업의 진행 상태 표시

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

### 작업 - 프로젝트 간 전임 작업 프로젝트의 완료율 표시

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![프로젝트 간 전임 작업 및 후임 작업 보기를 보여 주는 화면 이미지](assets/cross-project-predecessors-and-successors.png)


## 작업 - 할당된 모든 사용자와 각 사용자를 보여 주는 반복

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![할당된 모든 사람과 각 사람을 할당한 사람을 보여 주는 화면 이미지](assets/all-assignees-and-requesters.png)

## 작업/프로젝트 - 프로젝트 또는 작업의 모든 사용자 정의 양식을 보여주는 반복

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![프로젝트의 모든 사용자 정의 양식을 보여주는 화면 이미지](assets/all-custom-forms-on-a-project.png)


## 프로젝트 - 프로젝트 보기에서 해결 가능 항목의 모든 기본 연락처를 보여 주는 반복

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![해결 방법에 대한 기본 연락처를 보여주는 화면 이미지](assets/primary-contacts-for-resolvables.png)

## 프로젝트 - 모든 프로젝트 팀원을 보여 주는 반복

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![모든 프로젝트 팀원을 보여 주는 화면 이미지](assets/all-project-team-members.png)

## 프로젝트 - 프로젝트에 대해 해결 가능한 모든 문제의 entryDate를 보여 주는 반복

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![프로젝트에 대해 해결 가능한 모든 문제의 entryDate를 보여 주는 화면 이미지](assets/resolvables-entry-date.png)

## 프로젝트 - 원래 프로젝트 요청자의 홈 그룹 표시

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![프로젝트 요청자 홈 그룹을 보여 주는 화면 이미지](assets/requestor-home-group.png)

## 프로젝트 - 프로젝트가 요청 대기열인 경우 표시

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![프로젝트가 요청 대기열인지 보여 주는 화면 이미지](assets/project-is-a-request-queue.png)

## 문제 - 모든 해결 프로젝트 팀원을 보여 주는 반복

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![모든 해결 프로젝트 팀원을 보여 주는 화면 이미지](assets/all-resolve-project-team-members.png)

## 문제 - 문제 기본 담당자의 모든 팀을 표시하는 반복

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![모든 기본 담당자 팀을 보여 주는 화면 이미지](assets/all-primary-contact-teams.png)

## 문서 - 문서 보고서의 폴더를 표시하는 반복

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![문서 보고서의 폴더를 보여 주는 화면 이미지](assets/folder-in-a-document-report.png)

## 문서 - 문서 보고서에서 상위 폴더를 보여 주는 반복

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![문서 보고서의 상위 폴더를 보여 주는 화면 이미지](assets/parent-folder-in-a-document-report.png)

## 문서 - 문서 승인 일자

```
displayname=Document approval dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![문서 승인 날짜 보기를 보여 주는 화면 이미지](assets/document-approval-dates.png)

## 증명 승인

### 증명 승인 - 프로젝트 이름 표시

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### 증명 승인 - 작업 이름 표시

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![증명 승인의 프로젝트 및 작업을 보여 주는 화면 이미지](assets/proof-approval-project-and-task.png)
