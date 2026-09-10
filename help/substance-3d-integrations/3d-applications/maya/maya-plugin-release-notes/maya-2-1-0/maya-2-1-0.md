---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-1-0.html"
breadcrumb-title: ''
description: Maya 플러그인 버전 2.1.0의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.1.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 마야 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# 마야 .

Maya 2.1.0의 Substance 변경 로그

* Python 3과의 호환성 보장
* Substance 엔진이 버전 7.2.9로 업데이트됨
* 워크플로우를 적용할 때 충돌하는 글로벌 멜 변수 이름이 있는 오류를 수정했습니다.
* 이제 Redshift 워크플로가 fresnel을 metalness로 설정
* 다른 Substance 프로그램 및 Substance 시작 프로그램과의 상호 운용성을 처리하는 새 플러그인 파일 subchancelink가 추가되었습니다.
* 지금 Substance Source을 열면 subchancelink 플러그인이 로드되는 경우 소스 탭에 대한 Substance 시작 관리자가 열립니다.
* Subancelink 플러그인을 사용하면 Launcher에서 UI가 추가될 때 Substance Source 재질을 Maya 통합에 보낼 수 있습니다.
* 스크립팅 명령을 추가하여 내부 라이브러리 버전을 가져오고 소스 페이지에 대한 Substance 시작 관리자 열기
* 웹 사이트 링크는 이제 [allegorithmic.com](http://allegorithmic.com) 대신 [substance3d.com](http://substance3d.com)에 열립니다.
* 문서 및 소스 링크는 웹 페이지를 열 때 사용자 설정 기본 브라우저를 엽니다.
* Windows에서 internet explorer가 더 이상 열리지 않음
* 셸프와 메뉴에 Substance share에 새 링크 추가
* Substance 링커 버전 및 해시를 쿼리하는 새 명령을 추가했습니다.
* Maya LT에서는 버전이 설정 메뉴에서 제거되었습니다
* About 메뉴는 더 이상 PySide2 및 Python에서 작성되지 않고 대신 Qt를 사용하는 네이티브 코드에서 작성됩니다. 이전에는 없었던 Maya LT에서 사용할 수 있습니다.
* 정보 메뉴에는 다른 진단 정보가 있습니다. 이제 소스 제어의 변경 사항과 일치하도록 git 해시를 표시합니다.
* 이제 클립보드에 대한 정보 메뉴 사본에 이 git 해시와 플러그인이 빌드된 Maya 버전이 포함됩니다.
* 이제 정보 창의 라이선스가 텍스트 파일로 열립니다.
* Maya 2017에 대한 지원 추가
* 워크플로 스크립트 생성기에서 더 이상 &#39;ordering&#39; 멤버에 대한 문자열을 출력하지 않습니다. 기존의 모든 워크플로우가 제대로 처리됩니다.

스크립팅 명령 추가됨:\
substancemaya:\
\* substanceUtilityGetLinkerVersion\
\* substanceUtilityGetLinkerHash\
\* substanceUiOpenAboutWindow\
\* substanceUiOpenSourceWebsite\
\* substanceUiOpenDocumentation\
\* substanceUiOpenShareWebsite

substancelink:\
\* substanceLinkGetLinkVersion\
\* substanceLinkGetPortalCliVersion\
\* substanceLinkOpenLauncher

이 버전은 Windows의 Maya 2017, 2018, 2019 및 2020용으로 출시되었습니다.\
Linux 및 Macos. 또한 Maya LT 2018, 2019 및 2020용으로 출시되었습니다\
Windows 및 MacOS.
