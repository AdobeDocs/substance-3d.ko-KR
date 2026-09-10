---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/position.html"
breadcrumb-title: ''
description: 메시 지오메트리 위치를 계산하고 텍스처에 저장하여 볼륨 기반 효과와 그레이디언트 마스크를 생성합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 위치
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

---


# 위치

위치 베이커(Position baker)는 메쉬 형상의 위치를 계산하고 텍스처에 저장합니다. 이 위치는 개체의 볼륨에서 정보를 계산하거나 그래디언트 마스크를 만드는 데 유용합니다.

**사용 가능 대상:**

* Substance Painter
* Substance Designer
* Substance 자동화 툴킷

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **모드** | 위치 텍스처로 계산할 정보를 제어합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>모든 축:</strong> X, Y 및 Z축의 위치를 출력 텍스처의 RGB 채널에 고정합니다.</li><li data-preserve-html="true"><strong>한 축:</strong> 한 축을 회색 음영 이미지로 출력 텍스처에 연결합니다.</li></ul> |
| **축** | **Mode** 매개 변수가 **한 축**(으)로 설정된 경우 계산할 축을 정의합니다. |
| **정규화 형식** | 축당 위치 값의 비율을 조정하는 방법을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>상자:</strong> 메시 볼륨(테두리 상자 길이)에 따라 각 축을 표준화합니다.</li><li data-preserve-html="true"><strong>BSphere:</strong> 메시 볼륨 반경(경계 구)에 따라 모든 축을 표준화합니다.</li></ul> |
| **정규화 비율** | 메시를 기준으로 위치 값의 크기를 조절하는 방법을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>재질당</strong>: 각 재질에 대해 값이 0과 1 사이로 조정됩니다(텍스처 집합).</li><li data-preserve-html="true"><strong>전체 장면</strong>(기본값): 전체 메시를 고려하여 값이 조정됩니다. 이를 통해 오브젝트와 재질(텍스처 세트) 간에 연속적인 위치 값을 설정할 수 있습니다.</li></ul> |
