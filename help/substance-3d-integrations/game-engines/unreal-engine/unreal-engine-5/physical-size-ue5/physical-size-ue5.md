---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/physical-size-ue5.html"
breadcrumb-title: ''
description: 물리적 크기 설정을 사용하여 Unreal Engine 5의 실제 치수를 기반으로 Substance 재료의 크기를 조정합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Physical Size - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 물리적 크기 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# 물리적 크기 - UE5

Substance 재질에 물리적 크기를 사용하면 재질이 세계에서 차지하는 크기에 따라 크기를 조정할 수 있습니다. 이 값은 Substance Designer으로 설정되고 재료 템플릿 시스템을 통해 Unreal로 읽힙니다.\
상위의 [Substance\_Triplanar\_Template](../../../../game-engines/unreal-engine/unreal-engine-5/material-template-usage/out-the-box-material-tem/out-of-the-box-material-templates.md) 재질에는 물리적 크기를 사용하여 언리얼 재질을 확장하는 방법의 예제가 포함되어 있습니다.



메시의 업스케일링 값에 관계없이 재질은 세계에서 차지하는 크기(센티미터)에 따라 타일링됩니다. 암석(그림 1)의 경우, 측정 때마다 1.8m(180cm) 크기이다.

![](../../../../assets/rock-material-parameters.png)

물리적 크기 데이터를 포함하는 Substance 재질은 해당 값을 physicalsize라는 기존의 재료 벡터 매개변수 노드에 복사합니다.



UE5의 재료들에 변위 값이 없기 때문에, 물리적 크기 템플릿은 삼면형 맵에 대한 값을 X, Y, X로서 복사한다.
