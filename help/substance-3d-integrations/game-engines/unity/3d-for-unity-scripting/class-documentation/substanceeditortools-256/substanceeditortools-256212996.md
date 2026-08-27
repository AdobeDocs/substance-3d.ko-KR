---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceeditortools-256212996.html"
breadcrumb-title: ''
description: Unity에서 Substance 재질 관리에 사용되는 SubstanceEditorTools 클래스의 참조 문서입니다.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceEditorTools
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# SubstanceEditorTools

## Adobe.SubstanceEditor.SubstanceEditorTools 클래스 참조

사용자가 편집기 스크립트에서 활용할 수 있는 도구 및 유틸리티입니다.

Adobe.SubstanceEditor.SubstanceEditorTools의 상속 다이어그램:

![](../../../../../assets/image2022-10-14-17-53-23.png)

### 정적 공용 멤버 함수

```
• static void SetGraphFloatInput (SubstanceGraphSO graph, int inputId, float value)
```


그래프 부동 입력을 설정합니다.

```
• static void SetGraphFloat2Input (SubstanceGraphSO graph, int inputId, Vector2 value)
```


그래프 float2 입력을 설정합니다.

```
• static void SetGraphFloat3Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


그래프 float3 입력을 설정합니다.

```
• static void SetGraphFloat4Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


그래프 float4 입력을 설정합니다.

```
• static void SetGraphIntInput (SubstanceGraphSO graph, int inputId, int value)
```


그래프 int 입력을 설정합니다.

```
• static void SetGraphInt2Input (SubstanceGraphSO graph, int inputId, Vector2Int value)
```


그래프 int2 입력을 설정합니다.

```
• static void SetGraphInt3Input (SubstanceGraphSO graph, int inputId, Vector3Int value)
```


그래프 int3 입력을 설정합니다.

```
• static void SetGraphInt4Input (SubstanceGraphSO graph, int inputId, int value0, int value1, int value2, int value3)
```


그래프 int4 입력을 설정합니다.

```
• static void SetGraphInputString (SubstanceGraphSO graph, int inputId, string value)
```


그래프 문자열 입력을 설정합니다.

```
• static void SetGraphInputTexture (SubstanceGraphSO graph, int inputId, Texture2D value)
```


그래프 텍스처 입력을 설정합니다.

```
• static void RenderGraph (SubstanceGraphSO graph)
```


대상 그래프를 렌더링하고 자산을 업데이트합니다.

```
• static string CreatePresetFromCurrentState (SubstanceGraphSO graph)
```


그래프 오브젝트의 현재 상태에서 사전 설정 XML을 만듭니다.

```
• static List< SubstanceGraphSO > GetGraphs (this SubstanceFileSO fileSO)
```


SubstanceFileSO와 연결된 SubstanceGraphSO 목록을 반환합니다.
