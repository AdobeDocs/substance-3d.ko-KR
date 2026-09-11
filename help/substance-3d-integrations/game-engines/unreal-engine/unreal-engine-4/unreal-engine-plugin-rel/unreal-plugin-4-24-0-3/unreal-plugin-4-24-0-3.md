---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/unreal-engine-4-plugin-release-notes/unreal-plugin-4-24-0-3.html"
breadcrumb-title: ''
description: Unreal Engine 4 플러그인 버전 4.24.0.3에 대한 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Unreal Engine 4 plugin release notes > Unreal plugin 4.24.0.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unreal 플러그인 4.24.0.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Unreal 플러그인 4.24.0.3

언리얼 엔진 Substance이 대대적인 구조조정을 단행했다. 이 구조의 일부는 **UTexture2D**&#x200B;을(를) 완전히 지원하며 입력과 출력을 모두 포함합니다. **UTexture2D**&#x200B;를 지원하므로 이제 플러그인을 사용하여 모바일을 포함한 언리얼 지원 플랫폼에 게시할 수 있습니다. 다중 플랫폼 지원 추가와 함께 **UTexture2D**&#x200B;도 UE4 내에서 텍스처 스트리밍 시스템의 기본 사용을 허용합니다.

또한 이 플러그인은 재질 **인스턴스**&#x200B;에 대한 완전한 지원을 제공하고 Substance 엔진에서 지원하는 숫자 출력을 사용하는 새 재질 템플릿 워크플로를 도입합니다. 재질 템플릿을 사용하면 UE4에서 Substance 재질 셰이더를 구성하는 방법을 정확하게 정의할 수 있습니다.

![](../../../../../assets/ue4-material-templates.png)

우리는 타일링, 텍스처 크기, 변위 및 방출 파라미터를 조정하기 위한 컨트롤이 내장된 변위, 굴절 및 세계 맞춤 재료 작업을 위한 템플릿을 함께 제공합니다. 재질 템플릿 시스템을 사용하여 사용자 정의 템플릿을 제공할 수도 있습니다.

![](../../../../../assets/ue4-material-instance-params.png)
