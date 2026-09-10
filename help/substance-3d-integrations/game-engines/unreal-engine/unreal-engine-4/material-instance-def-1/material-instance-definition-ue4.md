---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/material-instance-definition-ue4.html"
breadcrumb-title: ''
description: Unreal Engine 4에서 Substance 재질로 재질 인스턴스 정의를 생성하여 GPU 렌더링 성능을 최적화합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Material Instance Definition - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 재료 인스턴스 정의 - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---


# 재료 인스턴스 정의 - UE4

Substance과 함께 UE4 재질 인스턴스를 사용할 수 있습니다. 이렇게 하면 처리할 새 재질을 업로드하지 않아 GPU 렌더링 프로세스의 큰 단계가 절약됩니다. MID는 런타임이나 편집기에서 만들 수 있습니다. 버전 4.24.0.3을(를) 통해 재질 인스턴스화에 대한 완전한 지원을 추가했으며 Substance 엔진에서 지원하는 숫자 출력을 사용하는 새 재질 템플릿 워크플로를 도입했습니다. 재질 템플릿을 사용하면 UE4에서 Substance 재질 셰이더를 구성하는 방법을 정확하게 정의할 수 있습니다.

sbsar 파일을 가져올 때 사용할 템플릿을 선택할 수 있습니다.

![](../../../../assets/ue4-material-templates.png)

우리는 타일링, 텍스처 크기, 변위 및 방출 파라미터를 조정하기 위한 컨트롤이 내장된 변위, 굴절 및 세계 맞춤 재료 작업을 위한 템플릿을 함께 제공합니다. 재질 템플릿 시스템을 사용하여 사용자 정의 템플릿을 제공할 수도 있습니다.

![](../../../../assets/ue4-material-instance-params.png)

## 편집기에서 재질 인스턴스 만들기

1. Substance에서 만든 UE4 재질을 마우스 오른쪽 버튼으로 클릭하고 &#39;재질 인스턴스 만들기&#39;를 선택합니다. 이렇게 하면 UE4 인스턴스 재료가 만들어집니다.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/01-12?$png$&jpegSize=100&wid=592){width="560px"}
1. Substance 인스턴스 팩토리를 마우스 오른쪽 버튼으로 클릭하고 &quot;그래프 인스턴스 만들기&quot;를 선택합니다. 이렇게 하면 그래프의 인스턴스가 만들어지고 다른 UE4 재질이 만들어집니다. 새로 생성된 UE4 재질은 사용되지 않으므로 삭제합니다.

   ![](../../../../assets/02-10.png){width="300px"}
1. 1단계에서 만든 재질 인스턴스를 두 번 클릭하고 모든 맵의 텍스처 매개 변수를 활성화합니다.
1. 텍스처를 2단계에서 만든 새 INST 텍스처로 설정합니다. 이렇게 하면 인스턴스 그래프의 Substance 출력 맵을 사용하도록 재질 인스턴스가 설정됩니다.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/03-6?$png$&jpegSize=200&wid=1011){width="800px"}

이제 특정 Substance 텍스처 세트를 사용하는 UE4 재질 인스턴스가 있습니다. 이는 UE4 프로젝트에서 여러 물질을 사용하여 작업하는 보다 최적화된 방법입니다. 청사진을 사용하여 MID를 만드는 방법을 알아보려면 이 페이지를 확인하십시오. [청사진(UE4): 동적 재질 인스턴스](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
