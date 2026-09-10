---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-1.html"
breadcrumb-title: ''
description: 3ds Max 플러그인 버전 2.3.1의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 3ds Max 2.3.1

2020년 2월 13일에 릴리스됨

이제 플러그인은 3ds Max 디렉터리의 외부에 C:\ProgramData\Autodesk\ApplicationPlugins\SubstanceIn3dsMax으로 설치됩니다. 이제 3ds Max에서 플러그인을 찾으라고 할 때 아무 곳에서나 작동하므로 네트워크 드라이브 등에 설치된 상태에서 작동합니다.\
애플리케이션 플러그인으로 전환하고 설치 디렉토리를 변경하면 2.1.1 이전 버전에서의 업그레이드가 제대로 작동하지 않습니다. 3ds Max 2018 및 2019의 경우 수동으로 제거해야 합니다. 2.2.0 버전은 올바르게 업그레이드되어야 합니다.\
이 릴리스에서 다루지 않은 일부 문제의 경우 이러한 문제와 발생할 수 있는 기타 문제를 곧 수정할 예정입니다.

이 버전은 현재 3ds Max 2018, 2019, 2020 및 2021용으로 출시되었습니다.

* 이제 sbsar 로드가 프로젝트 이미지 폴더를 먼저 찾습니다.
* 이제 VRay RT 및 VUE 파일 렌더러에 대해서만 렌더러 호환성 대화 상자가 나타납니다
* Slate Material Editor의 드래그하여 놓기 기능을 사용하여 Max 배치 관련 문제 제거
* 렌더링 대화 상자가 더 이상 3ds 최대 자동 모드로 표시되지 않음
* 더 작은 python 스크립트는 이제 Python 3과 호환됩니다.
* Substance Source 에셋을 3ds Max로 보내기 위한 Substance 시작 관리자에 대한 지원이 추가되었습니다. 시작 관리자를 변경해야 하지만 기능이 추가되면서 플러그인 지원이 함께 제공됩니다.
* 이제 Redshift 렌더러 스크립트에서 Redshift 2.6.24에 설정된 새 노드 이름을 사용합니다.
* Substance 2 SubstanceFilePath에 빈 충돌이 할당되면 Max가 더 이상 경로를 지정하지 않습니다.
* SubstanceOutput 유형의 이름 충돌을 이전 플러그인과 제거합니다.
* SubstanceOutput 클래스가 Substance2Output으로 이름이 변경되었습니다.
* Substance 메뉴 관리자 클래스가 Substance2MenuManager로 이름이 변경되었습니다.
* 이제 장면을 열면 매개 변수 블록 ID가 강제로 지워지며 장면 파일 간의 충돌이 제거됩니다. 장면 간에 전환할 때 로드 시 잘못된 매개 변수 블록이 있는 문제를 수정해야 합니다. 가져오기에는 더 복잡한 변경 사항이 필요하므로 여전히 문제가 있을 수 있습니다
* 이제 플러그인이 3ds Max 외부에 설치됩니다. 모든 패스가 로드 위치에서 기준으로 변경되었습니다.
* 이제 플러그인은 Autodesk Application 플러그인 시스템을 사용합니다.
