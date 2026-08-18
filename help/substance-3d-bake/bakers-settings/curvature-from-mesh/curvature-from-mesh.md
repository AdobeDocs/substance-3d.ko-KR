---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature-from-mesh.html"
breadcrumb-title: ''
description: 정밀한 가장자리 감지를 위해 광선 추적을 사용하여 높은 폴리 메쉬에서 정확한 곡률 텍스처를 생성합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메쉬에서 곡률
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# 메쉬에서 곡률

메쉬 베이커의 곡률(Curvature from mesh baker)은 높은 폴리 메쉬로부터 곡률 텍스처를 생성합니다. 베이커 [곡률](../../bakers-settings/curvature/curvature.md)보다 느리지만 더 정확한 결과를 생성합니다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷
* Substance Painter

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **보조 광선** | 주변 기하학을 읽기 위해 방출되는 광선의 양입니다. 값이 높으면 노이즈가 적게 발생하지만 계산하는 데 시간이 더 오래 걸립니다. 기본값은 32입니다. |
| **샘플링 반경** | 형상 서피스의 곡률을 계산하기 위해 인근 형상을 고려하는 정도입니다. 값이 높을수록 가장자리가 더 강해질 수 있으며 값이 낮을수록 가장자리가 더 가늘어지지만 정보가 누락될 수 있습니다. |
| **테두리 상자 기준** | 샘플링 반지름이 메쉬 크기에 상대적인지 또는 단위 기준 거리로 정의되었는지 정의합니다. |
| **자체 교차** | 곡률선의 이름으로 일치 베이커가 낮은 도형과 높은 도형을 일치시키는 방법을 나타냅니다. 수동으로 메쉬를 분리(분해)시킬 필요 없이 베이킹 프로세스를 필터링하는 데 사용할 수 있습니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>항상</strong>(기본값): 낮은 폴리 메시가 모든 높은 폴리 메시와 일치합니다.</li><li data-preserve-html="true"><strong>메시 이름별</strong>: 메시 이름을 기준으로 필터링하여 원하지 않는 형상과 일치하지 않도록 합니다.</li></ul>일치하는 도형에 대해 자세히 알아보려면 [이름별 일치](../../features/matching-by-name/matching-by-name.md)를 참조하세요. |
| **자동 톤 매핑 경계** | 곡률 값을 텍스처에 기록하는 방법을 제어합니다. 활성화하면, 값의 범위는 베이킹 공정 동안 발견된 최소값 및 최대값을 기준으로 0과 1 사이에서 정규화될 것이다. 비활성화하면 최소값과 최대값이 수동으로 정의됩니다.  **참고:** UDIM/UV 타일을 굽는 경우 이 매개 변수를 사용하지 않도록 설정하여 톤 매핑을 균일화하고 타일별로 지정하지 않아야 합니다. 그렇지 않으면 각 텍스처 간에 이음새가 생길 수 있습니다. 적합한 최소/최대 값을 수동으로 찾으려면 이 설정을 활성화하고 먼저 콘솔/로그를 확인하여 baker에서 출력한 값을 확인합니다. |
| **톤 매핑 최소** | **자동 톤 매핑 경계**&#x200B;가 사용되지 않도록 설정된 경우, 텍스처에 맞게 곡률 결과의 크기를 조절하는 최소값을 정의합니다. |
| **톤 매핑 최대** | **자동 톤 매핑 경계**&#x200B;가 비활성화되면 최대 값을 정의하여 곡률 결과를 텍스처에 맞게 조정합니다. |
| **표준 맵** | 일반 텍스처로의 선택적 경로입니다. 베이커의 내부 계산을 대신하는 데 사용할 수 있습니다. |
| **월드 스페이스** | 이 옵션을 활성화하면 표준 텍스처가 탄젠트 공간(Tangent Space) 대신 월드 공간 표준(World Space normal)으로 해석됩니다. |
| **일반 방향** | 탄젠트 공간(Tangent Space)에 있는 경우 수직 텍스처의 형식.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong>(기본값)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
