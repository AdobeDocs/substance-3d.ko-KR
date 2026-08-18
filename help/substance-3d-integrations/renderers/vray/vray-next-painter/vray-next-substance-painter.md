---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/renderers/vray/vray-next-substance-painter.html"
breadcrumb-title: ''
description: 출력 템플릿 및 적절한 워크플로우 설정을 사용하여 V-Ray 다음 렌더러용 Substance Painter 텍스처를 내보냅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Vray > Vray Next - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Vray Next - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---


# Vray Next - Substance Painter

Substance Painter 2020.1(6.1.0)은 금속 및 Specular 워크플로우 모두에 대해 [VrayMtl](https://docs.chaosgroup.com/display/VRAY4MAYA/VRayMtl) 셰이더와 함께 제공됩니다. 뷰포트 셰이더를 구성하는 **VrayMtl 템플릿**&#x200B;을 사용하여 [Substance Painter 프로젝트를 설정](https://docs.substance3d.com/display/SPDOC/Project+Creation)할 수 있습니다.

![](../../../assets/template-16.jpg)

셰이더 설정(Shader Settings)에서 VrayMtl을 사용하여 작업하도록 Vray 셰이더를 구성할 수 있습니다.

>[!NOTE]
>
> 프로젝트가 [UV 타일 UDIM 레거시](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html)를 사용하도록 설정된 경우. [다음 UDIM 출력 템플릿 표시]를 사용합니다.

![](../../../assets/vray-mtl-shader.png){width="800px"}

[Vray Next]에서 렌더링하기 위한 텍스처를 내보내려면 [Vray Mtl] 출력 템플릿을 선택합니다.

![](../../../assets/template-project.jpg){width="800px"}

## Vray 재질 (Vray Next - 금속/거칠음)

| Substance Painter 내보내기 | VRayMtl |
| --- | --- |
| 기본 색상 | (**마야**) 확산 색상(양 = 1.0) (**3ds 최대**) 확산 |
| 거칠기 | (**마야**) 반사/거칠기 (BRDF = GGX) + (거칠기 사용 가능)(**3ds 최대**) 거칠기 → BRDF/ GGX 사용 및 거칠기 사용 가능 |
| 금속재질 | (**Maya**) 반사/금속도 (**3ds 최대**) 금속도 |
| 표준 | (**Maya**) 범프 및 표준 매핑/맵 (맵 유형 = 접선 공간에서 표준)(**3ds** **최대**) 비트맵 → 표준 |
| 높이 | (**Maya**) 변위 셰이더/변위 (**3ds** **Max**) 개체 수정자 → VrayDisplacementMod → Tex 맵 |
| 배출 | 자체 조명 |
| 투과형 | (**Maya**) 서브서피스 분산/반투명 색상(**3ds 최대**) 반투명 → 뒷면 색상 |
| 이방성 각도 | (**Maya**) 비등방성/비등방성 회전(**3ds** **최대**) BRDF/회전 |
| 이방성 레벨 | (**마야**) 비등방성/비등방성(**3ds 최대**) BRDF/각도 |

## Vray 재질 (Vray Next - Specular/광택

| Substance Painter 내보내기 | VRayMtl |
| --- | --- |
| 확산 | (**마야**) 확산 색상(양 = 1.0) (**3ds 최대**) 확산 |
| 반사 | (**마야**) 반사/반사 색상(양 = 1.0) (**3ds 최대**) 반사 |
| 광택 | (**마야**) 반사/거칠기 (BRDF = GGX) + (거칠기 사용 가능)(**3ds 최대**) BRDF→ 광택 / GGX 사용 및 광택 사용 가능 |
| 표준 | (**Maya**) 범프 및 표준 매핑/맵 (맵 유형 = 접선 공간에서 표준)(**3ds** **최대**) 비트맵 → 표준 |
| 높이 | (**Maya**) 변위 셰이더/변위 (**3ds** **Max**) 개체 수정자 → VrayDisplacementMod → Tex 맵 |
| 배출 | 자체 조명 |
| 투과형 | (**Maya**) 서브서피스 분산/반투명 색상(**3ds 최대**) 반투명 → 뒷면 색상 |
| 이방성 각도 | (**Maya**) 비등방성/비등방성 회전(**3ds** **최대**) BRDF/회전 |
| 이방성 레벨 | (**마야**) 비등방성/비등방성(**3ds 최대**) BRDF/각도 |

>[!NOTE]
>
> 자료를 나타내는 지도는 정확하게 해석되어야 할 것이다. 자세한 내용은 [색상 관리](../../../renderers/color-management/color-management.md)페이지를 참조하세요.

이 예에서는 Vray Metallic/Roughness 셰이더를 사용하는 Substance Painter 뷰포트 및 Maya를 사용하는 Vray 렌더링을 보여 줍니다.

![](../../../assets/vray-maya.jpg){width="800px"}
