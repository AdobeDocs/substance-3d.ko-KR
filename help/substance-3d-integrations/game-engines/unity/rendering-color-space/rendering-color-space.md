---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/rendering-color-space.html"
breadcrumb-title: ''
description: 실제 기반 셰이더를 사용하여 Substance 재질이 제대로 렌더링되도록 Unity의 색상 공간 설정을 구성합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Rendering Color Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 색상 공간 렌더링 중
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# 색상 공간 렌더링 중

Substance 텍스처는 물리적 기반 셰이더와 함께 사용되도록 설계되었습니다. 최상의 결과를 얻으려면 Unity Player 설정에서 색상 공간을 Linear로 설정해야 합니다.

1. 편집>프로젝트 설정>플레이어로 이동
1. [렌더링] 섹션에서 색상 공간을 [선형]으로 변경합니다. Unity는 기본적으로 감마 공간을 사용하는데, 감마 공간이 잘못되어 텍스처 색상이 잘못 표시됩니다.

   >[!NOTE]
   >
   > **정보**
   > 
   > Unity의 색상 공간 설정이 [감마]로 설정된 경우 텍스처의 sRGB 옵션이 비활성화됩니다

   ![](../../../assets/rendering-4.png){width="600px"}
