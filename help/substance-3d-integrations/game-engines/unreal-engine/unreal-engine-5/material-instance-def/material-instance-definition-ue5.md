---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-instance-definition-ue5.html"
breadcrumb-title: ''
description: Unreal Engine 5에서 Substance 재질을 사용하여 재질 인스턴스 정의를 만들어 GPU 렌더링 성능을 최적화합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Instance Definition - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 재료 인스턴스 정의 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---


# 재료 인스턴스 정의 - UE5

Substance에 UE5 재질 인스턴스를 사용할 수 있습니다. 이렇게 하면 새 재질을 프로세스에 업로드하지 않아 GPU 렌더링 프로세스의 큰 단계가 절약됩니다. MID는 런타임이나 편집기에서 만들 수 있습니다. 버전 5.0.0에서는 재질 인스턴스화에 대한 완전한 지원을 추가했습니다.

## 편집기에서 재질 인스턴스 만들기

1. Substance에서 만든 UE5 재질을 마우스 오른쪽 버튼으로 클릭하고 &quot;재질 인스턴스 만들기&quot;를 선택합니다. 그러면 UE5 인스턴스 재료가 생성됩니다.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-31-at-6-07-08-pm?$png$&jpegSize=300&wid=1472)
1. Substance 인스턴스 팩토리를 마우스 오른쪽 버튼으로 클릭하고 &quot;그래프 인스턴스 만들기&quot;를 선택합니다. 그러면 그래프의 인스턴스가 만들어지고 다른 UE5 재질이 만들어집니다. 새로 생성된 UE5 재질은 사용되지 않으므로 삭제합니다.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-10-38-pm.png)
1. 1단계에서 만든 재질 인스턴스를 두 번 클릭하고 모든 맵의 텍스처 매개 변수를 활성화합니다.
1. 텍스처를 2단계에서 만든 새 INST 텍스처로 설정합니다. 이렇게 하면 인스턴스 그래프의 Substance 출력 맵을 사용하도록 재질 인스턴스가 설정됩니다.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-13-18-pm.png)

이제 특정 Substance 텍스처 세트를 사용하는 UE5 재질 인스턴스가 있습니다. 이는 UE5 프로젝트에서 여러 물질을 사용하여 작업하는 보다 최적화된 방법입니다. 청사진을 사용하여 MID를 만드는 방법을 알아보려면 이 페이지를 확인하십시오. [청사진(UE5): 동적 재질 인스턴스](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
