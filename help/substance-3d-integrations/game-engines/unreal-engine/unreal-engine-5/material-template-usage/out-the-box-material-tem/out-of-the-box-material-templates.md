---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5/out-of-the-box-material-templates.html"
breadcrumb-title: ''
description: SBSAR 재질을 Unreal 엔진 5로 가져올 때 사전 설치된 재질 템플릿을 사용하면 빠른 설정 및 워크플로를 수행할 수 있습니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5 > Out-of-the-Box Material Templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 기본 재질 템플릿
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# 기본 재질 템플릿

SBSAR 재질을 콘텐츠 브라우저로 가져올 때 드롭다운에서 즉시 사용할 수 있는 다른 재질 템플릿을 선택할 수 있습니다.

![](../../../../../assets/screen-shot-2022-05-10-at-8-58-45-pm-copy.png)

## Substance 표준 템플릿

일반 UV 경험을 위한 기본 재질 템플릿입니다. UV 양에 대한 몇 가지 기본 컨트롤을 제공하므로 UV를 조정하여 텍스처를 늘릴 수 있습니다. [UV 분할] 옵션을 활성화하여 UV 비율을 분할할 수 있으며, U 양, V 양, UV 오프셋 및 UV 회전 각도도 있습니다. 이렇게 하면 UV 회전뿐만 아니라 일부 UV 타일링을 수행할 수 있습니다.

![](../../../../../assets/screen-shot-2022-05-10-at-9-06-40-pm-copy.png)

## Substance 삼평면 템플릿

삼각형 템플릿은 메쉬의 X, Y 및 Z 각도나 면을 삼각형으로 매핑하여 텍스처의 세 가지 투영을 함께 혼합하여 각도를 매끄럽게 혼합합니다. 삼평면 템플릿을 사용하면 개체가 구부러질 때 여러 면에서 재질이 함께 혼합될 수 있습니다

Substance 삼각 재질의 ![세부 메뉴](../../../../../assets/triplanar-template.png)

트리평면 템플릿은 물리적 크기를 지원하므로 물리적 크기를 활성화하면 트리평면 템플릿이 재질의 물리적 크기에 따라 이미지의 크기를 조절하므로 개체의 크기를 얼마나 조절하든 해당 텍스처는 항상 동일하게 유지되고 균일한 모양을 갖습니다. 여기에서 물리적 크기 자세히 알아보기: [물리적 크기 - UE5](../../../../../game-engines/unreal-engine/unreal-engine-5/physical-size-ue5/physical-size-ue5.md)

## Substance 굴절 템플릿

굴절 템플릿은 주로 투명 개체, 예를 들어 안경에 사용됩니다. 이를 통해 유리 재질 또는 투명 재질에 대해 가질 수 있는 IOR 값이나 표준 텍스처를 수정할 수 있습니다.

![](../../../../../assets/screen-shot-2022-05-10-at-9-07-38-pm.png)

## Substance 자동차 페인트 템플릿

자동차 페인트 템플릿에는 투명 코트 지지체가 추가되어 있으며 조정 가능한 UV 타일링 및 값, 투명 코트 거칠기 값 및 프레넬 전원 값을 지원합니다.

![Substance 자동차 페인트 재질의 세부 정보 메뉴](../../../../../assets/car-paint-template.png)

## 변위 템플릿 설정

>[!IMPORTANT]
>
> 시험적 템플릿
> 
> 경고: 다음 템플릿은 실험적이며 버전 간 주요 변경 사항이 적용됩니다. 이 템플릿들은 이 글쓰기의 당시에 그 자체로 실험적인 에픽의 나나이트 기능을 활용한다. 100% 안정적이지 않을 수 있으며 프로젝트에서 사용할 때는 주의해야 합니다.

다음 단계에 따라 프로젝트에서 Nanite 변위 지원을 완전히 활성화하고 메쉬와 함께 변위 재질을 사용합니다.

1. 프로젝트 폴더 > 구성 > DefaultEngine.ini 로 이동하여 엽니다
1. [/Script/Engine.RendererSettings] 섹션에 다음을 추가합니다.
   * r.Nanite.AllowTessellation=1
   * r.Nanite.Tessellation=1
1. 변위 템플릿을 적용할 정적 메쉬를 선택하고 설정을 엽니다.
1. Nanite 지원 활성화 옵션을 켭니다.
1. 원하는 .sbsar를 컨텐트 브라우저로 가져오고 Substance\_변위\_템플릿 또는 Susbtance\_Triplanar\_Displacement\_Template을 선택합니다.
1. 변위 양을 변경하려면 재료 템플릿으로 이동하여 출력 노드를 선택합니다. 그런 다음 변위 섹션에서 강도 를 조정합니다.

## Substance 변위 템플릿

Substance 표준 템플릿과 마찬가지로 이 템플릿에서는 Nanite 변위 지원을 추가하면서 U 및 V 값을 조정할 수 있습니다.

![Substance 변위 자료에 대한 세부 정보 메뉴](../../../../../assets/displacement-template.png)

## Substance 삼평면 변위 템플릿

Substance 변위 템플릿과 마찬가지로 이 템플릿은 물리적 크기 지원 옵션과 함께 3면 투영을 적용하며 Nanite 변위 지원을 추가합니다.

Substance 삼각 변위 자료의 ![세부 정보 메뉴](../../../../../assets/triplanar-displacement-template.png)
