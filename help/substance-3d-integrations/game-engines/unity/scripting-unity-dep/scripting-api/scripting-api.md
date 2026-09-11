---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/scripting-api.html"
breadcrumb-title: ''
description: 레거시 프로젝트 지원에 대해 더 이상 사용되지 않는 Substance Unity 스크립팅 API에 대한 참조 설명서.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 스크립팅
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 1%

---


# 스크립팅

## Unity API Substance - 2.2.0

## Substance 재료 매개변수

| Public 메서드 | 설명 | 매개변수 |
| --- | --- | --- |
| public **float** *GetInputFloat*(**string** inputName) | Substance **부동** 입력 가져오기 | SBSAR의 **문자열** *입력 이름* 입력 이름 |
| public **int** *SetInputFloat*(**string** inputName, **float** 값) | Substance **부동** 입력 업데이트 | 매개 변수를 업데이트하는 데 사용되는 SBSAR **부동** *값* 값의 **문자열** i *nputName* 입력 이름 |
| public **void** *SetInputVector2*(**string** inputName, **Vector2** 값) | Substance **Vector2** 입력 업데이트 | **문자열** *입력 이름* 매개 변수를 업데이트하는 데 사용되는 SBSAR **벡터2** *입력* 값의 입력 이름 |
| 공용 **벡터2** *GetInputVector2*(**문자열** inputName) | Substance **Vector2** 입력 가져오기 | SBSAR의 **문자열** &quot;inputName&quot; 입력 이름 |
| public **void** *SetInputVector3*(**string** inputName, **Vector3** 값) | Substance **Vector3** 입력 업데이트 | **문자열** *입력 이름* 매개 변수를 업데이트하는 데 사용되는 SBSAR **벡터3** *값* 값의 입력 이름 |
| 공용 **벡터3** *GetInputVector3*(**문자열** inputName) | Substance **벡터3** 입력 가져오기 | SBSAR의 **문자열** *입력 이름* 입력 이름 |
| public **void** *SetInputVector4*(**string** inputName, **Vector4** 값) | Substance **Vector4** 입력 업데이트 | **문자열** *입력 이름* 매개 변수를 업데이트하는 데 사용되는 SBSAR **벡터4** *값* 값의 입력 이름 |
| 공개 **벡터4** *GetInputVector4*(**문자열** inputName) | Substance **Vector4** 입력 가져오기 | SBSAR의 입력 **문자열** inputName 이름 |
| 공용 **void** *SetInputColor*(**문자열** inputName, **색상** 값) | Substance **색상** 입력 업데이트 | 매개 변수를 업데이트하는 데 사용되는 SBSAR **색상** 값의 **문자열** inputName 입력 |
| 공용 **색상** *GetInputColor*(**문자열** inputName, **int** dataType) | Substance **색상** 가져오기 | **문자열** *입력 이름* SBSAR **Int** *dataType*&#x200B;의 입력 이름 |
| public **void** *SetInputBool*(**string** inputName, **bool** 값) | Substance **부울** 입력 업데이트 | **문자열** *입력 이름* 매개 변수를 업데이트하는 데 사용되는 SBSAR **Bool** *값* 값의 입력 이름 |
| 공용 **bool** *GetInputBool*(**문자열** inputName) | Substance **부울** 입력 가져오기 | SBSAR의 **문자열** *입력 이름* 입력 이름 |
| public **void** *SetInputInt*(**string** inputName, **int** 값) | Substance **Int** 입력 업데이트 | **문자열** *입력 이름* 매개 변수를 업데이트하는 데 사용되는 SBSAR **Int** *값* 값의 입력 이름 |
| 공용 **int** *GetInputInt*(**문자열** inputName) | Substance **Int** 입력 가져오기 | SBSAR의 **문자열** *입력 이름* 입력 이름 |
| public **void** *SetInputVector2Int*(**string** inputName, **int** x, **int** y) | Substance **Vector2Int** 입력 업데이트 | **문자열** *입력 이름* SBSAR **Int** *x* 매개 변수를 업데이트하는 데 사용되는 값 **Int** y 매개 변수를 업데이트하는 데 사용되는 값 |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector2Int*( string inputName) | 2 int의 배열 가져오기(Vector2Int의 x 및 y 값) | **문자열** *입력 이름* SBSAR **Int** *x* 매개 변수를 업데이트하는 데 사용되는 값 **Int** y 매개 변수를 업데이트하는 데 사용되는 값 |
| **void Substance.Game.SubstanceGraph**.*SetInputVector3Int*( string inputName, int x, int y, int z) | Substance Vector3Int 입력 업데이트 | **문자열** *입력 이름* SBSAR **Int** *x* 매개 변수를 업데이트하는 데 사용되는 값 **Int** y 매개 변수를 업데이트하는 데 사용되는 값 **Int** z 매개 변수를 업데이트하는 데 사용되는 값 |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector3Int*( string inputName) | 3 int의 배열 가져오기(Vector3Int의 x, y 및 z 값) | **문자열** *입력 이름* SBSAR **Int** *x* 매개 변수를 업데이트하는 데 사용되는 값 **Int** y 매개 변수를 업데이트하는 데 사용되는 값 **Int** z 매개 변수를 업데이트하는 데 사용되는 값 |
| **void Substance.Game.SubstanceGraph**.*SetInputVector4Int*( string inputName, int x, int y, int z, int w) | Substance Vector4Int 입력 업데이트 | **문자열** *입력 이름* SBSAR **Int** *x* 매개 변수를 업데이트하는 데 사용되는 값 **Int** y 매개 변수를 업데이트하는 데 사용되는 값 **Int** z 매개 변수를 업데이트하는 데 사용되는 값 **Int** w 매개 변수를 업데이트하는 데 사용되는 값 |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector4Int*( string inputName) | 4 int의 배열 가져오기(Vector4Int의 x, y, z 및 w 값) | **문자열** *입력 이름* SBSAR **Int** *x* 매개 변수를 업데이트하는 데 사용되는 값 **Int** y 매개 변수를 업데이트하는 데 사용되는 값 **Int** z 매개 변수를 업데이트하는 데 사용되는 값 **Int** w 매개 변수를 업데이트하는 데 사용되는 값 |
| **void Substance.Game.SubstanceGraph**.*SetInputString*( 문자열 inputName, 문자열 값) | Substance 문자열 입력 업데이트 | **문자열** *입력 이름* 매개 변수를 업데이트하는 데 사용되는 SBSAR **문자열** *값*&#x200B;의 입력 이름 |
| **문자열 Substance.Game.SubstanceGraph**.*GetInputString*( 문자열 inputName) | Substance 문자열 입력 가져오기 | SBSAR의 **문자열** *입력 이름* 입력 이름 |
| **void Substance.Game.SubstanceGraph**.*SetInputTexture*( 문자열 inputName, 텍스처 2D 값) | Substance 텍스처 2D 입력 업데이트 | **문자열** *입력 이름* 매개 변수를 업데이트하는 데 사용되는 SBSAR **텍스처2D** *값*&#x200B;의 입력 이름 |
| **텍스처 2D Substance.Game.SubstanceGraph**.*GetInputTexture*( 문자열 inputName) | Substance 텍스처 2D 입력 받기 | SBSAR의 **문자열** *입력 이름* 입력 이름 |
| **VectorInt Substance.Game.SubstanceGraph**.*GetTexturesResolution*() | 그래프의 대상 설정 텍스처 해상도 가져오기(Vector4Int의 x = 너비, y = Height, 값은 32, 64, 128, 256, 512, 1024, 2048 및 4096일 수 있음) | 없음 |
| **int Substance.Game.SubstanceGraph**.*SetTexturesResolution*( Vector2Int 크기) | Set the graph&#39;s Target Settings 텍스처 resolution (Vector2Int&#39;s x = width, y = Height, values can be 32, 64, 128, 256, 512, 1024, 2048 &amp; 4096) 성공할 경우 0을 반환하고, 그렇지 않으면 -1을 반환합니다. | 매개 변수를 업데이트하는 데 사용되는 **Vector2Int** *크기&lbrace;3&#x200B;**.*** |
| **List Substance.Game.SubstanceGraph**.*GetGeneratedTextures*() | 그래프의 질감 셰이더에 사용되는 모든 Substance 텍스처 2D 개체를 반환합니다. | 없음 |
| **int Substance.Game.SubstanceGraph**.*굽기*( 텍스처 2D 텍스처, 문자열 absolutePath) | 그래프의 질감 셰이더에 사용되는 모든 Substance 텍스처 2D 오브젝트에 대한 .png 파일을 생성합니다. | 없음 |
| **&#x200B;**&#x200B;Substance.게임.**&#x200B; SubstanceGraph**.*복제*() | Substance 그래프 복제 | 없음 |
| **Substance.Game.SubstanceGraph**.*복제*(문자열 newGraphName) | Substance 그래프를 복제하고 이름을 지정합니다(해당 자료도 이름이 동일함) | **문자열 newGraphName** |
| **&#x200B;**&#x200B;Substance.게임.**&#x200B; SubstanceGraph**.*GetInputProperties*() | 프로시저 입력 정보를 쿼리하고 :public 구조체 InputProperties { public string name; // inputName public string label; // GUIpublic string의 위젯 레이블; // GUIpublic string[] componentLabels의 위젯 그룹; // 슬라이더(최대 4개 레이블)의 경우 public string[] enumOptions; // optionMenupublic InputPropertiesType의 경우 public Vector4 maximum; // 슬라이더 퍼블릭 Vector4 minimum; // 슬라이더 퍼블릭 부동 단계의 경우 // 슬라이더 }public enum InputPropertiesType { Boolean = 0,/ 0 부동, // 1 Vector2, // 2 Vector3, // 3 Vector4, // 4 color/ 의 배열을 반환합니다. 5 열거형, // 6 텍스처, // 7 문자열, // 8 유효하지 않음 = -1// -1 }; | 없음 |
| **bool** **Substance.Game.SubstanceGraph**.*HasInput*(**문자열** inputName) | 그래프에 입력이 있는지 확인하고 true/false를 반환합니다. | SBSAR의 **문자열** *입력 이름* 입력 이름 |
| **bool** **Substance.Game.SubstanceGraph**.*IsInputVisible*(**문자열** inputName) | visibleif 입력이 표시되는지 확인합니다. true/false를 반환합니다. | SBSAR의 **문자열** *입력 이름* 입력 이름 |

