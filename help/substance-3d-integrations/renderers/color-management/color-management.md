---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/color-management.html"
breadcrumb-title: ''
description: 다른 렌더러에서 Substance 재질을 사용할 때 색상 관리 및 감마 교정에 대해 이해합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 색상 관리
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 1%

---


# 색상 관리

우리는 선형 공간 렌더링이 조명 계산에 정확한 수학을 제공한다고 말하는 데 있어 단순한 접근법을 취할 것이다. 빛 상호 작용을 신뢰할 수 있는 실세계 방식으로 표현할 수 있는 환경을 조성한다. 선형 공간 렌더링에 대한 논의를 위해 감마 교정의 개념을 소개해야 한다. 표시 및 저장을 위해 이미지를 인코딩할 때 감마 교정은 대역폭과 비트 할당을 줄이는 최적화 프로세스입니다. 이 프로세스는 밝기에 대한 인간의 눈 인식을 활용하며, 이는 대략적으로 휘도의 세제곱근을 따른다.

>[!NOTE]
>
> 선형 공간 렌더링은 매우 복잡한 피사체입니다. 자세한 내용은 [Substance 아카데미](https://academy.substance3d.com/)의 무료 [PBR GUIDE VOLUME ONE](https://academy.substance3d.com/courses/the-pbr-guide-part-1)을 참조하세요.

## 색상 관리

이 문서의 목적은 [3D 소프트웨어](https://www.adobe.com/products/substance3d/3d-augmented-reality.html) 및 렌더러의 **Substance Painter** 및 **Substance Designer**&#x200B;에서 내보낸 텍스처로 작업하는 프로세스를 자세히 설명하는 것입니다.

재료 채널에 대한 입력으로 사용되는 이미지를 해석하는 올바른 방법은 이미지가 장면에서 사용되는 방식에 따라 다릅니다. 색상 공간, 인코딩 및 색상 값이 **장면 참조 광도** 또는 **표시 참조 광도**&#x200B;에 비례하는지 여부도 중요한 역할을 합니다.

* **비색상 데이터**&#x200B;를 나타내는 데 사용되는 이미지는 변환해서는 안 됩니다. 일반적으로 **보통**, **거칠기**, **금속**, **변위** 및 **주변** **오클루전** 지도입니다.
* 우리가 보는 색상을 나타내는 이미지에는 여러 시나리오가 있을 수 있습니다. 예를 들어 이미 **장면 선형**&#x200B;인 이미지는 일반적으로 **OpenEXR** 및 **HDR**&#x200B;과 같은 형식으로 저장된 **HDR** 이미지와 같이 변환할 필요가 없습니다.
* 디스플레이(**디스플레이 참조**)용으로 만든 이미지의 감마를 제거해야 합니다. 여기에는 **PNG**, **JPEG** 및 **BMP**&#x200B;와 같은 대부분의 형식이 포함됩니다. 해당 이미지는 **기본** **색상**, **확산**, **Specular** 및 **발광**&#x200B;입니다.

지나치게 단순화되었지만, 다음과 같은 과정을 생각해 보는 것이 도움이 될 수 있습니다.

* &quot;장면 참조(예: 선형)&quot; : 변환 적용 안 함
* &quot;표시 참조(예: sRGB)&quot; : 적절한 계산을 위해 이미지를 &quot;선형화&quot;하도록 역변환을 적용합니다

>[!NOTE]
>
> 감마 공간에서 선형 공간으로 변환하는 sRGB 디코딩 함수(EOTF)는 Substance Painter 및 Substance Designer에서 사용되며 IEC 61966-2-1:1999 표준에 의해 정의됩니다

색상 관리에 [OpenColorIO](https://opencolorio.org/)를 사용하도록 Substance Designer을 구성할 수 있습니다. 이를 통해 여러 응용 프로그램에서 *일관성 있는* 색상 변환과 이미지 표시를 할 수 있습니다. 이 모드에서는 Substance Designer이 내부적으로 **선형 RGB** 색상으로 작동합니다. 일반적으로 8비트 심도는 선형 색상을 나타내기에 충분하지 않으므로 [그래프](https://docs.substance3d.com/display/SDDOC/Graph+View)의 색상 텍스처에 *최소* **16비트** 깊이를 사용하는 것이 좋습니다.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sd-cm?$png$&jpegSize=200&wid=686)

[ACES](https://www.oscars.org/science-technology/sci-tech-projects/aces)을(를) 도입하면 이제 선형 sRGB(sRGB의 감마 버전 없음)와 CG 렌더링에 더 적합한 넓은 색상 영역(&quot;장면 참조&quot; 또는 선형) 색상 공간인 [ACEScg](https://acescolorspace.com/)이라는 두 개의 색상 공간이 생깁니다.

*색상 영역 플롯 그래픽 -<https://acescolorspace.com/>*

Substance Designer은 **Adobe Color Engine(ACE)**&#x200B;도 지원합니다. **ACE**&#x200B;을(를) 사용하면 **sRGB**, **선형 sRGB** 및 **ACEScg** 사이에서 작업 색상 공간을 선택할 수 있습니다. **sRGB**&#x200B;을(를) 사용하는 경우 **ACE**&#x200B;은(는) 레거시 모드와 거의 같습니다. 선형 색상 공간을 사용하는 경우 **ACE**&#x200B;은(는) [OpenColorIO](https://opencolorio.org/index.html)과(와) 비슷합니다.

## Substance 플러그인

Substance 통합 플러그인을 통해 Substance 재질을 사용할 때 출력은 통합 및 호스트 애플리케이션의 색상 관리를 통해 자동으로 선형/감마로 플래그가 지정됩니다. 그러나 프로세스를 이해하는 것이 중요합니다. Substance 맵을 Substance 재료가 아닌 내보낸 비트맵으로 사용할 때는 사용 중인 렌더러에 따라 텍스처를 **감마 인코딩** 또는 **raw**&#x200B;로 수동으로 플래그해야 할 수 있습니다. 일반적으로 8 또는 16비트 .png, .jpg, .tga 또는 .tif 파일은 감마 인코딩된 반면 **sRGB OETF** 및 .exr 파일은 선형입니다.

## 3D 응용 프로그램

### 텍스처를 사용한 작업

* [Maya의 텍스처 Substance](../../renderers/color-management/textures-in-maya/substance-textures-in-maya.md)
* [최대 3ds의 텍스처 Substance](../../renderers/color-management/textures-in-3ds-max/substance-textures-in-3ds-max.md)
