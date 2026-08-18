---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: 메쉬 색상 속성과 UV 매핑을 확인하여 메쉬 베이킹 오류의 색상 맵 문제를 해결합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메쉬에서 색상 맵으로 인해 베이킹 실패
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# 메쉬에서 색상 맵으로 인해 베이킹 실패

>[!WARNING]
>
> **문제**
> 
> 가능한 오류 메시지:
> 
> &#x200B;> > > 
> 
> [ Baking ] Baking 실패 (Mesh의 색상 맵)\
> 꼭지점 색상을 찾을 수 없음

>[!NOTE]
>
> **설명**
> 
> [메시에서 색상 맵](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)의 기본 설정은 메시 UV를 기반으로 높은 폴리 메시 꼭지점 색상을 텍스처로 굽는 것입니다. 그러나 고-폴리 메쉬(high-poly mesh)가 어떠한 꼭짓점 색상 정보도 가지고 있지 않은 경우가 종종 있다. 따라서 제빵사는 존재하지 않는 정보를 쓸 수 없다.

>[!NOTE]
>
> **해결 방법**
> 
> 이 오류 메시지를 방지하려면 다양한 해결 방법을 사용할 수 있습니다.
> 
> * 꼭지점 색상이 있는 높은 폴리 메시 사용
> * 다른 설정을 사용하여 메시 베이커의 색상 맵 설정
> * 필요하지 않은 경우 Mesh baker의 색상 맵을 사용하지 마십시오.
