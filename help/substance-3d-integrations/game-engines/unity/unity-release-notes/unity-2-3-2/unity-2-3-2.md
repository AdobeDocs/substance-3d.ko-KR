---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-2.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.3.2의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# 유니티 .

## 새로운 기능:

* 재료 일련화
* 반사: 이제 플러그인을 통해 패키지의 이전 Substance 파일을 가져올 수 있습니다(가져올 때 자동으로 새 Substance 데이터로 업데이트됨)
* 재질 속성은 Substance 데이터가 있는 패키지를 가져올 때 이전됩니다.
  * 참고: 이는 2.3.0 업데이트 이상을 사용하여 제작된 패키지에만 적용됩니다
* Substance 그래프 메뉴에 베이크 텍스처 버튼 추가

### 버그 수정:

* 라이브러리 폴더가 제거된 경우 Substance 재질 타일링이 재설정되는 문제를 해결했습니다.
* 재생 모드에서 나오는 속도 향상
* Substance DLL이 사용 중일 때 플러그인을 업데이트할 때 발생하는 충돌을 수정했습니다.
* 이제 Unity 내에서 Allegorihmic 폴더를 삭제할 수 없습니다.
  * 참고: Allegorimic 폴더의 내용은 수정할 수 없습니다. Unity 내에서 삭제하면 여러 문제가 발생하여 Unity를 닫았다가 다시 열 때 Allegorithmic 폴더가 마술처럼 다시 나타날 수 있습니다. 이제 프로젝트의 Assets 폴더에서 Unity를 수동으로 닫은 상태로 삭제할 것을 알리는 경고가 표시됩니다.
* 재생 모드에서 나오는 속도 향상
* 라이브러리 폴더를 제거하면 Substance 재질 속성이 재설정되는 버그가 수정되었습니다.

## 알려진 문제:

**핵심 Substance 플러그 인**

* iOS용으로 빌드하려면 사용자가 Xcode의 빌드 설정 메뉴에서 &#39;Bitcode 사용&#39;을 비활성화해야 합니다.
* Substance은 에셋 번들에서 작동하지 않습니다.
* 다시 가져오기 후 에셋 브라우저의 Substance 미리보기 아이콘이 모두 Substance 아이콘으로 변경됩니다

**스크립팅**

* 프로젝트가 빌드 설정에서 x86으로 설정되어 있으면 스크립팅이 런타임에 작동하지 않습니다
* 특정 빌드 플랫폼에서 il2cpp 스크립팅 백엔드를 사용하는 문제

**Substance Painter 라이브 링크**

* Substance 라이브 링크로 페인팅한 후 프로젝트를 빌드하면 페인팅된 메쉬가 다시 기본 재질로 설정됩니다
* AO 채널이 Painter 라이브 링크와 함께 전송되지 않음
* 여러 재질이 있는 메시는 Unity Live Link에서 작동하지 않습니다
* Unity LiveLink가 SimpleJson을 사용하는 방식은 프로젝트에서 SimpleJson의 다른 인스턴스와 충돌합니다
