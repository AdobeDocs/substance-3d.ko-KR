---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-substance-material-parameters.html"
breadcrumb-title: ''
description: Unreal Engine 5에서 런타임에 동적 재료 제어용 Blueprint 노드를 사용하여 Substance 재료 매개변수를 변경합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Substance material parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 청사진(UE5) Substance 재료 매개변수
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---


# 청사진(UE5): Substance 재질 매개변수

## float 매개 변수 변경:

[입력 부동 노드 설정](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/integrations/blueprint-node-reference-151584784.html)을 사용하여 float, color(float4) 및 부울 Substance 매개 변수를 변경합니다.

1. &quot;Substance 그래프 인스턴스&quot; 유형의 변수를 참조로 만듭니다.\
   \**이렇게 하려면 [내 청사진] 탭에 변수를 추가하고 이름을 지정하십시오. 드롭다운에서 Substance 그래프 인스턴스 > 개체 참조를 검색합니다. 변수를 그래프로 드래그하고 가져오기(변수 이름) 를 선택합니다. 세부 정보 탭의 기본값 섹션에서 Substance 그래프 인스턴스를 설정합니다.*
1. 입력 부동 노드 설정 을 만들고 대상을 Substance 그래프 인스턴스 변수로 설정합니다. 모든 결과를 보려면 검색 창의 [상황에 맞는] 상자를 선택 취소해야 할 수 있습니다.
1. 입력 부동 설정 노드에서 식별자를 변경할 Substance 매개 변수의 이름으로 설정합니다.\
   *\* Substance INST를 열고 매개 변수 이름 위에 마우스를 놓으면 식별자 이름을 찾을 수 있습니다. 식별자 이름이 도구 설명 팝업에 나타납니다.*
1. 입력 부동 노드에서 연결을 드래그하여 배열 노드 만들기 를 만듭니다. Make Array Node의 인덱스는 0입니다. 인덱스 0은 부동 소수점 값에 해당합니다.
1. 비동기 또는 동기화 렌더링 부동을 만들고 입력 설정 노드의 실행 줄을 렌더링 노드에 연결합니다. 렌더링할 인스턴스를 Substance 그래프 인스턴스 변수로 설정합니다.\
   *\* 비동기화는 비차단 상태이며 동기화는 차단 중입니다.*

![](../../../../../assets/steps.png){width="800px"}

## 부울 매개 변수

부울 매개 변수는 [입력 부울 설정]을 사용하여 변경됩니다.

![](../../../../../assets/setbool.png){width="800px"}

## 색상 매개 변수

색상 매개 변수는 입력 색상 설정 을 사용하여 변경됩니다.

![](../../../../../assets/setcolor.png){width="800px"}

## 정수 매개 변수 변경:

정수 매개 변수는 입력 설정 부동과 동일하게 작동합니다. 입력 정수 설정 노드를 사용합니다.

![](../../../../../assets/int.png)

## 식별자

substance INST에서 매개 변수에 대한 식별자를 찾을 수 있습니다. 마우스를 매개 변수 위로 이동하면 도구 설명에 식별자 이름이 표시됩니다. Substance Designer 출력 식별자 필드에 설정된 이름입니다.

![](../../../../../assets/screen-shot-2022-04-01-at-4-50-02-pm-copy.png)
