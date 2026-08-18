---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5.html"
breadcrumb-title: ''
description: Unreal Engine 5에서 재료 템플릿을 생성하고 사용하여 Substance 출력 노드가 재료 입력에 연결되는 방법을 정의합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 재료 템플릿 사용 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# 재료 템플릿 사용 - UE5

재료 템플릿을 사용하면 출력 노드를 재료의 입력에 연결하기 위한 템플릿으로 사용할 재료 기본 재질을 만들 수 있습니다.\
재료 입력과 동일한 이름 및 유형을 공유하는 출력이 자동으로 사용됩니다. 이 상위 재질 예에는 &quot;baseColor&quot;라는 텍스처 출력이 있는 Substance의 경우 채워질 &quot;baseColor&quot; 텍스처 샘플 노드가 있습니다.\
![](../../../../assets/parent-material-sample.png)

Substance 출력은 텍스처, 단일 부동 소수점 또는 int 스칼라 값, 벡터(2~4) 값 업데이트를 지원합니다. 런타임에 float 또는 int 출력을 사용하려면 그래프에서 dynamicMaterialInstance를 constantMaterialInstances(편집기에서 생성된 모든 재질)로 가져와야 런타임에 스칼라 값을 변경할 수 없습니다.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/scalar-value?$png$&jpegSize=100&wid=245)

Substance Graph 인스턴스는 생성 시 모든 관련 출력 값을 채우려고 시도합니다.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-04-01-at-4-38-31-pm?$png$&jpegSize=200&wid=1076)
