---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/renderers/corona.html"
breadcrumb-title: ''
description: 3ds Max에서 Specular/광택 작업 과정 및 필수 맵을 사용하여 Corona 렌더러와 함께 Substance 재질을 사용하세요.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 코로나
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 1%

---


# 코로나

Corona로 렌더링하는 경우에는 Substance Painter 또는 Substance 플러그인에서 내보낸 맵을 사용할 수 있습니다. Corona는 1/IOR 맵과 함께 Specular/광택 작업 과정을 사용하고 있습니다. 다음 지도가 필요합니다.

* 확산
* 반사(Specular)
* 광택
* 1/IOR(변환됨)

1/IOR 맵은 Substance Designer 및 Substance Painter 모두의 기본 작업 과정인 금속/거칠기 작업 과정에서만 변환할 수 있습니다.

1. 코로나 사전 설정을 사용하여 Substance Painter에서 맵을 내보냅니다.
1. 사용자 정의 Substance의 경우 Vray 사전 설정으로 설정된 basecolor\_metallic\_roughness 변환 노드를 사용하여 사용자 정의 출력을 만들 수 있습니다.
1. 3ds Max 및 Cinema 4D의 경우 레이어가 있는 코로나 재질을 사용하여 금속 및 유전체 재질을 처리하고 1/IOR 맵을 변환하지 않아도 됩니다.

## 목차

* [3ds Max용 Corona](../../renderers/corona/corona-for-3ds-max/corona-for-3ds-max.md)
* [코로나 - Substance Painter](../../renderers/corona/corona-painter/corona-substance-painter.md)
