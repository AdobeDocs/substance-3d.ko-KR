---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-displacement-ue4.html"
breadcrumb-title: ''
description: 표면 세부 묘사를 위해 Unreal Engine 4의 Substance 재질에서 변위 맵을 사용하고 테셀레이션을 활성화합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Displacement - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 변위 작업 - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# 변위 작업 - UE4

변위 작업을 하려면 재질에 쪽맞춤을 활성화해야 합니다.

![](../../../../assets/tess.png){width="600px"}

Height 출력을 사용하려면 Substance 팩토리 인스턴스에서 출력을 두 번 클릭하여 Height을 만들어야 합니다. Height은 기본적으로 활성화되어 있지 않습니다. 그런 다음 이 Height 출력을 재질로 드래그할 수 있습니다.

![](../../../../assets/height-1.png){width="800px"}

재료에 Height 출력을 추가한 후에는 World 변위 및 Tessellation Modifier를 구동하는 몇 개의 노드를 만들어야 합니다.

1. 2개의 스칼라 매개 변수를 만듭니다. 하나는 거리가 될 것이고 다른 하나는 쪽맞춤을 위한 승수가 될 것이다.
1. Height에서 Distance 매개 변수까지 빨강 채널을 곱합니다
1. VertexNormalWS 노드를 추가하고 2단계에서 곱의 출력으로 이 값을 곱합니다.
1. VertexNormal의 곱을 재질 상의 세계 변위에 입력합니다.
1. 테셀레이션 멀티플라이어 매개 변수를 가져와 소재에 있는 테셀레이션 멀티플라이어에 입력합니다.

![](../../../../assets/setup-3.png){width="800px"}

>[!NOTE]
>
> 다른 텍스처 출력은 그래프를 단순화하기 위해 이 이미지에서 생략했습니다. 여기에서는 명확성을 위해 변위 및 멀티플라이어 노드만 표시됩니다.
