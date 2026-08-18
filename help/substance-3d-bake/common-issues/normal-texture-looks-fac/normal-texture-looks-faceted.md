---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: 메쉬 표준을 매끄럽게 만들고 매끄러움 그룹 설정을 조정하여 표준 텍스처에서 면처리된 모양을 수정합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal texture looks faceted
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 표준 텍스처가 면처리된 것처럼 보임
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# 표준 텍스처가 면처리된 것처럼 보임

>[!WARNING]
>
> **문제**
> 
> [표준] 텍스처는 면이 보이거나 메시를 굽은 후 메시의 모든 면이 보입니다.
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **설명**
> 
> 노멀을 베이킹하면 이 결과가 나오는 주된 이유는 낮은 폴리 메쉬 노멀이 제대로 설정되지 않았기 때문이다. 각 면의 모든 가장자리는 하드 에지(hard edge)이며, 하이-폴리 메쉬(high-poly mesh)와 매칭하는 동안 광선 투영은 이웃 정보를 무시하고 이음새 또는 무의식 정보를 생성한다. 결과가 메시에서 괜찮아 보일 수 있지만, 나중에 음영 문제가 발생할 수 있으며 해결해야 합니다.

>[!NOTE]
>
> **해결 방법**
> 
> 주요 해결책은 정점 수직 또는 낮은 폴리 메쉬를 재작업하는 것이며, 프로세스의 정확한 이름은 3D 모델링 소프트웨어에 따라 다릅니다.
> 
> * Houdini의 Maya에서 **평균 표준**&#x200B;을 사용하세요.
> * 3DS 최대값에서 **하나의 매끄러움 그룹**&#x200B;을 사용하세요.
> * 믹서기에서 **부드러운 음영**&#x200B;을 사용하세요.
> * zBrush에서 내보낸 메시는 항상 단면화되어 다른 소프트웨어에서 정리되어야 합니다.
> 
> 이 작업으로는 충분하지 않을 수 있습니다. 메시를 내보낼 때는 설정에 따라 교점 표준 또는 음영 정보도 저장/생성해야 합니다.
