---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: 이름별 일치 또는 거리 조정을 사용하여 베이킹 중에 메시 부분이 서로 번지지 않도록 합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시 부분이 서로 간에 재단 물림
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# 메시 부분이 서로 간에 재단 물림

>[!WARNING]
>
> **문제**
> 
> 메시 형상이 다른 부품에서 번지고 가공물을 생성합니다.
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **설명**
> 
> 베이킹 프로세스는 매치를 생성하기 위해 낮은-폴리 메시 표면으로부터 광선을 보내 높은-폴리 메시에 부딪친다. 때때로 광선이 너무 멀리 가서 잘못된 기하학에 부딪쳐 출혈과 아티팩트를 생성합니다.

>[!NOTE]
>
> **해결 방법**
> 
> 이 문제를 방지하기 위해 몇 가지 해결 방법을 사용할 수 있습니다.
> 
> * [이름별 일치](../../features/matching-by-name/matching-by-name.md) 기능을 사용하여 메시를 격리합니다
> * 광선 거리를 제한하려면 [케이지](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)를 사용하십시오.
> * 일반적인 베이커 설정에서 기본 광선 거리를 더 낮은 값으로 변경합니다.
