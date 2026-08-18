---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-bump-offset-parallax-ue4.html"
breadcrumb-title: ''
description: Unreal Engine 4에서 Substance 재료로 범프 오프셋 매핑(Bump Offset mapping)을 사용하여 깊이 착시 및 표면 세부 정보를 생성합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Bump Offset (Parallax) - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 범프 오프셋 작업(시차) - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# 범프 오프셋 작업(시차) - UE4

**범프 오프셋** 매핑을 사용하면 UV 좌표를 창의적인 방식으로 수정하여 표면에 깊이가 있는 것처럼 보이게 할 수 있으므로 개체의 표면에서 텍스처가 더 멀리 떨어지게 할 수 있으며 표면에 실제 표면보다 더 많은 세부 사항이 있는 것처럼 보이게 할 수 있습니다. 이 방법(How To) 예제에서는 범프 오프셋 재료 표현식을 찾는 방법뿐만 아니라 재료에서 범프 오프셋 노드를 활용하는 방법도 다룹니다.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/HowTo/BumpOffset/>

Height 출력을 사용하려면 Substance 팩토리 인스턴스에서 출력을 두 번 클릭하여 Height을 만들어야 합니다. Height은 기본적으로 활성화되어 있지 않습니다. 그런 다음 이 Height 출력을 재질로 드래그할 수 있습니다.

![](../../../../assets/height-1.png){width="600px"}

범프 오프셋 노드를 만든 다음 Height의 빨강 채널을 Height에 연결합니다. 그런 다음 범프 오프셋의 좌표 입력에 텍스트 좌표를 제공할 수 있습니다. 마지막으로, 범프 오프셋의 출력은 모든 Substance 텍스처에 대한 UV 입력에 플러깅된다.

![](../../../../assets/bump.png){width="800px"}
