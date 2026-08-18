---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-6-0.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.6.0의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.6.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# 유니티 .

2021년 6월 7일에 릴리스됨

업데이트/추가됨:

* Substance Source 액세스를 위한 새로운 워크플로우! 이제 Substance Source 액션이 Substance 시작 관리자 내의 소스 탭에 액세스하여 에셋을 Unity로 직접 보낼 수 있습니다.
* 플러그인 버전 정보를 클립보드에 복사할 수 있습니다.
* 대상 설정에서 &quot;로드 시 생성&quot;이 제거됨

수정:

* HDRP 프로젝트에서 재질 설정이 변경되면 변위 모드가 기본값(테스트)으로 되돌아갑니다
* 해상도 크기가 검사기 창에 표시되지 않음
* Unity 버전 2020.2 이상에 플러그인을 설치할 수 없음

알려진 문제:

* 이전 버전 2.5.4 이하에서 플러그인을 업데이트할 때 액세스 거부 오류 및/또는 충돌이 발생합니다
  * 해결 방법: 플러그인 버전 2.6.0을 설치하기 전에 Unity 프로젝트 버전 2020.2 이상에서 이전 플러그인 버전 2.5.4 이하를 제거해야 합니다
* Substance 플러그인이 설치되면 이미지 파일의 텍스처 미리 보기가 검사기에 표시되지 않습니다
  * 이 문제의 출처는 Unity에 있으며 2021.2 버전(현재 Beta 버전) 내에서 Unity에 의해 수정될 예정입니다
