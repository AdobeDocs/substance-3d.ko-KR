---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-dynamic-material-instance-skip-to-end-of-metadata.html"
breadcrumb-title: ''
description: 실행 시 블루프린트를 사용하여 Unreal Engine 5의 Substance 자료에서 동적 재질 인스턴스를 만듭니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Dynamic Material Instance Skip to end of metadata
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 청사진(UE5) 동적 재질 인스턴스 메타데이터 끝으로 건너뛰기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# 청사진(UE5): 동적 재질 인스턴스 메타데이터 끝으로 건너뛰기

1. Instance Factory 유형의 변수를 만들고 기본값을 Imported Instance Factory로 설정합니다.
1. Create Graph Instance 노드를 추가하고 Substance 인스턴스 팩토리를 상위 자료와 함께 Factory 입력에 연결하여 템플릿 역할을 합니다(이 항목은 플러그인에 포함된 기본\_substance 자료 중 하나일 수 있음).
1. 이전 단계에서 만든 Substance 그래프 인스턴스 객체를 저장할 다른 변수를 만듭니다.
1. 그래프 인스턴스의 &quot;동적 재질 인스턴스 가져오기&quot; 기능을 사용하여 기존 재질 인스턴스를 만들거나 가져올 수 있습니다. 이름(Name)과 모 피쳐 재료(In Parent Material)를 비워 두면 2단계에서 인스턴스를 생성할 때 사용된 매개변수가 사용됩니다.
1. 재료(Material) 유형의 변수를 생성합니다. 자재 인스턴스 동적(MID)입니다. &quot;Get Dynamic Material Instance&quot;의 반환 값을 변수로 설정합니다.

   ![](../../../../../assets/dynamic-material-annotated-1.png)
1. Set Material Node를 추가하고 MID 변수의 값을 Material Input으로 설정합니다. 대상에 대해 재질을 적용할 개체로 설정합니다.
1. 선택 사항: 원하는 substance 매개변수를 설정합니다(이 예에서는 기존 substance graph 인스턴스를 사용하여 새 인스턴스에 값을 복사합니다).
1. 비동기 또는 동기화 렌더링 노드를 만들고 렌더링할 인스턴스를 Substance 그래프 인스턴스 변수에 연결합니다.
