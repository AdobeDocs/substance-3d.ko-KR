---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/generated-textures-packing.html"
breadcrumb-title: ''
description: Substance이 Unity에서 텍스처를 생성하는 방법을 이해하고 최적의 셰이더 입력을 위해 텍스처 패킹을 구성합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Generated Textures (Packing)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 생성된 텍스처(패킹)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 6%

---


# 생성된 텍스처(패킹)

생성된 텍스처는 텍스처를 생성하기 위해 Substance 엔진에서 계산한 Substance의 출력을 표시합니다. 이러한 텍스처는 셰이더 입력으로 전달됩니다. 기본적으로 셰이더에 사용되는 기본 입력만 만들어집니다. &quot;모든 출력 생성&quot;이 활성화되어 있으면 모든 텍스처가 여기에 표시됩니다.

![](../../../assets/screen-shot-2022-03-29-at-1-24-16-pm-copy.png)

&quot;모든 출력 생성&quot;이 활성화된 경우

![](../../../assets/screen-shot-2022-03-29-at-1-29-35-pm-copy.png)

## 사용

1. 텍스처 아이콘을 선택하면 프로젝트 창에서 텍스처가 선택됩니다. 텍스처가 프로젝트 폴더에 생성되지 않으므로 런타임 재질에 대해서는 작동하지 않습니다.
1. sRGB 버튼은 [텍스처 가져오기 설정]의 sRGB(색상 텍스처) 옵션과 비슷하게 작동합니다. 이 옵션을 사용하면 텍스처를 감마 공간(sRGB)이나 선형 중 어떤 공간으로 해석할지 설정할 수 있습니다. Substance 플러그인은 이 해석을 자동으로 처리하지만 필요한 경우 재정의할 수 있습니다.

   | Substance 출력 | sRGB |
   | --- | --- |
   | 기본 색상 | 활성화됨 |
   | 확산 | 활성화됨 |
   | 반사 | 활성화됨 |
   | 표준 | 비활성화 |
   | 금속재질 | 비활성화 |
   | 거칠기 | 비활성화 |
   | 광택 | 비활성화 |
   | 높이 | 비활성화 |
   | 앰비언트 오클루전 | 비활성화 |

## 패킹 채널

드롭다운 메뉴를 사용하여 다른 텍스처의 알파 채널에 텍스처를 압축할 수 있습니다. 생성된 각 텍스처에는 Substance 재질에 의해 생성된 모든 텍스처 출력 목록이 포함된 드롭다운 메뉴가 있습니다. 목록에서 맵을 선택하여 텍스처의 알파 채널에 압축하면 됩니다. [소스] 옵션은 텍스처의 알파 채널입니다.

이 이미지에서 Height 맵을 선택했습니다.

![](../../../assets/screen-shot-2022-03-29-at-2-48-33-pm.png)

다음 이미지에서는 Height 출력이 기본 색상 맵의 알파 채널에 팩킹되고 있음을 확인할 수 있습니다.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-29-at-2-53-20-pm-copy?$png$&jpegSize=200&wid=1248)

## 출력 텍스처 매핑

또한 출력 텍스처 매핑 섹션을 통해 Unity 재질의 서피스 입력에 출력 텍스처를 개별적으로 할당할 수 있습니다. .sbsar로 생성된 출력 텍스처는 왼쪽 열에 표시되고 사용 가능한 [단위 표면 입력]은 오른쪽 열에 표시됩니다. 나중에 드롭다운을 통해 변경할 수 있습니다.

![](../../../assets/image2023-3-27-14-30-24.png)
