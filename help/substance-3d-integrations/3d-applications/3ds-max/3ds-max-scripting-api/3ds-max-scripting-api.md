---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-scripting-api.html"
breadcrumb-title: ''
description: 재료 작업을 자동화하는 Substance 3ds Max 스크립팅 API에 대한 참조 설명서.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds MAX Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds MAX 스크립팅 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 2%

---


# 3ds MAX 스크립팅 API

다음은 Substance 2 노드의 명령 및 속성 목록입니다.

## 속성:

| 속성 | 설명 | 유형 |
| --- | --- | --- |
| 이름 | Substance2 노드의 이름입니다. 기본값은 &quot;Substance 2&quot;입니다. | 문자열 |

## 명령:

| Command | 설명 | 돌아가기 | 반환 유형: | 매개변수 |
| --- | --- | --- | --- | --- |
| getCurrent패키지 이름 | 로드된 패키지의 기본 파일 이름(그래프 노드에 로드된 sbsar 파일)을 가져옵니다. | 로드된 패키지(sbsar 파일)의 파일 이름(접두어 디렉터리 제외) | 문자열 |  |
| getCurrentGraphName | 현재 그래프의 이름 가져오기 | 현재 그래프 인스턴스의 식별자 | 문자열 |  |
| getOutputsNamesFromCurrentGraph | 활성화된 출력의 출력 사용 이름 목록 가져오기 | 활성화된 출력의 채널 이름 목록이 포함된 표 | 목록 |  |
| getPresetIdentifiers | Substance 그래프에서 사전 설정 목록 가져오기 | 모든 사전 설정에 대한 문자열 식별자 목록이 포함된 표 | 목록 |  |
| setPackageAndGraphName | 디스크에서 그래프 노드로 sbsar 파일 로드 | 성공하면 참, 실패하면 거짓 | 부울 | ***문자열 매개 변수***: **substancePackageFilePath** disk ***String 매개 변수의 sbsar 파일 경로***: **graphInstanceNameToSelect** 그래프의 문자열 식별자 |
| setInputInt | 새 값을 사용하여 정수 입력 설정 |  |  | ***정수 매개 변수***: **값** 입력을 {String 매개 변수로 설정할 정수 값&#x200B;***:** inputIdentifier***5} 입력의 고유 문자열 식별자** |
| setInputFloat | 새 값으로 부동 입력 설정 |  |  | ***부동 매개 변수***: **값** 입력을 {String 매개 변수로 설정하는 부동 값&#x200B;***:** inputIdentifier***5} 입력의 고유 문자열 식별자** |
| setInputString | 새 값으로 문자열 입력 설정 |  |  | ******&#x200B;문자열 매개 변수&#x200B;***:**&#x200B;값&#x200B;**입력을 {String 매개 변수로 설정할 문자열 값***: **inputIdentifier** 입력의 고유 문자열 식별자 |
| setInputBool | 새 값을 사용하여 부울 입력 설정 |  |  | ***부울 매개 변수:* 값&#x200B;**입력을***문자열 매개 변수로 설정하는 부울 값&#x200B;***: **inputIdentifier** 입력의 고유 문자열 식별자 |
| setInputVec2 | 두 개의 요소로 벡터 입력 설정 |  |  | ***Point2 매개 변수:*****value** 입력을 ***String 매개 변수로 설정할 최대 point2 값&#x200B;***: **inputIdentifier** 입력의 고유 문자열 식별자 |
| setInputVec3 | 세 가지 요소로 벡터 입력 설정 |  |  | ***Point3 매개 변수:* 값&#x200B;**입력을***String 매개 변수로 설정할 최대 point3 값&#x200B;***: **inputIdentifier** 입력의 고유 문자열 식별자 |
| setInputVec4 | 4개 요소로 벡터 입력 설정 |  |  | ***Point4 매개 변수***: **값** 입력을 ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자로 설정하는 최대 point4 값 |
| setInputColor | 새 값으로 색상 입력 설정 |  |  | ***색상 매개 변수***: **값** 입력을 ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자로 설정할 최대 색상 값 |
| setInputComboSelection | 콤보 상자 입력에서 현재 선택한 값 설정 |  |  | ***정수 매개 변수***: 콤보 상자 위젯의 **값** 인덱스&#x200B;***문자열 매개 변수***: **inputIdentifier** 입력의 고유 문자열 식별자 |
| getInputInt | 정수 입력 유형에 대한 입력 값 가져오기 | 입력의 현재 정수 값 | 정수 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputFloat | 부동 입력 유형에 대한 입력 값 가져오기 | 입력의 현재 부동 소수점 값 | 부동 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputString | 문자열 입력 유형에 대한 입력 값 가져오기 | 입력의 현재 문자열 값입니다. | 문자열 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputBool | 부울 입력 유형에 대한 입력 값 가져오기 | 입력의 현재 부울 값입니다. | 부울 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputVec2 | point2 입력 유형에 대한 입력 값 가져오기 | 입력의 현재 최대 point2 값입니다. | Point2 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputVec3 | point3 입력 유형에 대한 입력 값 가져오기 | 입력의 현재 최대 point3 값입니다. | Point3 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputVec4 | Point4 입력 유형에 대한 입력 값 가져오기 | 입력의 현재 최대 point4 값입니다. | Point4 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputColor | 색상 입력 유형에 대한 입력 값 가져오기 | 입력 색상의 현재 값 | 색상 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getInputComboSelection | 식별자 기반의 콤보 상자 선택 색인 가져오기 | 선택한 콤보 상자 항목의 인덱스입니다 | 정수 | ***문자열 매개 변수:* inputIdentifier **입력의 고유 문자열 식별자입니다. |
| getMaterialDependentCount | 재질 종속성 수를 가져옵니다. | 재료 유형의 종속 참조 수 | 정수 |  |
| ApplyValuesToSelectedPreset | 현재 선택된 사전 설정을 현재 입력 값으로 재정의합니다 |  |  |  |
| RemoveAllPresets | 현재 그래프 노드의 모든 사전 설정을 제거합니다 |  |  |  |
| CreatePreset | 현재 입력에서 새 사전 설정 만들기 |  |  | ***문자열 매개 변수:* newPresetName **새 사전 설정의 표시 이름 |
| RemoveOnePreset | 지정된 이름의 사전 설정 제거 |  |  | ***문자열 매개 변수:* selectedPresetName **제거할 사전 설정 이름 |
| ImportPreset | sbsprs 파일을 현재 사전 설정으로 가져오기 |  |  | ***String 매개 변수:*****filePath** 사전 설정을 가져올 파일 경로를 포함하는 문자열 |
| ExportPreset**\*deprecated** 2.5.0에서 제거\* | 현재 선택된 사전 설정을 sbsprs 파일로 내보내기 |  |  | ***문자열 매개 변수***: **filePath** 사전 설정을 내보낼 파일 경로를 포함하는 문자열 |
| exportPresetList | 주어진 사전 설정을 단일 사전 설정 파일로 내보내기 |  |  | ***문자열 매개 변수***: **filePath** 사전 설정을 내보낼 파일 경로를 포함하는 문자열&#x200B;***List 매개 변수***: **사전 설정** 내보낼 사전 설정의 이름을 포함하는 목록 |
| BakeOutputsOfSelectedGraph | 선택한 그래프 인스턴스의 비트맵을 디스크로 굽기 |  |  | ***문자열 매개 변수:* filePath **이미지를 기록할 루트 경로 디렉터리***문자열 매개 변수&#x200B;***: **imageFormatExtension** 이미지를 기록할 파일 확장명/형식 |
