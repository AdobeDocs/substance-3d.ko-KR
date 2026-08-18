---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: 조각당 탄젠트 공간 계산 을 활성화하는 경우와 이것이 베이킹 결과에 미치는 영향에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Should I enable
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 활성화해야 함
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 1%

---


# &quot;조각당 탄젠트 공간 계산&quot;을 활성화해야 합니까?

>[!WARNING]
>
> **질문**
> 
> &quot;조각당 탄젠트 공간 계산&quot; 설정은 무엇을 의미하며 사용법은 무엇입니까?

>[!NOTE]
>
> **설명**
> 
> 이 설정을 활성화하면 베이커에서 Vertex Shader 대신 Fragment Shader(Pixel Shader라고도 함)에서 Tangent Space 계산을 수행할 수 있습니다. 계산이 정점에서 정점으로 보간되는 대신 픽셀별로 수행됨을 의미합니다. 이 설정은 일반 맵 제빵사가 텍스처를 인코딩하는 방법을 아는 데 사용됩니다. 그것은 또한 셰이더들이 텍스처를 읽어내는 방법을 알곤 했다.
> 
> 이 매개 변수를 사용하거나 사용하지 않으려면 보통 텍스처를 3D 뷰포트 및 렌더링 엔진(예: Iray)과 동기화하기 위해 다시 굽습니다.

>[!NOTE]
>
> **해결 방법**
> 
> 텍스처 렌더링의 대상이 되는 소프트웨어 또는 게임 엔진에 따라 다음 설정을 사용하지 않거나 사용할 수 있습니다.
> 
> | *소프트웨어* | *조각당 탄젠트 공간 계산* |
> | --- | --- |
> | **언리얼 엔진 4** | 활성화됨 |
> | **통합** | 비활성화 |
