---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/renderman/renderman-substance-painter.html"
breadcrumb-title: ''
description: pxrSurface 재질 및 적절한 출력 변환을 사용하여 Renderman에 대한 Substance Painter 텍스처를 내보냅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Renderman > Renderman - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderman - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 1%

---


# Renderman - Substance Painter

Substance Painter 2020.1(6.1.0)은 [**pxrSurface**](https://rmanwiki.pixar.com/display/REN/PxrSurface) 및 pxrDisney [출력 템플릿](https://docs.substance3d.com/display/SPDOC/Export)를 지원합니다.

![](../../../assets/renderman.png)

출력에 **pxrSurface**&#x200B;을(를) 사용하는 것이 좋습니다.

![](../../../assets/pxrsurface.png)

## Renderman 셰이더(Maya - RM 23.1)

| Substance Painter 내보내기 | PxrSurface |
| --- | --- |
| DiffuseColor | 확산 / 색상 |
| 반사 거칠음 | 기본 Specular/거칠음 |
| SpecularFaceColor | 기본 Specular/얼굴 색상 |
| 표준 | Globals / Bump / PxrNormalMap → Orientation (Open GL) |
| 변위 | (빨강 채널 ) PxrDispTransform (결과 F) → (disp 스칼라) PxrDisspace (Out 색상) → (변위 셰이더) PxrSurfaceSG |
| GlowColor | 광선/색상 (게인 = 1.0) |
| 현재 상태 | 글로벌/현재 상태 |

>[!NOTE]
>
> 자료를 나타내는 지도는 정확하게 해석되어야 할 것이다. 자세한 내용은 [색상 관리](../../../renderers/color-management/color-management.md)페이지를 참조하세요.
