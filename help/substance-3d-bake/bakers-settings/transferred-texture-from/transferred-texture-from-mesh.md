---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/transferred-texture-from-mesh.html"
breadcrumb-title: ''
description: 일반 맵 변환 지원을 포함하여 UV를 기반으로 메시 간에 텍스처를 전송합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Transferred Texture from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시에서 전송된 텍스처
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 3%

---


# 메시에서 전송된 텍스처

메시 베이커에서 전송된 텍스처를 사용하면 각각의 UV를 기반으로 메시 하나에서 다른 메시로 텍스처를 변환할 수 있습니다. 이 제빵사는 또한 (특수 변환이 필요한) 전송 또는 표준 지도를 지원합니다. 작업하기 위해 두 망 모두 UV 정의가 필요합니다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **텍스처 파일** | 전송할 입력 텍스처 파일의 경로 |
| **UV 설정** | 메시 UV를 사용하여 높은 폴리 메시에서 텍스처를 읽고 낮은 폴리 메시 위에 투영합니다. |
| **필터링 모드** | 텍스처의 픽셀 보간을 수행하는 방법을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>가장 가까운</strong>: 보간이 없습니다. 지정된 위치에서 가장 가까운 픽셀을 사용하십시오. 정밀하지만 앨리어싱을 만들 수 있습니다.</li><li data-preserve-html="true"><strong>쌍선형</strong>(기본값): 지정된 위치에 가장 가까운 네 개의 픽셀을 사용합니다. 앨리어싱은 없지만 흐리게 표시될 수 있습니다.</li></ul> |
| **표준 맵** | 활성화된 경우 전송할 입력 텍스처가 표준 맵임을 제빵사에 나타냅니다. 이는 베이커가 텍스처에 특수 변환을 적용하여 대상 메쉬와 호환되도록 함을 나타냅니다. |
| **맵 유형** | 입력 텍스처의 표준 맵 유형을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>월드 스페이스</strong></li><li data-preserve-html="true"><strong>탄젠트 공간</strong>(기본값)</li></ul> |
| **일반 방향** | **맵 유형**&#x200B;이 **탄젠트 공간**(으)로 설정된 경우 입력 텍스처의 표준 형식을 정의합니다.가능한 값은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong>(기본값)</li></ul> |
