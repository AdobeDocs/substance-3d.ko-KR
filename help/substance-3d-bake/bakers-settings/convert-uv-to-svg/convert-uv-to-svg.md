---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/convert-uv-to-svg.html"
breadcrumb-title: ''
description: 메쉬 UV를 벡터 그래픽 파일로 변환하여 정밀한 마스크와 오버레이를 만들 수 있습니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Convert UV to SVG
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV를 SVG로 전환
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 6%

---


# UV를 SVG로 전환

[UV를 SVG으로 변환] 베이커는 낮은 폴리 메쉬 UV를 벡터 그래픽 파일로 변환합니다. 이 벡터 그래픽 파일을 사용하여 마스크를 만들 수 있습니다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **패딩** | SVG 모양에 기하학적 패딩을 추가할 정도를 제어합니다. |
| **색상 모드** | SVG 모양에 색상을 지정하는 방법을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>무작위:</strong> 각 UV 셸은 무작위 색상으로 칠해집니다.</li><li data-preserve-html="true"><strong>색조 이동:</strong> 각 UV 셸은 고유한 색조 값으로 채색됩니다.</li><li data-preserve-html="true"><strong>회색 음영:</strong> 각 UV 셸에 고유한 회색 음영 값이 적용됩니다.</li><li data-preserve-html="true"><strong>균일한 색상:</strong> 모든 UV 쉘의 색상은 50% 회색 값으로 지정됩니다.</li><li data-preserve-html="true"><strong>재질 ID 색상</strong>: UV 쉘은 장면 보기에서 정의된 재질 색상으로 표시됩니다.</li></ul> |
