---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/tiling-substance-ue4.html"
breadcrumb-title: ''
description: 텍스처 좌표 노드 및 스칼라 매개 변수를 재질에 추가하여 Unreal Engine 4에서 타일 Substance 텍스처를 만듭니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Tiling Substance - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 타일링 Substance - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '77'
ht-degree: 0%

---


# 타일링 Substance - UE4

Substance 텍스처를 바둑판식으로 배열하려면 [텍스처 좌표] 노드를 추가하고 여기에 스칼라 매개 변수를 곱해야 합니다.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/ExpressionReference/Coordinates/#texturecoordinate>

U와 V 타일 모두에 대한 매개 변수를 만들려면 [추가 벡터]를 사용하고 이를 TexCoord로 곱할 수 있습니다. 이를 통해 U와 V 타일 양을 독립적으로 설정할 수 있습니다.

![](../../../../assets/tiling-3.png){width="800px"}
