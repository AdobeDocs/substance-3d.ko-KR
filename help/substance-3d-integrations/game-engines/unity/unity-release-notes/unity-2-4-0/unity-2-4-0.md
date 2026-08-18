---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-0.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.4.0의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# 유니티 .

>[!WARNING]
>
> Unity에서 기본 빌드 아키텍처를 x86\_64 대신 x86으로 변경했습니다.\
> Substance을 참조하는 스크립트는 실행되지 않습니다. 다시 x86\_64로 변경해야 빌드가 작동합니다.

## 새로운 기능:

* HDRP 프로젝트 지원 추가됨(미리 보기)
* Substance 메뉴에 환경 설정 추가됨
* 기본 Substance 해상도 가져오기 설정을 설정하는 기능 추가
* 기본 [표준] 압축을 설정하는 기능 추가
* Substance 가져오기 시 모든 출력을 생성하는 기능 추가
* 사용자 정의 출력 + 동일한 사용량의 출력 지원
* 플랫폼 해상도 설정 추가됨
* IL2CPP 지원 버그 수정 추가됨

### 버그 수정:

* Mac OS에서 Substance Source을 열면 Linux 오류가 발생하는 버그가 수정되었습니다.
* 플랫폼 전환 시 소요되는 시간 단축. 이제 모바일 플랫폼에 대한 텍스처 변환은 대상 플랫폼을 전환할 때가 아니라 빌드할 때 수행됩니다.
* sbsar을 가져오는 동안 검증 실패 오류
* .NET 3.5를 사용하여 프로젝트를 업그레이드하면 Substance 재질이 손상됨
* Substance 소스가 OS X의 linux 대화 상자에서 지원되지 않음
* 그래프 이름 변경은 ForceText serialization 모드에서 구성 요소 및 장면 파일을 제거합니다.
* 동일한 사용을 사용하는 여러 출력이 있는 Substance 재질은 플러그인에서 sbsar의 사용자 정의 출력을 지원하지 않습니다

### 알려진 문제:

* 2017-2018/2019에서 프로젝트를 업그레이드할 때 사용자가 Substance 플러그인을 가져온 후 프로젝트를 업데이트하려면 Unity를 다시 시작해야 합니다.\
  해결 방법: 에셋/프로젝트 패키지를 만들고 2.4.0 플러그인을 사용하여 해당 패키지를 최신 프로젝트로 가져옵니다. Substance 파일을 올바르게 변환해야 합니다.
* Unity에서 기본 빌드 아키텍처를 x86으로 변경했습니다. 현재 Substance 플러그인은 x86\_64만 지원합니다.

**더 이상 완전히 지원되지 않음:**

* Substance 라이브 링크가 Asset Store 패키지에서 제거되었습니다. (패키지는 계속 Substance share에서 다운로드할 수 있습니다.)
