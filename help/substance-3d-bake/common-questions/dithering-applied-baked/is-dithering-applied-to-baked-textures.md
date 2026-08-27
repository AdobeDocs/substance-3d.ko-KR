---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: 디더링이 구운 텍스처에 적용되는지 여부와 텍스처 품질에 미치는 영향을 파악합니다.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: '디더링이 구운 텍스처에 적용됩니까? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# 구운 텍스처에 디더링이 적용되나요?

>[!WARNING]
>
> **질문**
> 
> 베이커가 텍스처 [디더링](https://en.wikipedia.org/wiki/Dither)을 지원합니까? 그렇다면 언제 적용됩니까?

>[!NOTE]
>
> **설명**
> 
> 8비트 노멀 맵에서 밴딩을 방지하기 위해 디더링이 적용됩니다. 예:
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **해결 방법: Substance Designer**
> 
> 디더링은 다음과 같은 경우에 자동으로 적용됩니다.
> 
> * Baker 출력이 8비트 텍스처 파일에 저장되는 경우
> * 8비트로 설정된 그래프의 비트맵 노드에서 Baker 출력을 사용할 경우

>[!NOTE]
>
> **해결 방법: Substance Painter**
> 
> 디더링은 내보내기 프로세스 중에 활성화하거나 비활성화할 수 있는 옵션입니다. 표준, 변위 및 Height 채널에 대해 8비트 파일 형식으로 내보낼 때만 적용됩니다.

>[!NOTE]
>
> **솔루션 : Substance 자동화 툴킷**
> 
> 지금은 디더링이 지원되지 않습니다.
