---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/octane/octane-for-modo.html"
breadcrumb-title: ''
description: 라이브 DB 재질 및 적절한 출력 구성을 통해 MODO에서 Octane 렌더러와 함께 Substance 재질을 사용합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Octane > Octane for MODO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MODO용 옥탄
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# MODO용 옥탄

## MODO 플러그인의 Substance

Substance 출력은 Octane을 사용하여 기본적으로 작동합니다. 다음 Substance 출력 및 텍스처 레이어 효과 구성을 사용할 수 있습니다.

1. Substance 만들기>텍스처>Substance 만들기 를 선택하고 모드를 [비실제 재질]로 설정합니다. 언리얼 재질을 사용하면 고급 OGL 뷰포트에서 텍스처를 볼 수 있습니다.
1. 기본 색상, 금속, 거칠기 및 표준의 출력을 만듭니다.
1. MODO는 OGL 노멀 맵을 사용합니다. Substance 속성에서 일반 방향을 OpenGL로 변경해야 합니다.

   ![](../../../assets/ogl.png)
1. Substance PBR 사전 설정을 로드합니다. 이 사전 설정은 옥탄 재정의입니다. 셰이더 그룹으로 드래그합니다.

   [Substance\_PBR.lxp](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/integrations/files/162005234/162005272/1/1502792782697/substance-pbr.lxp)
1. 재정의를 선택하고 클립 브라우저의 Substance 출력을 도식 보기로 드래그합니다. 파일 이름이 출력 된 노드를 가져와서 적절한 입력 노드(예: 기본 색상 → 기본 색상)에 연결합니다.

   ![](../../../assets/connect-6.png)
1. 나머지 Substance 출력 연결

   ![](../../../assets/outputs-4.png){width="640px"}
