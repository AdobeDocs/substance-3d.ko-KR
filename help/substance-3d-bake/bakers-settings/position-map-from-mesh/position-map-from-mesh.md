---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/position-map-from-mesh.html"
breadcrumb-title: ''
description: 하이 폴리 메쉬에서 정확한 위치 맵을 계산하여 정확한 형상 위치 정보를 캡처합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시에서 위치 맵
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# 메시에서 위치 맵

메시 베이커의 위치 맵은 높은 폴리 메시 형상의 위치를 계산하고 텍스처에 저장합니다. 베이스 포지션 베이커와 비슷하지만 보다 정확한 결과를 낼 수 있다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **모드** | 위치 텍스처로 계산할 정보를 제어합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>모든 축:</strong> X, Y 및 Z축의 위치를 출력 텍스처의 RGB 채널에 고정합니다.</li><li data-preserve-html="true"><strong>한 축:</strong> 한 축을 회색 음영 이미지로 출력 텍스처에 연결합니다.</li></ul> |
| **축** | **Mode** 매개 변수가 **한 축**(으)로 설정된 경우 계산할 축을 정의합니다. |
| **정규화 형식** | 축당 위치 값의 비율을 조정하는 방법을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>상자:</strong> 메시 볼륨(테두리 상자 길이)에 따라 각 축을 표준화합니다.</li><li data-preserve-html="true"><strong>BSphere:</strong> 메시 볼륨 반경(경계 구)에 따라 모든 축을 표준화합니다.</li></ul> |
| **정규화 비율** | 메시를 기준으로 위치 값의 크기를 조절하는 방법을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>재질당</strong>: 각 재질에 대해 값이 0과 1 사이로 조정됩니다(텍스처 집합).</li><li data-preserve-html="true"><strong>전체 장면</strong>(기본값): 전체 메시를 고려하여 값이 조정됩니다. 이를 통해 오브젝트와 재질(텍스처 세트) 간에 연속적인 위치 값을 설정할 수 있습니다.</li></ul> |
