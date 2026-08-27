---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/custom-materials.html"
breadcrumb-title: ''
description: 특수 워크플로우를 위한 Substance 플러그인으로 MODO에서 Unreal, Unity 및 glTF 사용자 정의 재질을 사용합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Custom Materials
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 맞춤형 재질
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 12%

---


# 맞춤형 재질

Substance 플러그인은 Unreal, Unity 및 glTF 사용자 정의 재질을 지원합니다. sbsar 파일을 로드하기 전에 사용할 음영 모드를 선택할 수 있습니다.

## 목차

## Unity Material

유니티 재질을 사용하면 재질 레이어 효과가 자동으로 설정됩니다. Substance 플러그인은 Unity 재질을 Substance 항목 재질 바로 위에 배치합니다.

| Substance 출력 | 색상 공간 | 재질 레이어 효과 |
| --- | --- | --- |
| 기본 색상 | sRGB | 유니티 알베도 |
| 광택 | 선형 | 유니티 Smoothness |
| 금속재질 | 선형 | 유니티 메탈릭 |
| 표준 | 선형 | 유니티 노멀 |
| 배출 | sRGB | Unity Emission **\*이미지에서 sRGB로 설정** |
| 높이 | 선형 | 유니티 범프 |
| 앰비언트 오클루전 | 선형 | 유니티 앰비언트 오클루전 |

![](../../../assets/unity-1.png){width="600px"}

## 언리얼 재질

[언리얼 재질]을 사용할 때는 [재질 레이어] 효과가 자동으로 설정됩니다. Substance 플러그인은 언리얼 재질을 Substance 항목 재질 바로 위에 배치합니다.

| Substance 출력 | 색상 공간 | 재질 레이어 효과 |
| --- | --- | --- |
| 기본 색상 | sRGB | 언리얼 기본 색상 |
| 거칠기 | 선형 | 언리얼 거칠음 |
| 금속재질 | 선형 | 언리얼 메탈릭 |
| 표준 | 선형 | 비현실 정상 |
| 높이 | 선형 | 언리얼 범프 |
| 배출 | sRGB | 스틸 이미지 **에서 sRGB로 설정된 비실제 방출**\ |
| 앰비언트 오클루전 | 선형 | 언리얼 앰비언트 오클루전 |
| 불투명도 | 선형 | 비실제 불투명도 **\*텍스처 레이어에서 반전된 선택을 해제해야 함** |

![](https://helpx-prod.scene7.com/is/image/HelpxProd/unreal?$png$&jpegSize=200&wid=1343){width="600px"}

[표준]을 반전해야 할 수도 있습니다. Substance에 일반 방향에 대한 컨트롤이 있는 경우 조정 메뉴에서 이 작업을 수행할 수 있습니다. 그렇지 않은 경우 텍스처 자체에서 이 작업을 수행할 수 있습니다. 자세한 내용은 &quot;**[표준 작업](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&quot; 페이지를 참조하세요.

## glTF 재질

glTF 재질을 사용하는 경우에는 [재질 레이어] 효과가 자동으로 설정됩니다. Substance 플러그인은 glTF 재질을 Substance 항목 재질 바로 위에 배치합니다.

| Substance 출력 | 색상 공간 | 재질 레이어 효과 |
| --- | --- | --- |
| 기본 색상 | sRGB | glTF 기본 색상 |
| 거칠기 | 선형 | glTF 거칠음 |
| 금속재질 | 선형 | glTF 금속 |
| 표준 | 선형 | glTF 표준 |
| 배출 | sRGB | glTF 방출 **\*이미지 스틸**&#x200B;에서 sRGB로 설정 |
| 앰비언트 오클루전 | 선형 | glTF 앰비언트 오클루전 |

![](../../../assets/gltf.png){width="600px"}

[표준]을 반전해야 할 수도 있습니다. Substance에 일반 방향에 대한 컨트롤이 있는 경우 조정 메뉴에서 이 작업을 수행할 수 있습니다. 그렇지 않은 경우 텍스처 자체에서 이 작업을 수행할 수 있습니다. 자세한 내용은 &quot;**[표준 작업](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&quot; 페이지를 참조하세요.
