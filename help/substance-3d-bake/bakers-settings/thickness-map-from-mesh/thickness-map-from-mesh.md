---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/thickness-map-from-mesh.html"
breadcrumb-title: ''
description: SSS 셰이더와 마스크에 사용하기 위해 메시 표면에서 안쪽으로 광선을 캐스팅하여 Thickness 맵을 생성합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Thickness Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시의 두께 맵
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 5%

---


# 메시의 두께 맵

메쉬의 Thickness 맵은 주변 오클루전 베이커와 매우 유사하지만 메쉬 표면에서 내부로 광선을 방출합니다. 이 텍스처는 SSS(Sub Surface Scattering) 셰이더에서 또는 마스킹 텍스처를 위해 사용될 수 있다.

텍스처 속성은 다음과 같이 정의됩니다.

* 검은색 값은 모델의 얇은 부분을 나타냅니다.
* 흰색 값은 모델의 굵은 부분을 나타냅니다.

**사용 가능 대상:**

* Substance Painter
* Substance Designer
* Substance 자동화 툴킷

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **보조 광선** | 오클루전 광선의 양입니다. 값이 높으면 노이즈가 적게 발생하지만 계산하는 데 시간이 더 오래 걸립니다. 기본값은 64입니다. |
| **최소 폐색기 거리** | 오클루전 광선이 높은 폴리 기하학에 도달하는 최소 거리입니다. 기본값은 0.00001입니다. |
| **최대 폐색기 거리** | 오클루전 광선이 높은 폴리 기하학에 도달하는 최대 거리입니다. 기본값은 0.1입니다. |
| **테두리 상자 기준** | 활성화된 경우 단위는 개체의 테두리 상자를 기준으로 합니다(테두리 상자의 대각선 길이 1.0). 비활성화된 경우 최소 및 최대 오클루더 거리에 사용되는 단위는 메쉬를 내보낼 때 정의된 단위입니다(미터, 센티미터 또는 내보낸 장면의 단위). |
| **스프레드 각도** | 폐색 광선의 최대 확산 각도입니다. 기본값은 180입니다. |
| **배포** | 오클루전 광선 각 분포입니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>코사인</strong>(기본값)</li><li data-preserve-html="true"><strong>균일</strong></li></ul> |
| **뒷면 무시** | 활성화된 경우, 오클루전 광선은 뒷면의 히트를 무시합니다(높은 폴리 표준이 광선이 주사되는 낮은 폴리와 반대 방향을 향하는 경우). 대부분의 경우 아티팩트를 방지하기 위해 이 설정을 활성화해야 합니다. |
| **자체 오클루전** | 오클루전 광선의 이름별 일치 베이커가 낮은 도형과 높은 도형을 일치시키는 방법을 나타냅니다. 수동으로 메쉬를 분리(분해)시킬 필요 없이 베이킹 프로세스를 필터링하는 데 사용할 수 있습니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>항상</strong>(기본값): 낮은 폴리 메시가 모든 높은 폴리 메시와 일치합니다.</li><li data-preserve-html="true"><strong>메시 이름별</strong>: 메시 이름을 기준으로 필터링하여 원하지 않는 형상과 일치하지 않도록 합니다.</li></ul>일치하는 도형에 대해 자세히 알아보려면 [이름별 일치](../../features/matching-by-name/matching-by-name.md)를 참조하세요. |
| **자동 정규화** | 출력 값을 0-1 범위에 맞게 조정할지 여부를 정의합니다. 가장 밝은 점은 순수한 흰색으로, 가장 어두운 점은 순수한 검은색으로 설정됩니다. |
