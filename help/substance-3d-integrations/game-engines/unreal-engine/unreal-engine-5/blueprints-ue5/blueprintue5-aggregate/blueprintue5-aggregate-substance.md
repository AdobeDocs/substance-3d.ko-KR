---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-aggregate-substance.html"
breadcrumb-title: ''
description: 고급 워크플로우용 Blueprint Aggregate 노드를 사용하여 Unreal Engine 5에서 런타임에 여러 Substance 재료를 결합합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 청사진(UE5) 집계 Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# 청사진(UE5): 집계 Substance

1. &quot;합산 Substance 팩토리 생성&quot; 노드를 사용하고 출력 및 입력 팩토리를 설정합니다. 출력 팩터리에 입력 팩터리 매개 변수에서 입력 이미지로 사용할 텍스처 맵이 있어야 합니다.
1. 해당 값의 이름(출력 그래프의 출력 이름 및 입력 그래프의 입력 매개 변수 이름)으로 입력으로 사용되는 각 출력 텍스처의 SubstanceConnection 객체를 만듭니다
1. Create Graph Instance 노드를 추가하고 &quot;Create Aggregate Instance Factory&quot; Substance의 결과를 상위 자료와 함께 Factory 입력에 연결하여 템플릿 역할을 합니다(이 항목은 플러그인에 포함된 기본\_substance 재질 중 하나일 수 있음).
1. Substance 그래프 인스턴스 변수를 만들고 이전 노드의 결과를 저장합니다.
1. 선택 사항: 원하는 substance 매개변수를 설정합니다(이 예에서는 그래프 출력에 대한 새 해상도 설정).
1. 비동기 또는 동기화 렌더링 노드를 만들고 렌더링할 인스턴스를 Substance 그래프 인스턴스 변수에 연결합니다.
1. 그래프 인스턴스의 &quot;동적 재질 인스턴스 가져오기&quot; 기능을 사용하여 기존 재질 인스턴스를 만들거나 가져올 수 있습니다. 이름(Name) 및 모 재질에(In Parent Material)를 비워 두면 3단계에서 인스턴스를 생성할 때 사용된 매개변수가 사용됩니다.
1. Set Material Node를 추가하고 MID 변수의 값을 Material Input으로 설정합니다. 대상에 대해 재질을 적용할 개체로 설정합니다.
