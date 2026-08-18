---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-2.html"
breadcrumb-title: ''
description: 3ds Max 플러그인 버전 2.3.2의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# 3ds Max 2.3.2

2020년 4월 8일 릴리스

오늘 2.3.2 버전의 플러그인을 릴리스했습니다. 이 플러그인은 대부분 2.3.1의 상단에 버그 수정 릴리스가 포함되어 있습니다.

2.3.2 릴리스:

* 7.2.9로 Substance 엔진 업데이트됨
* 3ds Max 2018, 2019 및 2020에서 Redshift/VRay 충돌 시 렌더링 문제 수정
* 디버그 어설션 오류가 더 이상 나타나지 않습니다.
* 이제 Substance2 노드에 iMultipleOutputChannelsWithValues에 대한 스크립팅 인터페이스가 올바르게 있습니다.
* 이제 메뉴의 Substance 소스 항목이 설치된 경우 Substance 시작 관리자에서 소스 탭으로 열립니다.
* Substance 재질은 이제 Corona 렌더러를 사용하여 작업할 때 올바르게 업데이트되어야 합니다
* Substance 출력을 VRay Next와 함께 사용할 때 더 이상 일시적으로 이미지로 대체되지 않습니다
* 렌더링 호환성 대화 상자가 자동 적용에서 제거되었습니다. 필요한 경우 설정 대화 상자에서 계속 사용할 수 있습니다
* 3ds Max 2021에서 Substance 재질이 적용되는 동안 fbx를 내보낼 때 발생할 수 있는 문제 수정

알려진 문제:

* 3ds Max 2018에서 Substance 재질이 오브젝트에 첨부된 fbx를 내보내면 fbxmax.dlu 플러그인에서 충돌이 발생합니다. 현재 Autodesk와 함께 수행할 수 있는 작업이 있는지 또는 fbx 통합의 이전 릴리스에 대한 제한인지 확인하고 있습니다. 이전 해결 방법이 불안정하여 제거되었습니다. 3ds Max 2019 이상에서는 이 문제가 발생하지 않습니다.

이 버전은 3ds Max 2018, 2019, 2020 및 2021용으로 출시되었습니다.
