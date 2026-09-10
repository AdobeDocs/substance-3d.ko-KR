---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-4.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.3.4의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# 유니티 .

>[!WARNING]
>
> **Unity 2019.2에서 플러그인을 사용하면 다음 오류가 발생합니다.**
> 
> InspectorSubstanceImporter.OnInspectorGUI는 예기치 않은 동작을 방지하기 위해 ApplyRevertGUI를 호출해야 합니다.\
> UnityEditor.Experimental.AssetImporters.AssetImporterEditor:OnDisable()\
> Substance.Editor.InspectorSubstanceImporter:OnDisable()
> 
> 이 오류는 지울 수 있으며 플러그인의 기능에는 영향을 주지 않습니다.

>[!WARNING]
>
> **읽어 보세요. Substance 재질 분리:**\
> 빈 용도의 사용자 정의 출력을 포함하는 Substance 재질은 가져올 때 중단됩니다. 또한 중복 사용이 포함된 Substance 재질은 중단됩니다.\
> GameTextures.com의 이전 sbsar 파일은 현재 Unity 플러그인의 Substance과 호환되지 않습니다. 지원되지 않는 사용 출력이 포함된 이러한 재질은 중단됩니다. 플러그인을 사용하기 전에 프로젝트를 백업해야 합니다.

## 새로운 기능:

* Substance 엔진 v7에 대한 지원 추가
* Linux 지원 추가

### 버그 수정:

* 텍스처 맵 없이 Substance 가져오기와 관련된 문제 수정
* Unity 2019.x에서 반사 프로세스가 올바르게 작동하지 않는 문제를 해결했습니다.
* Substance 재질이 있는 프리팹을 포함하는 패키지를 가져올 때 발생하는 프리팹 처리 문제를 수정했음
* 반영 프로세스 후 고정 재료/텍스처 할당이 이월되지 않음
* 반사판의 변경으로 인해 재질이 손상되는 문제를 해결했습니다.
* 금속 알파 채널에 거칠기가 채워지지 않는 문제를 해결했습니다.
* Substance 플러그인을 설치할 때 비 Substance 텍스처에 대한 가져오기 설정을 변경하면 특정 옵션이 되돌리는 문제를 수정했습니다.
* Mac에서 Substance Source이 열리지 않는 문제를 수정했음

## 알려진 문제:

**핵심 Substance 플러그 인**

* iOS용으로 빌드하려면 사용자가 Xcode의 빌드 설정 메뉴에서 &#39;Bitcode 사용&#39;을 비활성화해야 합니다.
* Substance은 에셋 번들에서 작동하지 않습니다.
* 다시 가져오기 후 에셋 브라우저의 Substance 미리보기 아이콘이 모두 Substance 아이콘으로 변경됩니다
* 사용량이 공백으로 설정된 출력이 있는 사용자 정의 Substance 재질은 재질을 분할합니다.
* 중복된 용도가 있는 사용자 정의 Substance 재질은 재질을 저하시킵니다.
* Linux에서 플러그인을 가져온 후 편집기를 다시 시작해야 합니다.

**스크립팅**

* 프로젝트가 빌드 설정에서 x86으로 설정되어 있으면 스크립팅이 런타임에 작동하지 않습니다
* 특정 빌드 플랫폼에서 il2cpp 스크립팅 백엔드를 사용하는 문제

**Substance Painter 라이브 링크**

* Substance 라이브 링크로 페인팅한 후 프로젝트를 빌드하면 페인팅된 메쉬가 다시 기본 재질로 설정됩니다
* AO 채널이 Painter 라이브 링크와 함께 전송되지 않음
* 여러 재질이 있는 메시는 Unity Live Link에서 작동하지 않습니다
* Unity LiveLink가 SimpleJson을 사용하는 방식은 프로젝트에서 SimpleJson의 다른 인스턴스와 충돌합니다
