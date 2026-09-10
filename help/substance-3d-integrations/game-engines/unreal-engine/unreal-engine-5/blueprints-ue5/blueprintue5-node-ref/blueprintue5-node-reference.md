---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-node-reference.html"
breadcrumb-title: ''
description: Unreal Engine 5에서 재료 작업용으로 사용할 수 있는 모든 Substance 청사진 노드에 대한 참조 안내서입니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Node Reference
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 청사진(UE5) 노드 참조
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---


# 청사진(UE5): 노드 참조

## 일반 Substance 노드:

| 이름 | 입력 | 설명 |
| --- | --- | --- |
| **GetSubstance** | 입력: **재질** | 재질에 사용된 Substance 그래프 인스턴스의 배열을 반환합니다. 서로 다른 두 그래프 인스턴스의 텍스처 출력을 사용하는 재질을 만드는 경우 이 함수는 해당 두 그래프 인스턴스를 반환합니다. |
| **GetSubstanceTexture** | 입력: **SubstanceGraphInstance** | Substance 그래프 텍스처 입력 매개 변수에서 활성화된 모든 인스턴스와 현재 계산된 인스턴스의 배열을 반환합니다. |
| **GetGraphName** | 입력: **SubstanceGraphInstance** | Designer에 설정된 그래프 이름을 반환합니다. |
| **GetFactoryName** | 입력: **SubstanceGraphInstance** | 이 노드에 전달된 **SubstanceGraphInstance**&#x200B;을(를) 만드는 데 사용된 **GraphInstanceFactory**&#x200B;의 이름을 반환합니다. |
| **GetSubstanceLoadingProgress** | 없음 | 가득 찬 물질의 수를 백분율로 0에서 1 사이의 플로트를 반환합니다. |
| **CreateGraphInstance** | 입력: **SubstanceInstanceFactory** - 그래프 인스턴스를 만들 팩터리입니다.입력: **GraphIndex**(int) - 만들 그래프의 인덱스입니다. 입력: **InstanceName**(FString) - 새 인스턴스에 지정할 이름입니다. | 응용 프로그램이 종료될 때까지 유지되는 새 독립 실행형 그래프 인스턴스를 반환합니다. |
| **DuplicateGraphInstance** | **SubstanceGraphInstance** - 복사본을 만들 그래프 인스턴스입니다. | 응용 프로그램이 종료될 때까지 유지되는 새 독립 실행형 그래프 인스턴스를 반환합니다. |
| **인스턴스 출력 사용** | 입력: **SubstanceGraphInstance** - 입력을 활성화하는 출력이 포함된 그래프 인스턴스: **OutputIndexes**(int32 배열) - 활성화할 출력의 인덱스입니다. | 이전에 사용하지 않도록 설정한 경우 **SubstanceGraphInstance**&#x200B;에 전달된 텍스처 출력을 만듭니다. 이 기능은 **SubstanceGraphInstance** 편집기의 출력을 활성화하는 것과 동일합니다. *참고: 새로 만든 텍스처로 재질이 업데이트되지 않습니다. 새 출력을 사용하여 런타임에 sampler 매개 변수를 설정하여 처리해야 합니다.* |
| **DisableInstanceOutput** | 입력: **SubstanceGraphInstance** - 입력을 비활성화하는 출력이 포함된 그래프 인스턴스: **OutputIndexes**(int32 배열) - 비활성화하려는 출력의 인덱스입니다. | 활성화된 경우 은 그래프 객체에서 전달된 텍스처 출력을 비활성화하고 삭제합니다 |
| **복사 입력 매개 변수** | 입력: **SubstanceGraphInstance** - 값을 적용할 그래프 인스턴스 입력: **SubstanceGraphInstance** - 값을 가져올 그래프 인스턴스 | Substance 그래프 인스턴스 입력 매개 변수의 변경된 모든 입력 값을 복원합니다. |
| **ResetInputParameters** | 입력: SubstanceGraphInstance | Substance 그래프 인스턴스의 입력 값을 기본값으로 다시 설정 |
| **SetGraphInstanceOutputSize** | 입력: **SubstanceGraphInstance**&#x200B;입력: 너비 - X 좌표의 텍스처 해상도입력: Height - Y 좌표의 텍스처 해상도 | 매개 변수에서 전달된 크기로 이 그래프 인스턴스에서 생성된 모든 출력의 텍스처 해상도를 설정합니다. 참고 - CPU 엔진의 Max 2048참고 - GPU 엔진의 Max 4096 |
| **비동기 렌더링** | **SubstanceGraphInstance** | Substance 그래프 텍스처 입력의 출력 인스턴스를 다시 계산합니다. (차단 금지) |
| **동기화 렌더링** | **SubstanceGraphInstance** | Substance 그래프 텍스처 입력의 출력 인스턴스를 다시 계산합니다. (차단) |

