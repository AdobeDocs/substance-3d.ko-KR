---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/maya/settings.html"
breadcrumb-title: ''
description: 동작을 사용자 정의하려면 [Substance 모음] 또는 메뉴를 통해 Maya에서 Substance 플러그인 설정을 구성합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 설정
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---


# 설정

Substance 설정 메뉴는 Substance 셸프 또는 Substance 메뉴를 통해 액세스할 수 있습니다. 이 메뉴의 설정은 편집 가능한 구성 파일 &quot;substance.cfg&quot;에 저장됩니다.

>[!NOTE]
>
> **구성 파일 위치**
> 
> **Windows**:\
> C:\Users\\Documents\maya\\substance\\
> **MacOS**:\
> /Users//Library/Preferences/Autodesk/maya//substance/\
> **Linux**:\
> /home//maya//substance/

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## 기본 해상도

sbsar 파일을 로드할 때 Substance 노드의 기본 해상도를 설정합니다.

## 렌더링 워크플로우

Substance 노드에서 사용할 기본 렌더링 작업 과정을 설정합니다.

## Substance 엔진

모든 Substance 노드에 대한 Substance 엔진 및 전역 관련 환경 설정 지정 Substance 엔진은 Substance 텍스처를 계산하는 데 사용됩니다.

### 엔진 유형

이 Substance 엔진은 CPU 및 GPU 엔진으로 사용할 수 있습니다. 엔진을 바꾸려면 Maya를 다시 시작해야 합니다. GPU 엔진은 CPU 엔진보다 높은 해상도를 허용합니다.

>[!WARNING]
>
> CPU와 GPU 엔진 간에 컴퓨팅 차이가 있을 수 있으므로 일관된 결과를 얻으려면 Substance Designer에 사용되는 엔진과 동일한 유형으로 설정하는 것이 가장 좋습니다.

CPU 코어 및 엔진 메모리는 Substance 엔진에서 사용할 수 있는 리소스 양에 대한 설정입니다.

### 렌더링 차단

이 옵션을 사용하면 Substance 엔진 계산이 Maya UI 프로세스를 차단할지 여부를 설정할 수 있습니다. 활성화되면 Substance 엔진이 우선하여 Maya UI 프로세스를 차단합니다. 비활성화하면 Maya UI 프로세스가 Substance 엔진 계산에 의해 차단되지 않습니다.

## 출력을 디스크로 캐시

프로젝트에서 새로 만든 모든 Substance 노드의 기본 캐시 위치, 파일 유형 및 캐시 폴더를 설정합니다.

## 렌더링 확장 프로그램

아놀드 셰이더와 함께 Substance 출력을 직접 사용하려면 렌더링 확장을 활성화합니다.

## 실제 크기

sbsar 파일을 로드할 때 기본적으로 물리적 크기를 사용해야 하는지 여부 및 sbsar을 다시 로드할 때 다시 계산해야 하는지 여부를 활성화합니다.

</td>
<td style="border: 0;" valign="top">

![](../../../assets/settings-35.png)

</td>
</tr>
</table>
