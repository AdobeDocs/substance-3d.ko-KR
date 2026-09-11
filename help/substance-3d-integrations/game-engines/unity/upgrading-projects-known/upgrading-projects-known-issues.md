---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/upgrading-projects-known-issues.html"
breadcrumb-title: ''
description: 마이그레이션 중에 방지할 Substance 자료 및 알려진 문제로 Unity 프로젝트를 업그레이드하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Upgrading ProjectsKnown Issues
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 프로젝트 업그레이드알려진 문제
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# 프로젝트 업그레이드/알려진 문제

>[!WARNING]
>
> Unity 3.0.0용 Substance 3D 플러그인은 이전 버전과의 호환성을 지원하지 않습니다. 따라서 Unity 2020.3.27x 이상을 사용해야 합니다.
> 
> Unity에서 기본 빌드 아키텍처를 x86\_64 대신 x86으로 변경했습니다.\
> Substance을 참조하는 스크립트는 실행되지 않습니다. 다시 x86\_64로 변경해야 빌드가 작동합니다.

## 알려진 문제

* 패널 폴더를 탐색하는 동안 &quot;*식에서 어설션이 실패했습니다.&quot; 오류가 발생했습니다.*
  * 일반적으로 축소판 그림 변경과 같이 UI가 변경되면 무해한 메시지가 표시되어야 하는 경우 Unity 측에서 발생하는 오류입니다.
* *이미지 입력이 8비트로 잠겨 있습니다.*
  * 이 문제는 버전 3.8.0-3에서 수정되었습니다. 올바른 워크플로우는 사용자가 텍스처에 대한 Unity의 기본 형식을 RGBA64로 변경하는 것입니다. 플러그인은 해당 정보를 Substance 엔진에 올바르게 전송하는 것을 처리합니다.
