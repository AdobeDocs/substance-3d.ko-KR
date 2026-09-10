---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: UV 풀기, 그룹 매끄럽게 하기 및 메시 토폴로지 문제를 확인하여 모든 면에 보이는 이음새를 수정합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 모든 면에 보이는 이음매
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# 모든 면에 보이는 이음매

>[!WARNING]
>
> **문제**
> 
> UV 솔기가 없더라도 형상의 일부 가장자리에 솔기가 표시됩니다.
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **설명**
> 
> [케이지](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)를 사용하지 않으면 베이킹 프로세스가 낮은 폴리 메쉬의 꼭지점 법선 방향으로 광선을 시작합니다. 각 꼭지점 법선이 분할되면(각 면이 인접 면과 동일한 꼭지점 법선을 공유하지 않는다는 의미) 광선이 가장자리에 있는 동일한 방향으로 전송되지 않습니다. 그러면 각 모서리 면의 정보가 다르기 때문에 분할됩니다.
> 
> 이 문제는 [이 페이지](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)에서 설명한 대로 앨리어싱으로 인해 악화됩니다.

>[!NOTE]
>
> **해결 방법**
> 
> 여기에서는 두 가지 해결책만 사용할 수 있습니다.
> 
> * 베이커에서 낮은 폴리 기하학에서 광선 방향을 계산하도록 하는 대신 [케이지](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)를 사용하여 광선 방향을 제어합니다.
> * 낮은 폴리 메쉬의 꼭지점 표준을 함께 병합합니다(부드럽게 하거나 공통 매끄러움 그룹 적용).
