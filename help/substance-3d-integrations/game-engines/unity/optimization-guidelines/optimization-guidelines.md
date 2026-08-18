---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/optimization-guidelines.html"
breadcrumb-title: ''
description: 최적화 지침에 따라 Substance 재질 복잡성과 렌더링 성능의 균형을 맞출 수 있습니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Optimization Guidelines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 최적화 지침
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# 최적화 지침

Substance 재질이 복잡할수록 이를 렌더링하는 데 더 많은 처리 능력이 필요합니다. 따라서 Substance 재질은 **복잡성과 렌더링 속도 사이의 균형을 맞춰야 합니다**. 이는 게임과 같은 실시간 그래픽 응용 프로그램에 사용되는 경우 *특히*&#x200B;중요합니다.

사용자 정의 Substance 재질을 만들 때는 다음 최적화 지침을 반드시 확인하십시오.

[Substance Designer 최적화 지침](https://docs.substance3d.com/display/SDDOC/Performance+Optimization+Guidelines)

주의해야 할 주요 사항은 절대 해상도가 4K 이상인 노드입니다.

>[!WARNING]
>
> **해상도 및 부모와 관련된 해상도 설정에 주의하세요!**\
> 값이 높으면 성능에 심각한 영향을 주므로 해당 재질이 어떻게 사용될 것인지, 그리고 이와 관련된 데이터 크기를 줄일 수 있는지 여부를 고려하십시오.
>   
> Substance CPU 엔진은 4K에서 계산할 수 있지만 속도가 매우 느리고 통합이 중단되거나 충돌할 수 있습니다.

다음 예제에서는 [타일 Sampler](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/node-library/texture-generators/patterns/tile-sampler) 노드의 출력 크기를 [절대](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/output-size) 4096으로 설정합니다. 최종 2048년 출력 해상도에 대해 하향 스케일링되기 전에 다운스트림으로 여러 노드가 4K에서 계산되도록 합니다.

![](../../../assets/absolute.png){width="1000px"}
