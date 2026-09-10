---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting.html"
breadcrumb-title: ''
description: Unity의 Substance 3D API를 사용하여 런타임에 Substance 매개 변수를 업데이트하고 변경하는 스크립트를 작성할 수 있습니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 스크립팅을 위한 Substance 3D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Unity 스크립팅을 위한 Substance 3D

문서의 이 섹션에는 Unity용 Substance 3D 플러그인을 통해 제공하는 Substance 3D API에 대한 세부 정보가 포함되어 있습니다. Substance API를 사용하면 스크립트를 작성하여 런타임에 Substance 매개 변수를 업데이트하고 변경할 수 있습니다.

## API 개요

플러그인은 세 개의 다른 어셈블리로 나뉩니다.

* Adobe.Substance
* Adobe.Substance.편집기
* Adobe.Substance.런타임

### Adobe.Substance

Substance SDK와 상호 작용하고 일치하는 Unity 개체를 생성하기 위한 공유 구성 요소를 포함합니다. 또한 C#과 Substance SDK C++ API 간의 통신을 위한 데이터 구조를 마샬링합니다.

#### Adobe.Substance.편집기

Unity Substance 개체에 대한 정보 표시를 처리하고 sbsar 파일이 프로젝트에 추가될 때 가져오기 파이프라인을 처리하기 위한 편집기 특정 클래스를 포함합니다. SubstanceEditorEngine 클래스는 Substance 엔진과 모든 관리되는 인스턴스의 수명을 처리하는 단일 클래스입니다.

#### Adobe.Substance.런타임

이 클래스에는 런타임 실행 중에 Substance 개체의 작성 및 관리를 처리하는 구성 요소가 있습니다. SubstanceRuntime은 런타임에 대한 SubstanceEditorEngine 클래스와 동일합니다. Substance Engine의 초기화와 사용자 스크립트가 상호 작용할 Substance 인스턴스의 인스턴스화를 처리합니다.

## 런타임 사용

런타임 시 Substance 인스턴스 입력을 수정하려면 장면에 SubstanceRuntime←- 재질을 추가해야 합니다(Substance 재질과 동일한 GameObject에). 이 클래스는 런타임에 Substance SDK 개체의 인스턴스화를 관리하는 Adobe.Substance.Runtime.SubstanceRuntime 싱글을 사용하여 재질을 설정하는 도우미 역할을 합니다.

## 코드 예제

다음 예제에서는 SubstanceRuntimeGraph를 사용하여 런타임에 입력 매개 변수를 변경하는 방법을 보여 줍니다.

### 매개변수 변경

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    // panel color 

    mySubstance.SetInputColor("paint_color", new Color(0.237 f, 0.834 f, 0.045 f, 1.0 f)); 

    // panel size 

    mySubstance.SetInputVector2("square_open", new Vector2(0.101 f, 0.209 f)); 

    // wear level 

    mySubstance.SetInputFloat("wear_level", 0.977 f); 

    // Submit async render. 

    mySubstance.RenderAsync(); 

  } 

}
```


또한 SubstanceRuntimeGraph를 사용하여 Substance 자료에 대한 입력 및 출력 정보에 액세스할 수 있습니다.

#### 입력 정보 가져오기

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```


다음 예제에서는 SubstanceEditorTools를 사용하여 편집기에서 사용자 정의 사전 설정 메뉴를 만드는 방법을 보여 줍니다.

##### 사전 설정 컨트롤 만들기.

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```
