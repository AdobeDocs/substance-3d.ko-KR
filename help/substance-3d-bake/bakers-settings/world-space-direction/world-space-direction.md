---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/world-space-direction.html"
breadcrumb-title: ''
description: 월드 공간에서 벡터 방향을 계산하고 방향 효과 및 마스킹을 위해 텍스처로 저장합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > World Space Direction
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 월드 스페이스 방향
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 4%

---


# 월드 스페이스 방향

세계 우주 방향 제빵사는 세계 공간에서 벡터 방향을 텍스처로 계산할 수 있게 해준다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **입력 방향** | 방향이 계산되는 입력을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>텍스처에서</strong>: 벡터 방향은 입력 텍스처에 의해 정의됩니다.</li><li data-preserve-html="true"><strong>균일 벡터에서</strong>(기본값): 벡터 방향은 X, Y, Z 슬라이더로 정의됩니다.</li></ul> |
| **일반 방향** | 출력 텍스처의 표준 형식인지 여부를 정의합니다. 그러면 포맷에 따라 녹색 채널이 반전됩니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong>(기본값)</li></ul> |
| **X Y Z** | **입력 방향**&#x200B;이 **균일 벡터에서**(으)로 설정된 경우 방향 벡터의 세 가지 구성 요소를 정의하는 슬라이더입니다. |
| **방향 파일** | **입력 방향**&#x200B;이 **시작 텍스처**&#x200B;으로 설정된 경우 방향 벡터를 정의하기 위한 입력 텍스처 파일의 경로입니다. |
