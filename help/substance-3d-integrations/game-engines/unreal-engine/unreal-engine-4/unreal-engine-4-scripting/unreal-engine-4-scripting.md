---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/unreal-engine-4-scripting.html"
breadcrumb-title: ''
description: Substance Unreal Engine 4 스크립팅 API 를 사용하여 프로젝트의 Substance 자료를 프로그래밍 방식으로 관리합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Unreal Engine 4 Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 언리얼 엔진 4 스크립팅
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# 언리얼 엔진 4 스크립팅

Unreal Engine 플러그인의 Substance은 스크립팅할 수 있습니다. 플러그인의 SubstanceGraphInstance.h 파일에 메서드가 나열되고 주석이 추가되며, 일반적으로 마켓플레이스에서 플러그인을 설치할 때 다음 디렉터리에 있습니다.

* **엔진 설치**: [UE\_4.X.X 위치]\Engine\Plugins\Marketplace\Substance\Source\SubstanceCore\Classes\SubstanceGraphInstance.h
* **프로젝트 설치**: [프로젝트 폴더 위치]\Plugins\Runtime\Substance\Source\SubstanceCore\Classes\SubstanceGraphInstance.h

  ![](../../../../assets/substancegraphinstance.png)

`BlueprintCallable`은(는) 메서드가 청사진 편집기에서도 사용 가능함을 나타냅니다.

## Unreal Engine의 Python 편집기에서 스크립팅

Unreal Engine의 Python 편집기에서 SubstanceGraphInstance.h 파일에 나열된 메서드를 사용할 때는 Pascal Case에서 Snake Case로 변환해야 합니다(각 단어 사이에 소문자와 밑줄이 있음). 예를 들어 `SetInputColor`은(는) `set_input_color`이(가) 됩니다.

[언리얼 엔진]의 [Python 편집기]는 [윈도우] > [개발자 도구] > [출력 로그]를 통해 액세스할 수 있고 왼쪽 아래 드롭다운을 Python으로 설정할 수 있습니다.

## 예제 스크립트

다음은 Python 편집기에서 사용할 수 있는 예제 스크립트 세트입니다.

## Substance 재질 만들기

```
## Python example on creating a Substance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create graph instance

for graph_desc in graph_descs: 

    print(graph_desc) 

## You could name based on label or on index or another way

    graph_name = "/Game/FirstInstance_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

## graph_name = f"/Game/FirstInstance_{graph_desc.index}"

## material_name = f"/Game/FirstMaterial_{graph_desc.index}"

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True)
```


## Substance 재질의 단일 그래프 만들기

```
## Python example on creating a Substance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create only 1 graph instance

graph_desc = graph_descs[0] 

print(graph_desc) 

graph_name = "/Game/MyGraphInstance" 

material_name = "/Game/MyMaterial" 

graph = factory.create_graph_instance(graph_desc, graph_name) 

graph.create_outputs() 

graph.create_material(material_name, mats[0]) 

graph.set_input_color("obsidian_color", unreal.LinearColor(0, 1, 1)) 

graph.set_input_color("lava_color", unreal.LinearColor(1, 0, 0)) 

graph.prepare_outputs_for_save() 

graph.render_sync() 

graph.save_all_outputs(True)
```


## 서로 다른 매개변수를 사용하여 Substance 재료의 여러 인스턴스를 생성합니다.

```
## Python example on creating mulitple Substance materials.

 

import unreal 

 

## Create factory. Should only need 1 factory, even if multiple instances are created

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create first graph instance

for graph_desc in graph_descs: 

    graph_name = "/Game/FirstInstance_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True) 

 

## Create second graph instance

for graph_desc in graph_descs: 

    graph_name = "/Game/SecondInstance_" + graph_desc.label 

    material_name = "/Game/SecondMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(1, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(1, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True)
```


## Substance 그래프 복제

```
## Python example on duplicating a Subtance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create first graph

for graph_desc in graph_descs: 

    print(graph_desc) 

    graph_name = "/Game/FirstGraph_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

 

## Duplicate graph

new_material_name = "/Game/SecondMaterial" 

new_graph = graph.duplicate() 

new_graph.create_outputs() 

new_graph.create_material(new_material_name, mats[0]) 

new_graph.prepare_outputs_for_save() 

new_graph.render_sync()
```
