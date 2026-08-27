---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ''
description: 사실감을 높이기 위해 광선 추적 기술을 사용하여 하이 폴리 메쉬에서 정확한 앰비언트 오클루전 텍스처를 굽습니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시에서 주변 오클루전
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%

---


# 메시에서 주변 오클루전

메쉬 베이커의 앰비언트 오클루전은 높은 폴리 메쉬로부터 앰비언트 오클루전 텍스처를 베이킹할 수 있습니다. 기본 [앰비언트 오클루전](../../bakers-settings/ambient-occlusion/ambient-occlusion.md) 제빵사보다 느리지만 더 정확한 결과를 생성합니다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷
* Substance Painter

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **보조 광선** | 폐색광선의 양. 값이 높으면 노이즈가 적게 발생하지만 계산하는 데 시간이 더 오래 걸립니다. 기본값은 64입니다. |
| **최소 폐색기 거리** | 폐색 광선이 높은 폴리 기하학에 닿을 최소 거리. 기본값은 0.00001입니다. |
| **최대 폐색기 거리** | 폐색 광선이 높은 폴리 기하학에 닿을 최대 거리. 기본값은 0.1입니다. |
| **테두리 상자 기준** | 활성화된 경우 단위는 개체의 테두리 상자를 기준으로 합니다(테두리 상자의 대각선 길이 1.0). 비활성화된 경우 최소 및 최대 오클루더 거리에 사용되는 단위는 메쉬를 내보낼 때 정의된 단위입니다(미터, 센티미터 또는 내보낸 장면의 단위). |
| **스프레드 각도** | 폐색 광선의 최대 확산 각도입니다. 기본값은 180입니다. |
| **배포** | 오클루전 광선 각 분포입니다. 광선이 퍼짐 각도 크기의 원뿔 내부에 분산되는 방식을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>코사인</strong>(기본값): 사실적이지만 매우 가늘게 가려진 영역에서 흰색 선으로 이어질 수 있습니다. 음영 및 조명에 더 적합합니다.</li><li data-preserve-html="true"><strong>균일</strong>: 선형 그레이디언트를 만드는 데 유용합니다. 레이어 마스크 및 기타 필터링에 더 적합합니다.</li></ul> |
| **뒷면 무시** | 이 매개 변수는 오클루전 광선이 뒷면의 히트를 무시하는지(높은 폴리 표준이 광선이 발사되는 낮은 폴리와 반대 방향을 향하는 경우)를 정의합니다. 대부분의 경우 아티팩트를 방지하기 위해 이 설정을 활성화해야 합니다. 가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nevers</strong>(기본값): 백페이스는 절대 무시되지 않습니다.</li><li data-preserve-html="true"><strong>항상</strong>: 뒷면은 항상 무시됩니다.</li><li data-preserve-html="true"><strong>메시 이름별</strong>: 접미어 키워드와 일치하는 메시에 대해서만 뒷면이 무시됩니다. [공통 매개 변수](../../bakers-settings/common-parameters/common-parameters.md)를 참조하십시오.</li></ul> |
| **자체 오클루전** | 오클루전 광선의 이름별 일치 베이커가 낮은 도형과 높은 도형을 일치시키는 방법을 나타냅니다. 수동으로 메쉬를 분리(분해)시킬 필요 없이 베이킹 프로세스를 필터링하는 데 사용할 수 있습니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>항상</strong>(기본값): 낮은 폴리 메시가 모든 높은 폴리 메시와 일치합니다.</li><li data-preserve-html="true"><strong>메시 이름별</strong>: 메시 이름을 기준으로 필터링하여 원하지 않는 형상과 일치하지 않도록 합니다.</li></ul>일치하는 도형에 대해 자세히 알아보려면 [이름별 일치](../../features/matching-by-name/matching-by-name.md)를 참조하세요. |
| **표준 맵** | 일반 텍스처로의 선택적 경로입니다. 베이커의 내부 계산을 대신하는 데 사용할 수 있습니다. |
| **월드 스페이스** | 이 옵션을 활성화하면 표준 텍스처가 탄젠트 공간(Tangent Space) 대신 월드 공간 표준(World Space normal)으로 해석됩니다. |
| **일반 방향** | 탄젠트 공간(Tangent Space)에 있는 경우 수직 텍스처의 형식.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong>(기본값)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **감쇠** | 폐색기 거리에 의해 오클루전이 감쇄되는 방법을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>없음</strong>: 감쇠가 없습니다.</li><li data-preserve-html="true"><strong>선형</strong>(기본값) : 점진적 감쇠.</li><li data-preserve-html="true"><strong>매끄럽게</strong>: 부드러운 감쇠입니다.</li></ul> |
| **지표 평면** | 활성화된 경우 XZ 축의 메시 경계 상자 아래에서 보조 광선과 충돌하는 평면을 시뮬레이션합니다. 보이지 않는 평면도에서 그림자가 오는 것처럼 보이게 합니다. |
| **지표 평면 오프셋** | 메쉬에서 멀리 계획을 이동하여 효과의 강도를 줄일 수 있습니다. 값은 절대값이며 메쉬 크기에 상대적인 값이 아닙니다. |
