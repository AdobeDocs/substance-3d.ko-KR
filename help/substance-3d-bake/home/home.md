---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/home.html"
breadcrumb-title: ''
description: Substance Baker를 사용하여 메시 기반 정보를 텍스처 파일로 계산하고 텍스처링 워크플로우를 향상시키는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: bakers > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance Bakers
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 13%

---


# Substance Bakers

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

<b>Substance Bakers</b>는 메시 기반 정보를 텍스처 파일로 계산하는 고급 알고리즘의 도구 집합입니다. 이 예시는 3D 메시를 가진 모든 아티스트가 고급 텍스처링 방법을 활용하기 위해 사용할 수 있습니다. 베이킹은 <b> 강력한 도구</b> 및 <b>자동화된 텍스처링</b>을 제공하기 위한 Substance 소프트웨어 워크플로의 핵심입니다.

이 설명서에서는 <b>베이킹 기본</b> 및 이 프로세스를 처리할 때 발생할 수 있는 <b>일반적인 문제</b>에 대해 다룹니다.

</td>
<td width="58.30%" style="border: 0;" valign="top">

![](../assets/optim-baker-home.png){width="400px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## 시작하기

* [베이킹이란 무엇입니까?](../getting-started/what-is-baking/what-is-baking.md)
* 다음으로 굽기:
  * [Substance 3D Painter](../getting-started/software-interface/3d-painter/substance-3d-painter.md)
  * [Substance 3D Designer](../getting-started/software-interface/3d-designer/substance-3d-designer.md)
  * [Substance 3D 자동화 툴킷](../getting-started/software-interface/3d-automation-toolkit/substance-3d-automation-toolkit.md)
* [소프트웨어당 가용성](../getting-started/availability-per-software/availability-per-software.md)
* [호환되는 3D 소프트웨어](../getting-started/compatible-3d-software/compatible-3d-software.md)
* [튜토리얼](../getting-started/tutorials/tutorials.md)

</td>
<td style="border: 0;" valign="top">

### 베이커 설정

* [공통 매개 변수](../bakers-settings/common-parameters/common-parameters.md)
* [앰비언트 오클루전](../bakers-settings/ambient-occlusion/ambient-occlusion.md)
* [메시에서 주변 오클루전](../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)
* [메시에서 표준 구부리기](../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)
* [메시의 색상 맵](../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)
* [UV를 SVG로 전환](../bakers-settings/convert-uv-to-svg/convert-uv-to-svg.md)
* [곡선](../bakers-settings/curvature/curvature.md)
* [메쉬에서 곡률](../bakers-settings/curvature-from-mesh/curvature-from-mesh.md)
* [메쉬에서 곡률(사용되지 않음)](../bakers-settings/curvature-from-mesh-dep/curvature-from-mesh-deprecated.md)
* [메시의 높이 맵](../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)
* [메시의 표준 맵](../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)
* [메시의 불투명 마스크](../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)
* [위치](../bakers-settings/position/position.md)
* [메시의 위치 맵](../bakers-settings/position-map-from-mesh/position-map-from-mesh.md)
* [메시의 두께 맵](../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)
* [메시에서 전송된 텍스처](../bakers-settings/transferred-texture-from/transferred-texture-from-mesh.md)
* [월드 스페이스 방향](../bakers-settings/world-space-direction/world-space-direction.md)
* [실제 공간 표준](../bakers-settings/world-space-normals/world-space-normals.md)

</td>
<td style="border: 0;" valign="top">

### 안내선

* [오류 및 경고 메시지](../guides/error-and-warning-mes/error-and-warning-messages.md)
* [성능 및 최적화](../guides/performances-and-opt/performances-and-optimizations.md)
* [굽기 전 삼각 측량](../guides/triangulating-before-bak/triangulating-before-baking.md)

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### 기능

* [형상 캐시](../features/geometry-cache/geometry-cache.md)
* [GPU 광선 추적](../features/gpu-raytracing/gpu-raytracing.md)
* [이름별 일치](../features/matching-by-name/matching-by-name.md)
* [접선 공간](../features/tangent-space/tangent-space.md)

</td>
<td style="border: 0;" valign="top">

### 일반 질문

* [베이킹된 맵을 내보내는 방법](../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)
* [구운 텍스처에 디더링이 적용되나요?](../common-questions/dithering-applied-baked/is-dithering-applied-to-baked-textures.md)
* [&quot;조각당 탄젠트 공간 계산&quot;을 활성화해야 합니까?](../common-questions/should-enable-compute-tan/should-i-enable-compute-tangent-space-per-fragment.md)
* [Substance 소프트웨어의 외부에서 만들어진 텍스처가 올바르지 않음](../common-questions/texture-baked-outside-sof/texture-baked-outside-of-substance-software-looks-incorrect.md)
* [Assbin 파일이란 무엇입니까?](../common-questions/what-are-assbin-files/what-are-assbin-files.md)
* [구운 텍스처의 비트 심도는 무엇입니까?](../common-questions/what-the-bit-depth-baked/what-is-the-bit-depth-of-baked-textures.md)
* [OpenGL과 DirectX 표준 형식의 차이점은 무엇입니까?](../common-questions/what-the-difference-bet/what-is-the-difference-between-the-opengl-and-directx-normal-format.md)
* [굽거나 내보낸 후 내 텍스처에 이상한 스트레치가 생기는 이유는 무엇입니까?](../common-questions/why-are-there-strange-str/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.md)
* [앰비언트 오클루전/Thickness에서 이름별 매칭이 작동하지 않는 이유는 무엇입니까?](../common-questions/why-matching-name-not-wor/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.md)
* [굽고 나면 왜 내 메쉬가 완전히 검은색일까요?](../common-questions/why-mesh-fully-black-aft/why-is-my-mesh-fully-black-after-baking.md)

</td>
<td style="border: 0;" valign="top">

### 일반적인 문제

* [UV 솔기의 앨리어싱](../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)
* [베이커 출력이 완전히 검정색이거나 비어 있음](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/bake/baker-output-is-fully-black-159451835.html)
* [메시 기준 색상 맵 때문에 굽기 실패](../common-issues/baking-failed-with-color/baking-failed-with-color-map-from-mesh.md)
* [메시 표면에 검은색 음영 십자가 표시됨](../common-issues/black-shading-cross-are/black-shading-cross-are-visible-on-the-mesh-surface.md)
* [메시 부분이 서로 간에 재단 물림](../common-issues/mesh-parts-bleed-between/mesh-parts-bleed-between-each-other.md)
* [노멀 맵에 이상한 다채로운 그레이디언트가 있음](../common-issues/normal-map-has-strange/normal-map-has-strange-colorful-gradients.md)
* [표준 텍스처가 면처리된 것처럼 보임](../common-issues/normal-texture-looks-fac/normal-texture-looks-faceted.md)
* [일반 텍스처를 굽은 후 솔기가 보임](../common-issues/seams-are-visible-after/seams-are-visible-after-baking-a-normal-texture.md)
* [모든 면에 보이는 이음매](../common-issues/seam-visible-every-face/seam-visible-on-every-face.md)

</td>
</tr>
</table>
