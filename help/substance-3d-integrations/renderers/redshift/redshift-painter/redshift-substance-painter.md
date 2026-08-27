---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/renderers/redshift/redshift-substance-painter.html"
breadcrumb-title: ''
description: 출력 템플릿 및 적절한 질감 설정을 사용하여 Redshift 렌더러용 Substance Painter 텍스처를 내보냅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Redshift > Redshift - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Redshift - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---


# Redshift - Substance Painter

Substance Painter 2020.1(6.1.0)은 금속/거칠기(rsMaterial)에 대해 Redshift [출력 템플릿](https://docs.substance3d.com/display/SPDOC/Export)을 지원합니다. Redshift 템플릿을 사용하여 내보내면 Redshift 재질과 호환되는 텍스처를 만들 수 있습니다.

![](../../../assets/rs-export.png)

## Redshift 재질 설정

| Substance Painter 내보내기 | Redshift 재질 |
| --- | --- |
| 색상 | 확산/색상 |
| 거칠기 | 반사/거칠음 (BRDF = GCX) |
| 금속성 | 반사/금속성(프레넬 유형 = 금속성) |
| 표준 | 전체 / 범프 맵 / rsBumpMap (입력 맵 유형 = 접선 공간 표준 - Height 비율 = 1.0) |
| DisplaceHeightField | 변위 셰이더 / rsDisplacement TexMap (맵 인코딩 = Height 필드) |
| EmissionColor | 전체 / 배출 (배출 중량 = 1.0) |

>[!NOTE]
>
> 자료를 나타내는 지도는 정확하게 해석되어야 할 것이다. 자세한 내용은 [색상 관리](../../../renderers/color-management/color-management.md)페이지를 참조하세요.

## Maya / Redshift 예제

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maya-example?$pjpeg$&jpegSize=300&wid=1583){width="800px"}
