---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/aliasing-on-uv-seams.html"
breadcrumb-title: ''
description: 앤티 앨리어싱 및 패딩 설정을 조정하여 베이킹 중에 UV 솔기에 나타나는 앨리어싱 아티팩트를 수정합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Aliasing on UV Seams
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV 솔기의 앨리어싱
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# UV 솔기의 앨리어싱

>[!WARNING]
>
> **문제**
> 
> 굽기 후 UV 솔기의 테두리에 어두운 점이나 점이 나타납니다.
> 
> ![](../../assets/edge-aliasing.png)

>[!NOTE]
>
> **설명**
> 
> 베이커는 텍스처에 정보를 기록할 때 기하학에서 픽셀로 변환해야 합니다. 이 정보를 처리하면 [앨리어싱](https://en.wikipedia.org/wiki/Aliasing)이 발생할 수 있습니다. 앨리어싱은 UV의 형상이 픽셀 격자와 정렬되지 않거나 UV가 충분한 해상도를 제공할 수 있을 만큼 충분한 픽셀을 덮지 않기 때문에 자주 발생합니다.
> 
> 다음 이미지에서 형상은 빨간색 오버레이입니다. 베이커는 표면의 절반 이상이 기하학으로 덮인 경우 픽셀을 가득 찬 것으로 표시합니다(흰색 사각형은 전체 픽셀이고 검은색 사각형은 빈 픽셀임). 오른쪽 이미지에서는 픽셀 격자가 해상도의 두 배이므로 형상을 보다 정확하게 표현할 수 있습니다.
> 
> ![](../../assets/aliasing-example-large.png)
> 
> ![](../../assets/aliasing-example-small.png)

>[!NOTE]
>
> **해결 방법**
> 
> * [베이커]의 출력 텍스처 해상도를 높입니다.
> * 앤티 앨리어싱 설정을 높입니다(참고 : 계산하는 데 시간이 더 걸릴 수 있음).
> * 3D 모델링 소프트웨어의 UV 편집기에서 UV를 픽셀 격자에 정렬합니다.
> * UV에 대한 텍셀 비율을 더 개선합니다.
