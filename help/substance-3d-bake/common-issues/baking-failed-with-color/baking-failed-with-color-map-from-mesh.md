---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: 메시 색상 속성과 UV 매핑을 확인하여 메시 기준 색상 맵 굽기 오류를 해결합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시 기준 색상 맵 때문에 굽기 실패
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# 메시 기준 색상 맵 때문에 굽기 실패

>[!WARNING]
>
> **문제**
> 
> 가능한 오류 메시지:
> 
> > > > 
> 
> [ 베이킹 ] 베이킹 실패(메시 기준 색상 맵)\
> 꼭지점 색상을 찾을 수 없음

>[!NOTE]
>
> **설명**
> 
> [메시 기준 색상 맵](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)의 기본 설정은 메시 UV를 기반으로 높은 폴리 메시 꼭지점 색상을 텍스처로 굽는 것입니다. 그러나 고-폴리 메쉬(high-poly mesh)가 어떠한 꼭짓점 색상 정보도 가지고 있지 않은 경우가 종종 있다. 따라서 제빵사는 존재하지 않는 정보를 쓸 수 없다.

>[!NOTE]
>
> **해결 방법**
> 
> 이 오류 메시지를 방지하려면 다양한 해결 방법을 사용할 수 있습니다.
> 
> * 꼭지점 색상이 있는 높은 폴리 메시 사용
> * 다른 설정으로 메시 기준 색상 맵 베이커 설정
> * 필요없는 경우에는 메시 기준 색상 맵 제빵기를 사용하지 마세요