## 렌더링 중

| Public 메서드 | 설명 | 매개변수 |
| --- | --- | --- |
| 공개 **void** *QueueForRender*() | 대기열에 Substance 그래프 추가 | 없음 |
| ***mySubstance.**&#x200B;RenderAsync()* | 대기 중인 모든 Substance 그래프를 비동기적으로 렌더링 | 없음 |
| ***mySubstance.**&#x200B;RenderSync()* | 대기 중인 모든 Substance 그래프를 동기적으로 렌더링 | 없음 |

## 편집기 모드에서 스크립팅:

[편집기] 모드에서 그래프를 영구적으로 수정하려면 각 해당 Substance을 다시 가져와야 합니다. 이 작업은 다음과 같은 기능으로 수행됩니다.

```
static void ReImportSubstance(Substance.Game.Substance pSubstance)

{



// Re-import Substance object:

SubstanceImporter importer = AssetImporter.GetAtPath(pSubstance.assetPath) as SubstanceImporter;

importer.CommitSubstanceToImporter(pSubstance); // plugin function

EditorUtility.SetDirty(importer);

importer.SaveAndReimport();



}
```


(Substance 플러그인 함수: &#39;CommitSubstanceToImporter&#39;를 사용하여 수정된 모든 그래프 매개 변수 및/또는 입력을 Substance 가져오기 개체에 복사한 다음 Unity의 가져오기 메커니즘을 통해 디스크에 직렬화됨)
