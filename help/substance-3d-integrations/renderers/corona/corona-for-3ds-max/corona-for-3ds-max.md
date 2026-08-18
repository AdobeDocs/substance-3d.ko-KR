---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/corona/corona-for-3ds-max.html"
breadcrumb-title: ''
description: 3ds Max에서 Specular/광택 작업 과정 및 필수 맵을 사용하여 Corona 렌더러와 함께 Substance 재질을 사용하세요.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona > Corona for 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max용 Corona
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# 3ds Max용 Corona

## Maya 플러그인의 Substance

![](../../../assets/scene-001v03.jpg)

## Corona 1.6 - 6

[3ds Max 플러그인](../../../3d-applications/3ds-max/3ds-max.md)을 사용하면 Substance 메뉴에서 Corona를 선택하여 Substance 텍스처 입력을 사용하여 Corona 재질을 자동으로 설정할 수 있습니다.

![](../../../assets/corona.png){width="500px"}

## 코로나 7 - 9

코로나 렌더링 7 이상에서는 Substance2 노드가 선택된 상태에서 &quot;코로나로의 Substance&quot;를 선택하면 코로나 물리적 자료에 대한 네트워크가 생성됩니다.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/corona-physical-material?$png$&jpegSize=200&wid=857)

* 기본 색상 출력과 기본 색상 입력 사이에 **LiftGamaGain**&#x200B;이(가) 만들어집니다. 색상 차이를 보정하기 위해 감마 값 0.455가 사용됩니다.
* **CoronaNormal**&#x200B;은(는) Normal 출력과 Base 범프 입력 사이와 Coat Normal 출력과 Clearcoat Bump 입력 사이에 생성됩니다. 설정은 변경되지 않지만 일반은 여기에서 수정할 수 있습니다.
* 광택 색상 출력과 광택 색상 입력 사이에 **CoronaMix**&#x200B;이(가) 만들어집니다. 기본 레이어의 혼합량 0, 승수 2 설정 사용자는 [혼합 양] 값을 조정하여 광택을 조절할 수 있습니다.