## 그래프 인스턴스 특정 함수:

그래프 인스턴스에서만 호출할 수 있습니다.

| 이름 | 입력 | 설명 |
| --- | --- | --- |
| GetDynamicMaterialInstance | 입력: 이름(문자열) | Substance의 런타임 동적 재질 인스턴스를 반환하거나 인스턴스가 없는 경우 인스턴스를 만듭니다. Substance 값 출력에서 대부분의 런타임 값 변경에는 동적 재질 인스턴스가 필요합니다. |
| **GetInputNames** | 없음 | 모든 입력 매개 변수 이름을 포함하는 Strings 배열을 반환합니다. |
| **GetInputType** | 없음 | 이 입력과 연결된 데이터 형식을 반환합니다. |
| **SetInputInt** | 입력: **식별자**(문자열)입력: **InputValues**(int 배열) | 식별자에서 찾은 입력 값을 변경합니다. 게임 내에서 변경 내용을 적용하려면 **AyncRender** 또는 **SyncRender**&#x200B;을 사용하여 Substance를 렌더링해야 합니다. |
| **SetInputFloat** | 입력: **식별자**(문자열)입력: **InputValues**(부동 배열) | 식별자에서 찾은 입력 값을 변경합니다. 게임 내에서 변경 내용을 적용하려면 **AyncRender** 또는 **SyncRender**&#x200B;을 사용하여 Substance를 렌더링해야 합니다. |
| **GetInputInt** | 입력: **식별자**(문자열) | 입력 매개 변수의 현재 값을 사용하여 정수 배열을 반환합니다. |
| **GetInputFloat** | 식별자(문자열) | 입력 매개 변수의 현재 값을 사용하여 부동 배열을 반환합니다. |
| **SetInputBool** | 입력: **부울**(부울)입력: **식별자**(문자열) | 부울 값을 입력하여 토글할 수 있는 입력 값 유형을 할당합니다. 이전에는 bool에 casing된 int 값을 1 또는 0으로 설정해야만 이를 수행할 수 있었습니다. |
| **GetInputBool** | 입력: **식별자**(문자열) | 입력의 현재 부울 값을 반환합니다. |
| **SetInputColor** | 입력: **색상**(LinearColor)입력: **식별자**(FString) | 색상 입력 값 유형을 할당할 FLinearColor 값을 가져옵니다. 이전에는 부동 소수점 값을 설정하고 부동 소수점 배열을 전달하기만 했습니다. |
| **GetInputColor** | 입력: 식별자(FString) | 현재 색상 값을 UE4 형식으로 반환합니다. |
| **CreateAggregateSubstanceFactory** | 입력: **출력 팩토리**(SubstanceInstanceFactory)*입력 팩터리에 대한 입력으로 사용할 출력을 만드는 팩터입니다.*&#x200B;입력: **출력 팩토리 그래프 인덱스**(정수)*결합하는 데 사용할 substance 내의 그래프.* 입력: **입력 팩터리**(SubstanceInputFactory)*출력 팩터리의 입력 이미지로 출력을 사용하는 팩터리입니다.*입력:**연결**(SubstanceConnections 배열)*청사진 노드 만들기 배열을 사용하여 만들 수 있습니다. Substance 연결은 어떤 출력을 연결해야 하는 집계 노드를 연결하는 방법입니다.* **&#x200B; Return(SubstanceInstanceFactory)***을(를) 사용하여 새 결합된 인스턴스의 그래프 인스턴스를 만들 수 있습니다.* | 새 집계 Substance 노드를 사용하면 두 개의 Substance 인스턴스 팩터리를 가져와 런타임에 새 인스턴스 팩터리를 만들 수 있습니다. 이 팩터리는 새 그래프 인스턴스를 만드는 데 사용할 수 있습니다. 이렇게 하면 결합된 그래프 인스턴스 중 하나의 출력 텍스처를 다른 결합된 그래프 인스턴스의 입력 이미지에 연결할 수 있다는 점이 특별해집니다. 이 새 팩터리에서 Substance Graph 인스턴스를 만들려면 런타임 그래프 인스턴스에 대한 설명서를 참조하십시오. |
| **SubstanceConnectionStruct** | 입력: **출력 식별자**(FString)*입력에 연결할 텍스처 출력의 식별자.* 입력: **입력 식별자**(FString) | 집계 Substance 팩터리 만들기에서 각 출력 텍스처를 새 입력 텍스처로 연결하는 방법을 지정하는 데 사용됩니다. |
