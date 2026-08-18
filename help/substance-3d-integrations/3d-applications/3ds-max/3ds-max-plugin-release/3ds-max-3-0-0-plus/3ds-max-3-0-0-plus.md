---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-3-0-0-plus.html"
breadcrumb-title: ''
description: 3ds Max 플러그인 버전 3.0.0 이상의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3Ds Max 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 3ds Max 3.0.0+

## 3ds Max 3.0.4

<b>추가/업데이트:</b>

* Substance 플러그인 아이콘이 최신 아이콘으로 업데이트되었습니다.
* 플러그인에서 커넥터를 사용하여 사전 설정을 보내고 받을 수 있는 기능이 추가되었습니다.
* Notification 매개 변수에서 Core Interface의 사용을 대체하는 통합 메뉴 관리자

<b>고정:</b>

* 슬레이트 재질 편집기가 열려 있고 Substance2 텍스처 맵이 선택되어 있을 때 Substance 2 재질이 Corona를 사용하여 IR/프로덕션에서 렌더링되지 않을 수 있는 문제를 해결했습니다.
* Sampler Connector 업데이트에서 기존 노드를 업데이트하지 않고 새 Substance 2 노드를 만드는 문제를 해결했습니다.
* Substance2 노드를 추가할 때 3ds Max 플러그인에서 충돌 문제가 해결되었으며 일괄 가져오기를 사용하여 .sbsar 파일을 로드하면 더 이상 스크립트 편집기가 열리지 않습니다.
* .msi 설치 관리자를 사용할 때 호환되지 않는 .dll 파일로 인해 3DSMax 2025 플러그인을 로드하지 못했던 문제를 해결했습니다.

## 3ds Max 3.0.2

<b>추가/업데이트:</b>

* 모든 기존 아이콘을 qrc 및 rcc 파일에 통합하고, Autodesk가 선호하는 방법에 맞춰 정렬하고, SBSAR 그래프 패널에서 일관된 로딩을 보장하여 Substance 플러그인에서 아이콘 관리를 표준화했습니다.
* 창 크기를 조정할 때 입력 필드와 설명이 제대로 맞춰지도록 플러그인의 Substance 설정 창 응답성이 향상되었습니다.
* Substance 플러그인은 이제 Corona 11과 호환됩니다.

<b>고정:</b>

* V-Ray 재질에서 광택 색상과 광택 거칠기가 자동으로 연결되지 않는 문제를 해결했습니다. 이제 V-Ray와 Arnold에서 워크플로우를 만들 때 두 속성 모두 자동으로 연결됩니다.
* 저장된 값이 한 자리인 경우 CPU 코어 제한 설정을 조정하면 두 자리 값이 잘못 표시되는 플러그인의 UI 문제를 해결했습니다.
* Substance 호환성 기능과 관련된 3ds Max 플러그인 v3.0.0에 대한 콘솔의 렌더링 오류를 수정했습니다. 이제 [Substance 일괄 가져오기] 메뉴를 사용하여 만든 Substance 노드가 예상대로 렌더링됩니다.
