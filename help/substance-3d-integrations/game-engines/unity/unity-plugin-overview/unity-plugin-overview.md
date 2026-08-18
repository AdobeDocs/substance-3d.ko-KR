---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-plugin-overview.html"
breadcrumb-title: ''
description: 버전 지원, 기능 및 통합 기능을 포함하여 Unity용 Substance 3D 플러그인에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Plugin Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 플러그인 개요
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Unity 플러그인 개요

## Unity 버전 지원

Unity용 Substance 3D 플러그인 버전 3.0.0 Adobe은 현재 Unity 2020 LTS 이상을 지원합니다.

## Substance 패키지 다운로드

1. 플러그인은 Unity Asset Store <https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208>에서 다운로드할 수 있습니다.

## Substance 재료 가져오기

1. 프로젝트 창을 마우스 오른쪽 버튼으로 클릭하고 에셋 가져오기를 선택하거나 프로젝트 보기 패널로 가져올 Substance 재질을 드래그합니다.
1. 가져올 Substance 재질을 찾습니다. Substance 재질은 &quot;.sbsar&quot; 파일 확장명을 가집니다.
1. Substance 재질을 Unity 프로젝트로 가져옵니다.

   1. sbsar 에셋은 메인 가져오기 파일과 출력 텍스처 및 생성된 Unity 재질을 포함하는 폴더를 만듭니다.
1. 그런 다음 장면 보기에서 메시에 재질을 드래그 앤 드롭한 다음 검사기에서 매개 변수를 편집할 수 있습니다.

   ![](../../../assets/window-overview.png){width="1000px"}

>[!NOTE]
>
> **표준 맵 변환**
> 
> Unity 플러그인의 Substance은 자동으로 DirectX을 OpenGL로 변환합니다. [Substance Source](https://source.substance3d.com/)의 재질을 사용할 때 일반 방향을 OGL로 변경할 필요가 없습니다. Substance Designer에서 자체 재질을 만드는 경우 플러그인이 일반 변환을 자동으로 처리하므로 기본 DirectX 셰이더로 작업해야 합니다. 자세한 내용은 Unity에서 Working with Normals를 확인하십시오.

## 매개변수 변경

속성 창에서 매개 변수 및 해결 방법을 설정할 수 있습니다. [매개 변수 변경](../../../game-engines/unity/changing-parameters/changing-parameters.md)을 참조하세요.

[unity\_tweaking\_parameters.mp4](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/download/attachments/186056716/unity-tweaking-parameters.mp4)

## Unity 렌더링 파이프라인 지원

Substance 3D 플러그인은 HDRP 및 URP를 지원합니다. 더 많은 정보가 곧 제공될 것입니다.

## 튜토리얼 방법
