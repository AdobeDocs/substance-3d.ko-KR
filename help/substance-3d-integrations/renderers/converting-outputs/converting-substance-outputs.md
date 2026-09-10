---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/converting-substance-outputs.html"
breadcrumb-title: ''
description: 다양한 렌더러 요구 사항 및 워크플로우에 맞게 Substance 재질 출력을 변환하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Converting Substance outputs
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 출력 변환
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# Substance 출력 변환

## Substance Painter

변환된 맵을 Substance Painter에서 내보낼 수 있습니다. 다양한 렌더링 사전 설정이 지원되며 사전 설정을 선택하면 지도 유형이 변환됩니다. 변환은 metal/rough 워크플로우를 기반으로 합니다.

![](../../assets/convertpainter.png){width="800px"}

## Substance 플러그인

Substance 플러그인은 출력을 생성하고 특정 작업 과정에 대한 재질을 자동으로 만듭니다. 그러나 DCC 응용 프로그램 및 타사 렌더러의 경우 금속성/러프 출력을 수동으로 변환해야 할 수 있습니다. 다음 통합은 자동 렌더링 워크플로우를 지원하며 필요한 경우 모든 맵 유형을 적절하게 변환합니다.

* [마야의 Substance](../../3d-applications/maya/using-workflows/using-workflows.md)
* [최대 3ds의 Substance](../../3d-applications/3ds-max/3ds-max.md)

## 사용자 정의 Substance

사용자 정의 Substance을 작성하는 경우 Vray 및 Corona와 같은 렌더러에 필요한 특정 출력을 만들 수 있습니다. 금속/거칠기 변환 노드([라이브러리]&gt;[PBR 유틸리티])를 사용하면 기본 색상, 거칠기 및 금속 맵을 특정 렌더러로 쉽게 변환할 수 있습니다.

![](../../assets/convert-designer.png){width="600px"}
