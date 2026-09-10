---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-7-0.html"
breadcrumb-title: ''
description: 3ds Max 플러그인 버전 2.7.0의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# 3ds Max 2.7.0

<b>추가/업데이트:</b>

* 3ds Max 플러그인에서 Substance 엔진을 버전 9로 업그레이드하여 성능과 호환성을 개선했습니다.

<b>고정:</b>

* 3ds Max 버전 2019, 2022, 2023 및 2024에서 Substance 2 노드를 Slate Material Editor로 드래그하여 프로그램이 충돌 되는 충돌 문제를 해결했습니다. 이제 Substance 2 노드를 슬레이트 재료 편집기로 안전하게 드래그하여 놓을 수 있습니다.
* 3ds Max용 Substance 플러그인에서 &#39;Arnold에 Substance&#39; 및 기타 작업 과정을 선택해도 재료 슬레이트 편집기에서 관련 노드가 생성되지 않고 컴파일 오류가 있는 Maxscript를 잘못 열었던 문제를 해결했습니다. 이제 Arnold와 같은 워크플로우의 노드가 올바르게 생성되고 자동으로 연결됩니다.
* Substance 3D Sampler에서 시작 에셋/사전 설정(.sbsar - Substance2 텍스처 맵)을 내보내고 3ds Max 내에서 Corona 렌더러(버전 6 ~ 9hf1)로 변환하면 재료가 손상되어 검정 기본 색상과 깨진 범프 표준으로 렌더링되는 문제를 해결했습니다. 또한 이 업데이트는 Vray로의 변환에도 영향을 미치는 문제인 재질에 있는 Substance 속성 탭의 액세스 가능성을 해결합니다.
* 3ds Max 플러그인에서 Corona Material에 Substance2 텍스처의 입력을 플러깅하거나 뽑으면 충돌이 발생하는 문제를 수정했습니다.
* MaxScript 파일 내에 포함되거나 호출된 Python 스크립트가 기본적으로 허용되지 않는 3ds Max 2024의 호환성 문제를 해결했습니다
* 3Ds Max 플러그인에서 Corona 플러그인으로 Substance을 가져오고 실행하면 셰이더 미리 보기 및 렌더링에서 재질이 검은색으로 빛나고 빛나게 표시되는 문제를 해결했습니다. 이제 이 문제가 성공적으로 해결되어 코로나 렌더러를 사용한 Substance 맵이 올바르게 표시 및 렌더링되는지 확인할 수 있습니다.

이 버전은 3ds Max 2021, 2022 및 2023용으로 출시되었습니다.
