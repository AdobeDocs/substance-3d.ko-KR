---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/using-workflows-in-3ds-max.html"
breadcrumb-title: ""
description: 3ds Max의 렌더링 워크플로우를 사용하여 Substance 재질에서 다른 렌더러에 대한 셰이더 네트워크를 자동으로 만들 수 있습니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Using Workflows in 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max에서 워크플로우 사용
user-guide-description: ""
user-guide-title: ""
source-git-commit: 335f3107fb325bb769325bff8c150b3e8b7ff054
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%
---

# 3ds Max에서 워크플로우 사용

3ds Max 플러그인의 Substance은 렌더러를 지원하기 위해 셰이더 네트워크를 자동으로 만들기 위한 워크플로를 포함합니다. 렌더링 워크플로우는 Substance 메뉴에서 찾을 수 있습니다.

![](../../../assets/maya-max-v3-1/3dsmax-all-presets.png)

워크플로우를 사용하려면 재료 편집기에서 Substance 노드를 선택한 다음 Substance 메뉴에서 워크플로우를 선택합니다.

![](../../../assets/max-workflow.gif)

## OpenPBR 작업 과정

**Substance 메뉴**&#x200B;의 **작업 과정 목록**&#x200B;에서 **OpenPBR에 Substance** 및 **V-Ray OpenPBR에 Substance**&#x200B;의 두 가지 OpenPBR 작업 과정을 사용할 수 있습니다. 이러한 워크플로우는 Substance 3D Designer 또는 Sampler에서 OpenPBR 재질 모델을 사용하여 작성된 SBSAR 파일에 사용하도록 설계되었습니다(Designer V16.0+ 및 Sampler V6.0+ 이후 OpenPBR이 기본 모델임).

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-node-preview.png)

### OpenPBR 소개

OpenPBR은 Adobe과 오토데스크가 개발하고 ASWF(Academy Software Foundation)에 기여한 개방형 물리적 소재 음영 모델입니다. 렌더러 간에 호환되는 통합된 재질 정의를 제공합니다. 자세한 내용은 [OpenPBR 설명서](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/openpbr/openpbr-overview)를 참조하십시오.

### OpenPBR 워크플로우를 사용하는 경우

Substance 3D Designer 또는 Substance 3D Sampler에서 OpenPBR 재질 모델을 사용하여 SBSAR 파일을 만든 경우 OpenPBR 워크플로를 사용하십시오. SBSAR가 Adobe 표준 재질 모델(ASM)을 사용하여 작성된 경우 렌더러와 호환되는 레거시 워크플로우(Arnold, V-Ray 또는 V-Ray 6)를 사용합니다.

>[!NOTE]
>
> ASM 재료에 OpenPBR 워크플로우를 적용하거나 OpenPBR SBSAR에 표준 워크플로우를 적용하면 플러그인에서는 두 재질 모델에 공통적인 출력만 접속합니다. 결과가 완전하지 않을 수 있습니다.

### 사용 가능한 OpenPBR 워크플로우

**OpenPBR**

네이티브 3ds Max openPBRSurface 노드를 사용합니다. 아놀드, 브이레이와 호환됩니다. 3ds Max에서 OpenPBR 재질을 사용하여 작업하는 대부분의 사용자에게 권장되는 워크플로입니다.

**OpenPBR - V-레이**

OpenPBR 모드에서 V-Ray 재질(VRayMtl)을 사용합니다. 파이프라인이 V-Ray 재질 설정을 중심으로 특별히 제작된 사용자에게 권장됩니다.

### OpenPBR 작업 과정을 적용하는 방법

![](../../../assets/maya-max-v3-1/3dsmax-substance-to-openpbr.png)

1. [Substance 불러오기] 단추를 사용하여 SBSAR 파일(OpenPBR)을 선택합니다.
1. 상단 메뉴에서 OpenPBR 또는 OpenPBR - V-Ray 를 선택합니다.
1. 네트워크 생성(Create Network)을 클릭하여 Slate Material Editor에서 셰이더 네트워크를 생성합니다.
1. 플러그인은 SBSAR 출력들을 OpenPBR 노드의 대응하는 입력들에 자동으로 연결한다.
1. 평소와 같이 메시에 재질을 할당합니다.

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-overview.png)
