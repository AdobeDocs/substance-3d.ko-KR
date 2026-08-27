---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class/member-function-documentation.html"
breadcrumb-title: ''
description: Unity 스크립팅에서 SubstanceRuntimeGraph 클래스의 모든 멤버 함수에 대한 자세한 설명서입니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class > Member Function Documentation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 멤버 함수 설명서
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 2%

---


# 멤버 함수 설명서

## AttachGraph()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.AttachGraph  

( SubstanceGraphSO graph ) [inline]
```


이 런타임 처리기에 새 그래프 개체를 첨부합니다.

**매개 변수**

|  |  |
| --- | --- |
| 그래프 | 대상 물질 그래프입니다. |

### CreatePresetFromCurrentState()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.CreatePresetFromCurrentState ( ) [inline]
```


현재 그래프 상태를 사전 설정 XML에 저장합니다.

**반환**

그래프 입력의 현재 상태를 사용하여 만든 사전 설정입니다.

### GetGeneratedTextures()

```
List< Texture2D > Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetGeneratedTextures ( ) [inline]
```


Substance 인스턴스에 대한 모든 출력 텍스처가 있는 목록을 반환합니다.

**반환**

출력 텍스처.

### GetInputBool()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputBool ( string inputName ) [inline]
```


Substance 부울 입력을 가져옵니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름입니다. |


**반환**

현재 입력 값입니다.

### GetInputColor()

```
Color Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputColor ( string inputName ) [inline]
```


Substance 색상 가져오기

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputDescription()

```
SubstanceInputDescription Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputDescription ( string inputName ) [inline]
```


대상 입력 이름에 대한 전체 입력 설명을 반환합니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | 대상 입력 이름입니다. |


**반환**

대상 입력에 대한 입력 설명을 완료합니다.

### GetInputFloat()

```
float Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputFloat ( string inputName ) [inline]
```


Substance 부동 입력 가져오기

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputInt()

```
int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputInt ( string inputName ) [inline]
```


Substance Int 입력 가져오기

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputString()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputString ( string inputName ) [inline]
```


Substance 문자열 입력을 가져옵니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 값을 입력합니다.

### GetInputVector2()

```
Vector2 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2 ( string inputName ) [inline]
```


Vector2 Substance 입력 가져오기

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputVector2Int()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2Int ( string inputName ) [inline]
```


2 int의 배열을 가져옵니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputVector3()

```
Vector3 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3 ( string inputName ) [inline]
```


Substance Vector3 입력을 가져옵니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputVector3Int()

```
Vector3Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3Int ( string inputName ) [inline]
```


3 int의 배열 가져오기(Vector3Int의 x, y 및 z 값)

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputVector4()

```
Vector4 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4 ( string inputName ) [inline]
```


Substance Vector4 입력 가져오기

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetInputVector4Int()

```
int[] Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4Int ( string inputName ) [inline]
```


4 int의 배열 가져오기(Vector4Int의 x, y, z 및 w 값)

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |


**반환**

현재 입력 값입니다.

### GetOutputTexture()

```
Texture2D Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetOutputTexture ( string outputName ) [inline]
```


지정된 출력 이름에 대한 출력 텍스처를 반환합니다.

**매개 변수**

|  |  |
| --- | --- |
| outputName | 출력 이름. |


**반환**

출력 텍스처입니다.

### GetTexturesResolution()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetTexturesResolution ( ) [inline]
```


인스턴스 텍스처 출력 해상도를 반환합니다.

**반환**

현재 출력 해상도.

### HasInput()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.HasInput ( string inputName ) [inline]
```


이 substance 인스턴스에 지정된 이름의 입력이 있는 경우 true를 반환합니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | 이름을 입력합니다. |


**반환**

substance 인스턴스에 지정된 이름의 입력이 있는 경우 TRUE입니다.

### LoadPreset()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.LoadPreset ( string presetXML ) [inline]
```


사전 설정 XML을 사용하여 그래프 입력 매개 변수를 설정합니다.

**매개 변수**

|  |  |
| --- | --- |
| 사전 설정 XML | 사전 설정 XML 데이터. |

### RenderAsync()

```
Task Adobe.Substance.Runtime.SubstanceRuntimeGraph.RenderAsync ( ) [inline]
```


Substance 인스턴스를 비동기적으로 렌더링합니다.

**반환**

렌더링이 완료되면 완료되는 작업입니다.

### SetInputBool()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputBool ( string inputName, 

bool value ) [inline]
```


Substance 부울 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputColor()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputColor ( string inputName, 

Color value ) [inline]
```


Substance 색상 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputFloat()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputFloat ( string inputName, 

float value ) [inline]
```


Substance 부동 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputInt()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputInt ( string inputName, 

int value ) [inline]
```


Substance Int 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputString()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputString ( string inputName, 

string value ) [inline]
```


Substance 문자열 입력을 업데이트합니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputTexture()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputTexture (string inputName, 

Texture2D value ) [inline]
```


Substance Texture2D 입력을 업데이트합니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputVector2()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2 ( string inputName, 

Vector2 value ) [inline]
```


Substance Vector2 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputVector2Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2Int ( string inputName, 

Vector2Int value ) [inline]
```


Substance Vector2Int 입력을 업데이트합니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputVector3()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3 ( string inputName, 

Vector3 value ) [inline]
```


Substance Vector3 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputVector3Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3Int ( string inputName, 

Vector3Int value ) [inline]
```


Substance Vector3Int 입력을 업데이트합니다.

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputVector4()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4 ( string inputName, 

Vector4 value ) [inline]
```


Substance Vector4 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| 값 | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetInputVector4Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4Int ( string inputName, 

int x, 

int y, 

int z, 

int w ) [inline]
```


Substance Vector4Int 입력 업데이트

**매개 변수**

|  |  |
| --- | --- |
| inputName | SBSAR의 입력 이름 |
| x | 매개 변수를 업데이트하는 데 사용되는 값 |
| y | 매개 변수를 업데이트하는 데 사용되는 값 |
| z | 매개 변수를 업데이트하는 데 사용되는 값 |
| w | 매개 변수를 업데이트하는 데 사용되는 값 |

### SetTexturesResolution()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetTexturesResolution ( Vector2Int size ) [inline]
```


인스턴스 텍스처 출력 해상도를 설정합니다.

**매개 변수**

|  |  |
| --- | --- |
| 크기 |  |
