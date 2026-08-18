---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: 패딩, 앤티 앨리어싱 및 UV 레이아웃을 조정하여 구운 표준 텍스처에서 보이는 실밥을 제거합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 일반 텍스처를 굽은 후 솔기가 나타납니다
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 일반 텍스처를 굽은 후 솔기가 나타납니다

>[!WARNING]
>
> **문제**
> 
> 정상적인 맵 솔기는 깔끔하게 굽은 후에도 메쉬의 UV 테두리에 표시됩니다.

>[!NOTE]
>
> **설명**
> 
> 완전히 구워진 후에도 솔기가 여전히 보일 수 있습니다. 일반적인 대략적인 표면 정보를 텍스처로 변환하는 것이 주된 이유입니다. 때때로 텍스처가 정밀도가 부족하거나 충분히 정확하기 위해 낮은 폴리 기하학과 높은 폴리 기하학 사이에 너무 많은 것을 보상해야 한다. 일부 다른 상황에서는 도형이 표준 지도와 일치하는 방식이 모양이 얼마나 좋아 보이는지에 영향을 줄 수 있습니다.

>[!NOTE]
>
> **해결 방법**
> 
> 몇 가지 가능한 해결 방법을 사용하여 표준 맵으로 이음새의 강도를 줄일 수 있습니다.
> 
> * 종종 UV가 픽셀에 정렬되지 않아 앨리어싱이 발생하고 솔기가 생성됩니다. 자세한 내용은 [이 페이지](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)를 참조하세요.
>   * 텍스처 해상도를 높이는 것이 이 효과를 감소시키는 방법이 될 수 있다.
>   * 이 효과를 줄이기 위한 또 다른 방법으로 UV 테두리를 픽셀에 정렬할 수 있습니다.
> * 셰이더 **품질** 설정을 늘립니다. 셰이더 품질은 Specular 반사의 계산 방법에 영향을 줄 수 있습니다. 일부 UV 섬이 회전되고 이 매개 변수가 너무 낮으면 가시적인 이음새가 생길 수 있습니다. 자세한 내용은 [이 페이지](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html)를 참조하세요.
