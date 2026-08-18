---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/blender/physical-size-in-blender.html"
breadcrumb-title: ''
description: 물리적 크기 설정을 사용하여 Blender의 실제 치수를 기반으로 Substance 재질의 비율을 조정합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Physical size in Blender
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 믹서기의 물리적 크기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# 믹서기의 물리적 크기

Substance 재질에 물리적 크기를 사용하면 재질이 세계에서 차지하는 크기에 따라 크기를 조정할 수 있습니다. 크기는 Designer과 같은 Substance 애플리케이션에서 설정되고 [플러그인] 패널의 물리적 크기 섹션에 표시됩니다.

![](../../../assets/blender-physical-size.png)

물리적 크기를 활성화하면 재질이 실제 크기(센티미터)를 기반으로 타일링됩니다. 재질 타일링은 오브젝트의 크기에 관계없이 동일하게 유지됩니다. 이 기능은 추가 기능 패널에서 물리적 크기 셰이더로 전환하여 활성화할 수 있습니다. 개체의 비율을 조정한 후 물리적 크기 텍스처를 정확하게 타일링하려면 비율을 ctrl/cmd+A로 적용해야 합니다.

## 물리적 크기 조정

매핑 노드의 값은 물리적 크기 타일링에 대한 예술적 제어를 위해 조정될 수 있다. 또한 [텍스처 좌표] 입력에 대해 [빈] 등의 개체를 사용하면 입력 개체의 변형을 사용하여 텍스처 매핑을 제어할 수 있습니다(아래 예제 참조).

![](../../../assets/blender-physical-szie-empty.gif)
