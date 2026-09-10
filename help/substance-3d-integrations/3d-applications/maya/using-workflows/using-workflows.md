---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ''
description: Maya에서 Substance 출력에 대한 렌더링 사전 설정을 만들고 사용하여 다양한 렌더러에 대한 셰이더 네트워크를 자동으로 생성합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 워크플로우 사용
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# 워크플로우 사용

[작업 과정]에서 Substance 출력에 대한 렌더링 사전 설정을 선택하거나 만들 수 있습니다. 이러한 사전 설정은 Arnold 또는 Vray 같은 렌더러의 셰이더 네트워크입니다.

>[!NOTE]
>
> **워크플로 사전 설정 위치**
> 
> **Windows**:\
> C:\Users\\Documents\maya\2022\substance\workflows\generated\
> **MacOS**:\
> /Users//Library/Preferences/Autodesk/maya//substance/workflows/generated\
> **Linux**:\
> /home//maya//substance/workflows/generated

![](../../../assets/workflows-4.png)

워크플로우를 사용하려면 드롭다운 목록에서 사전 설정을 선택한 다음 셰이더 네트워크 만들기 버튼을 클릭하면 됩니다.

![](../../../assets/workflow.gif)

## 워크플로우 만들기

나만의 워크플로우를 만들어 렌더러 워크플로우 목록에 추가할 수 있습니다. 새 워크플로우를 추가하면 Substance 노드 이후에 생성된 모든 노드가 워크플로우에 저장됩니다. 이렇게 하면 원하는 수의 음영 노드를 만들어 사전 설정 워크플로로 저장할 수 있는 완전한 사용자 지정 셰이더 네트워크를 만들 수 있습니다.

## ![](../../../assets/saved-workflow.png) 워크플로 관리

### 사용자 정의 작업 과정 저장

1. Substance 출력을 수동으로 만들고 aiStandardSurface와 같은 재질에 연결합니다.
   1. Maya나 렌더링 특정 노드를 사용하여 셰이더 네트워크를 만들 수 있습니다.
1. **작업 과정 만들기** 단추를 클릭하고 작업 과정 사전 설정의 이름을 입력합니다.

### 작업 과정 복제

**워크플로 복제** 단추를 클릭하여 워크플로를 복제할 수 있습니다.

### 워크플로우 이름 바꾸기 및 덮어쓰기

**이름 바꾸기** 및 선택한 **덮어쓰기** 단추를 사용하여 기존 작업 과정의 이름을 바꾸고 업데이트된 데이터로 작업 과정을 덮어쓸 수 있습니다.

### 워크플로우 제거

워크플로우 제거 버튼을 사용하여 기존 워크플로우를 제거할 수 있습니다.
