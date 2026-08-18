---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity.html"
breadcrumb-title: ''
description: 기본 플러그인 지원 및 런타임 매개 변수 제어 기능이 있는 Unity 게임 엔진에서 Substance 재질을 가져오고 사용합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# 유니티

![](../../assets/unity.png)

>[!NOTE]
>
> **Unity 지원 버전**
> 
> Unity용 Adobe Substance 3D 플러그인 버전 3.0.0은 현재 Unity 2020.3.27x 이상을 지원합니다. [Unity Asset Store](https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208)에서 다운로드할 수 있습니다.

>[!WARNING]
>
> 플러그인을 업그레이드하거나 사용하기 전에 [프로젝트 페이지 업그레이드](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html)를 확인하세요.

>[!WARNING]
>
> 사용자 지정 Substance 자료를 작성하기 전에 [최적화 지침](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) 페이지를 확인하세요.

## 목차

* [Unity 릴리스 정보](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) - Unity 플러그인의 버전별 Substance의 새로운 기능
* [Unity에서 Substance 3D Adobe 다운로드](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) - Unity용 Substance 3D 플러그인은 Unity Asset Store https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555에서 사용할 수 있습니다.
* [Unity 플러그인 개요](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [통합 기본 설정](../../game-engines/unity/unity-preferences/unity-preferences.md) — Substance 기본 설정 창에서 플러그인에 대한 사용자 정의 옵션을 설정할 수 있습니다.
* [최적화 지침](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) - 사용자 지정 Substance 자료를 만들 때 다음 최적화 지침을 확인하세요.
* [프로젝트 업그레이드/알려진 문제](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) - Unity 플러그인의 Substance에 대해 알려진 문제
* [Substance 그래프 관리](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) - SGM(Substance 그래프 관리자)을 사용하여 Substance 자료를 기반으로 새 자료를 만들 수 있습니다
* [매개 변수 변경](../../game-engines/unity/changing-parameters/changing-parameters.md) - SGO(Substance 그래프 개체)에서 Substance 자료에 대한 매개 변수에 액세스할 수 있습니다.
* [생성된 텍스처(패킹)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) - 생성된 텍스처는 텍스처를 만들기 위해 Substance 엔진에서 계산한 Substance의 출력을 표시합니다
* [색상 공간 렌더링](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — 최상의 결과를 얻으려면 Unity Player 설정에서 색상 공간을 선형으로 설정해야 합니다.
* [이미지 입력 사용](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [모바일용 게시](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) - 모바일 플랫폼용 게시 지침
* [Unity 스크립팅용 Substance 3D](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) - Substance API를 사용하여 스크립트를 작성하고 런타임에 Substance 매개 변수를 업데이트하고 변경할 수 있습니다.
* [Unity에서 스크립팅(더 이상 사용되지 않음)](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) - Substance API를 사용하여 스크립트를 작성하고 런타임에 Substance 매개 변수를 업데이트하고 변경할 수 있습니다.
* [Substance 3D Assets 라이브러리 사용](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Substance 플러그인 제거](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D in Unity Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [유니티의 물리적 크기](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
* [프로젝트 간 sbsar 파일 공유](https://helpx.adobe.com/sharing-sbsar-files-between-projects.html) [&#128279;](../../game-engines/unity/sharing-sbsar-files-bet/sharing-sbsar-files-between-projects.md)

**[양식 찾음 - 필요한 규칙]**

>[!WARNING]
>
> 플러그인을 업그레이드하거나 사용하기 전에 [프로젝트 페이지 업그레이드](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html)를 확인하세요.

>[!WARNING]
>
> 사용자 지정 Substance 자료를 작성하기 전에 [최적화 지침](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) 페이지를 확인하세요.

### 목차

* [Unity 릴리스 정보](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) - Unity 플러그인의 버전별 Substance의 새로운 기능
* [Unity에서 Substance 3D Adobe 다운로드](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) - Unity용 Substance 3D 플러그인은 Unity Asset Store https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555에서 사용할 수 있습니다.
* [Unity 플러그인 개요](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [통합 기본 설정](../../game-engines/unity/unity-preferences/unity-preferences.md) — Substance 기본 설정 창에서 플러그인에 대한 사용자 정의 옵션을 설정할 수 있습니다.
* [최적화 지침](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) - 사용자 지정 Substance 자료를 만들 때 다음 최적화 지침을 확인하세요.
* [프로젝트 업그레이드/알려진 문제](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) - Unity 플러그인의 Substance에 대해 알려진 문제
* [Substance 그래프 관리](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) - SGM(Substance 그래프 관리자)을 사용하여 Substance 자료를 기반으로 새 자료를 만들 수 있습니다
* [매개 변수 변경](../../game-engines/unity/changing-parameters/changing-parameters.md) - SGO(Substance 그래프 개체)에서 Substance 자료에 대한 매개 변수에 액세스할 수 있습니다.
* [생성된 텍스처(패킹)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) - 생성된 텍스처는 텍스처를 만들기 위해 Substance 엔진에서 계산한 Substance의 출력을 표시합니다
* [색상 공간 렌더링](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — 최상의 결과를 얻으려면 Unity Player 설정에서 색상 공간을 선형으로 설정해야 합니다.
* [이미지 입력 사용](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [모바일용 게시](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) - 모바일 플랫폼용 게시 지침
* [Unity 스크립팅용 Substance 3D](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) - Substance API를 사용하여 스크립트를 작성하고 런타임에 Substance 매개 변수를 업데이트하고 변경할 수 있습니다.
* [Unity에서 스크립팅(더 이상 사용되지 않음)](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) - Substance API를 사용하여 스크립트를 작성하고 런타임에 Substance 매개 변수를 업데이트하고 변경할 수 있습니다.
* [Substance 3D Assets 라이브러리 사용](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Substance 플러그인 제거](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D in Unity Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [유니티의 물리적 크기](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
