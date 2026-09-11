---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/color-map-from-mesh.html"
breadcrumb-title: ''
description: 하이 폴리 메시에서 색상 속성을 텍스처로 투영하여 선택 마스크에 사용할 폴리 페인트 또는 재질 ID를 굽습니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시의 색상 맵
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 4%

---


# 메시의 색상 맵

Mesh Baker의 [색상 맵]은 고해상도 메쉬에서 텍스처로 색상 속성을 투영합니다. 폴리 페인트 또는 재질 ID를 베이킹하여 선택 마스크를 만드는 데 사용할 수 있습니다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷
* Substance Painter

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **색상 소스** | 색상 생성이 기반해야 하는 하이 폴리 메시 속성의 기준이 됩니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>정점 색상</strong>: 정점 색상을 읽고 텍스처에 저장합니다. 정점에서 정점으로 색상 보간</li><li data-preserve-html="true"><strong>재질 색상</strong>: 다각형 면에 할당된 재질 색상을 읽습니다.</li><li data-preserve-html="true"><strong>메시 ID</strong>: 찾은 개체별로 색상을 할당합니다.</li><li data-preserve-html="true"><strong>Polygroup/Submesh ID</strong>: 하위 개체(요소라고도 함)별로 색상을 할당합니다.</li></ul> |
| **색상 생성기** | **색상 소스**&#x200B;가 **메쉬 ID** 또는 **폴리그룹/서브메쉬 ID**(으)로 설정될 때 색상이 생성되는 방식을 정의합니다.가능한 값은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>무작위</strong>: 각 개체 또는 하위 개체의 색이 임의로 생성된 색상으로 지정됩니다.</li><li data-preserve-html="true"><strong>색조 이동</strong>: 각 개체 또는 하위 개체는 색조를 기반으로 고유한 색상으로 칠해집니다.</li><li data-preserve-html="true"><strong>회색 음영</strong>: 각 개체 또는 하위 개체의 색이 고유한 회색 음영 값으로 지정됩니다.</li></ul> |
