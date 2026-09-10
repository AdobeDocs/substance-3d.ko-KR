---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/bent-normals-from-mesh.html"
breadcrumb-title: ''
description: 높은 폴리 메시에서 주변 조명의 평균 방향을 설명하는 표준 구부리기 텍스처를 계산합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Bent Normals from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시에서 표준 구부리기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 3%

---


# 메시에서 표준 구부리기

메시 베이커의 표준 구부리기는 주변 조명의 평균 방향을 설명하는 텍스처를 계산합니다. 이 베이커는 [메시 앰비언트 오클루전](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md) 베이커에서 파생되었습니다.

**사용 가능 대상:**

* Painter
* Designer
* 자동화 툴킷

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **보조 광선** | 폐색광선의 양. 값이 높으면 노이즈가 적게 발생하지만 계산에는 더 오래 걸립니다. |
| **최소 폐색기 거리** | 폐색 광선이 높은 폴리 기하학에 부딪힐 최소 거리**.** |
| **최대 폐색기 거리** | 폐색 광선이 높은 폴리 기하학에 닿을 최대 거리. |
| **테두리 상자 기준** | 활성화되면, 광선 거리 계산은 저-폴리 메시의 정규화된 공간(0 내지 1)에 기초한다. 비활성화된 경우 광선 거리 계산은 내보낼 때 낮은 폴리 메시에 지정된 단위(미터, 센티미터 등)를 기준으로 합니다. |
| **스프레드 각도** | 폐색 광선의 최대 확산 각도입니다. 기본값은 180입니다. |
| **배포** | 오클루전 광선 각 분포입니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>코사인</strong>(기본값)</li><li data-preserve-html="true"><strong>균일</strong></li></ul> |
| **뒷면 무시** | 활성화된 경우, 폐색 광선은 뒷면의 히트를 무시합니다(높은 폴리 표준이 광선이 발사되는 낮은 폴리와 반대 방향을 향하는 경우). 대부분의 경우 아티팩트를 방지하기 위해 이 설정을 활성화해야 합니다. |
| **자체 오클루전** | 폐색광선의 이름별 일치 베이커가 낮은 도형과 높은 도형을 일치시키는 방법을 나타냅니다. 수동으로 메쉬를 분리(분해)시킬 필요 없이 베이킹 프로세스를 필터링하는 데 사용할 수 있습니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>항상</strong>(기본값): 낮은 폴리 메시가 모든 높은 폴리 메시와 일치합니다.</li><li data-preserve-html="true"><strong>메시 이름별</strong>: 메시 이름을 기준으로 필터링하여 원하지 않는 형상과 일치하지 않도록 합니다.</li></ul>일치하는 도형에 대해 자세히 알아보려면 [이름별 일치](../../features/matching-by-name/matching-by-name.md)를 참조하세요. |
| **맵 유형** | 출력 텍스처 유형을 정의합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>월드 스페이스</strong></li><li data-preserve-html="true"><strong>탄젠트 공간</strong>(기본값)</li></ul> |
| **일반 방향** | **매트 유형**&#x200B;이(가) 접선 공간으로 설정된 경우 출력 텍스처의 일반 형식을 제어합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong> <strong> <br/></strong></li><li data-preserve-html="true"><strong>DirectX</strong>(기본값)<strong> <br/></strong></li></ul> |
