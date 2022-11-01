---
title: 보기에 대한 기본 텍스트 모드 이해
description: Workfront에서 볼 수 있는 텍스트 모드, 카멜 표기법 및 몇 가지 기본 "플러그 앤 플레이" 텍스트 모드를 확인할 수 있습니다.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 보기에 대한 기본 텍스트 모드 이해


>[!IMPORTANT]
>
>전제 조건:
>
>* 보고 요소 이해
>* 보고 구성 요소 이해
>* 기본 보기 만들기


이 비디오에서는 다음을 학습합니다.

* 텍스트 모드는 무엇입니까?
* 낙타의 예는 무엇인가요
* 보기에서 사용할 수 있는 몇 가지 기본적인 &quot;플러그 앤 플레이&quot; 텍스트 모드

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## 작업 - 상위 4개 보기

먼저 작업 이름과 상위 이름에 대한 열을 만든 다음 다음 텍스트 모드를 사용하여 다른 세 개의 열을 만듭니다.

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

### 작업 - 상위 이름의 상위 상위

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

![4개의 상위 보기를 보여주는 화면 이미지](assets/4-parents-view.png)

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

### 사용자 - 기본 작업을 보여주는 모든 작업 역할

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
>UI를 통해 액세스할 수 있는 팀 필드에는 쉼표로 구분된 모든 팀이 표시되지만, 위의 텍스트 모드를 사용하면 각 팀이 별도의 행에 표시됩니다.


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


### 사용자 - 직접 보고서

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### 사용자 - 미래 유급휴가

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

![사용자 목록 보기를 보여주는 화면 이미지](assets/user-lists-view-large.png)

## 작업 - 태스크 지정 및 상태 작업 표시 방법

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

![지정 및 상태 보기를 보여주는 화면 이미지](assets/assignments-and-status-view.png)


## 작업 - 여러 태스크 지정에 역할 및 할당을 표시하는 방법

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

### 작업 - 지정 + 퍼센트 할당

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![지정 및 역할 보기를 보여주는 화면 이미지](assets/assignments-roles-and-percent-view.png)

## 작업 - 교차 프로젝트 선행 작업 및 후속 작업

### 작업 필터(선택 사항)

**프로젝트 간 선행 작업이 하나 이상 있는 모든 작업 표시**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### 작업 - 이전 이름 및 프로젝트 선행 작업이 다음 위치에 있음

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

### 작업 - 후속 이름 및 프로젝트 승계인이 다음 위치에 있음

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

### 작업 - 선행 작업의 예상 완료 날짜 표시

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

### 작업 - 선행 작업의 진행 상태 표시

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

### 작업 - 교차 프로젝트 이전 프로젝트의 완료율 표시

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

![크로스 프로젝트 선행 작업 및 후속 작업 보기를 보여주는 화면 이미지](assets/cross-project-predecessors-and-successors.png)


## 작업 - 지정된 모든 사용자와 각 작업을 지정한 사람을 표시하는 반복

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![할당되고 각 대상자를 지정한 모든 사람을 보여주는 화면 이미지입니다](assets/all-assignees-and-requesters.png)

## 작업/프로젝트 - 프로젝트 또는 작업의 모든 사용자 정의 양식을 표시하는 반복

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![프로젝트의 모든 사용자 지정 양식을 표시하는 화면 이미지입니다](assets/all-custom-forms-on-a-project.png)


## 프로젝트 - 프로젝트 보기에서 해결 가능 파일의 모든 주요 연락처를 표시하는 반복

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

![해상도의 기본 연락처를 보여주는 화면 이미지입니다.](assets/primary-contacts-for-resolvables.png)

## 프로젝트 - 모든 프로젝트 팀 멤버를 표시하는 반복

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

![모든 프로젝트 팀 구성원을 보여주는 화면 이미지입니다.](assets/all-project-team-members.png)

## 프로젝트 - 프로젝트의 모든 해결 가능한 문제의 entryDate를 보여 주는 반복

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

![프로젝트에 대한 모든 해결 가능한 문제의 entryDate를 보여 주는 화면 이미지입니다](assets/resolvables-entry-date.png)

## 프로젝트 - 원래 프로젝트 요청자의 홈 그룹을 표시합니다.

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![프로젝트 요청자 홈 그룹을 보여주는 화면 이미지입니다.](assets/requestor-home-group.png)

## 프로젝트 - 프로젝트가 요청 큐인지 표시

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

![프로젝트가 요청 큐인지 여부를 보여주는 화면 이미지입니다](assets/project-is-a-request-queue.png)

## 문제 - 모든 해결 프로젝트 팀 멤버를 보여 주는 반복

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

![모든 해결 프로젝트 팀 구성원을 보여주는 화면 이미지입니다.](assets/all-resolve-project-team-members.png)

## 문제 - 문제 주요 연락처의 모든 팀을 보여 주는 반복

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

![모든 기본 연락처 팀을 보여주는 화면 이미지](assets/all-primary-contact-teams.png)

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

![문서 보고서의 폴더를 표시하는 화면 이미지](assets/folder-in-a-document-report.png)

## 문서 - 문서 보고서의 상위 폴더를 표시하는 반복

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![문서 보고서의 상위 폴더를 표시하는 화면 이미지입니다](assets/parent-folder-in-a-document-report.png)

## 문서 - 문서 승인 날짜

```
displayname=Document Approval Dates
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

![문서 승인 날짜 보기를 보여주는 화면 이미지](assets/document-approval-dates.png)

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

![증명 승인의 프로젝트 및 작업을 보여주는 화면 이미지](assets/proof-approval-project-and-task.png)

