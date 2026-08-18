---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntime-class.html"
breadcrumb-title: ''
description: Unity에서 런타임 Substance 재료 작업에 사용되는 SubstanceRuntime 클래스에 대한 참조 문서입니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntime Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceRuntime 클래스
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 1%

---


# SubstanceRuntime 클래스

## Adobe.Substance.런타임.SubstanceRuntime 클래스 참조

Substance 엔진 초기화를 처리하는 Singleton 클래스이며 기본 처리기를 Substance 인스턴스로 가져오는 데 사용됩니다.\
Adobe.Substance.Runtime.SubstanceRuntime의 상속 다이어그램:

![](../../../../../assets/image2022-6-22-14-35-28.png)

### 공용 멤버 함수

```
• SubstanceNativeGraph InitializeInstance (SubstanceGraphSO substanceInstance)
```


지정된 SubstanceGraphSO에 대한 Substance SDK 핸들을 만듭니다.

### 속성

```
• static SubstanceRuntime Instance [get]
```


단일 인스턴스.

### 자세한 설명

Substance 엔진 초기화를 처리하는 Singleton 클래스이며 기본 처리기를 Substance 인스턴스로 가져오는 데 사용됩니다.

### 멤버 함수 설명서

#### InitializeInstance()

```
SubstanceNativeGraph Adobe.Substance.Runtime.SubstanceRuntime.InitializeInstance  

( SubstanceGraphSO substanceInstance ) [inline]
```


지정된 SubstanceGraphSO에 대한 Substance SDK 핸들을 만듭니다.

**매개 변수**

|  |  |
| --- | --- |
| substanceInstance | 대상 SubstanceGraphSO |


**반환**

Substance SDK와 통신하는 핸들

### 등록 정보 설명서

#### 인스턴스

```
SubstanceRuntime Adobe.Substance.Runtime.SubstanceRuntime.Instance [static], [get]
```


단일 인스턴스.

전역 단일 인스턴스.

>[!NOTE]
>
> NativeGraph.InRenderWork는 내부용으로만 Substance 엔진과 통신하기 위한 것으로, 사용자 정의 워크플로우에 사용해서는 안 됩니다.
