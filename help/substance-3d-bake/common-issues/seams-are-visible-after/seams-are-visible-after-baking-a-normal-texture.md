---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: 패딩, 앤티 앨리어싱 및 UV 레이아웃을 조정하여 구운 표준 텍스처에서 보이는 이음새를 제거하세요.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 일반 텍스처를 굽은 후 솔기가 보임
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 일반 텍스처를 굽은 후 솔기가 보임

>[!WARNING]
>
> **문제**
> 
> 노멀 맵 솔기는 깔끔하게 구워진 후에도 메쉬의 UV 테두리에서 볼 수 있습니다.

>[!NOTE]
>
> **설명**
> 
> 완전히 구워진 후에도 솔기가 여전히 보일 수 있습니다. 주된 이유는 텍스처에 대한 일반적인 대략적인 표면 정보입니다. 때때로 텍스처는 정밀도가 부족하거나 충분히 정확하기 위해 낮은 폴리 기하학과 높은 폴리 기하학 사이에 너무 많은 것을 보상해야 한다. 일부 다른 상황에서는 기하학이 노멀 맵으로 맞춰지는 방식이 외관의 품질에 영향을 줄 수 있습니다.

>[!NOTE]
>
> **해결 방법**
> 
> 노멀 맵을 사용하여 이음새 강도를 줄이기 위해 몇 가지 가능한 해결 방법을 시도할 수 있습니다.
> 
> * 종종 UV가 픽셀에 정렬되지 않아 앨리어싱이 발생하고 솔기가 생성됩니다. 자세한 내용은 [이 페이지](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)를 참조하세요.
>   * 텍스처 해상도를 높이는 것이 이러한 효과를 줄이는 방법이 될 수 있다.
>   * 이 효과를 줄이기 위한 또 다른 방법으로 UV 테두리를 픽셀에 정렬할 수 있습니다.
> * 셰이더 **품질** 설정을 늘립니다. 셰이더 품질은 Specular 반사의 계산 방법에 영향을 줄 수 있습니다. 일부 UV 섬이 회전되고 이 매개 변수가 너무 낮으면 가시적인 이음새가 생길 수 있습니다. 자세한 내용은 [이 페이지](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html)를 참조하세요.
