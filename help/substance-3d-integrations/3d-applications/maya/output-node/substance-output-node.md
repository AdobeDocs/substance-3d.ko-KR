---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/maya/substance-output-node.html"
breadcrumb-title: ''
description: Maya에서 Substance 출력 노드가 계산된 텍스처를 셰이더 네트워크에 연결하는 방법을 이해합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance Output Node
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 출력 노드
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Substance 출력 노드

Substance 출력 노드는 Substance 엔진에서 계산된 텍스처에 대한 참조입니다. Substance 노드에 연결되어 있습니다. 출력이 Substance 노드에서 생성될 때, Substance 엔진은 텍스처를 계산하고 이 데이터는 RAM이다. GPU 엔진을 사용하는 경우, 데이터는 GPU에서 계산되고 Substance GPU 혼합 엔진을 사용하여 메모리로 다시 전송됩니다. 활성화되지 않은 Substance 노드의 출력은 계산되지 않습니다.

![](../../../assets/outputnode.png)

이 노드에서는 Substance Designer의 출력에 설정된 식별자, 레이블 및 사용과 같은 출력 정보를 볼 수 있습니다. 또한 이 노드를 사용하면 출력 캐싱 섹션에서 텍스처를 디스크로 베이킹할 수 있습니다.
