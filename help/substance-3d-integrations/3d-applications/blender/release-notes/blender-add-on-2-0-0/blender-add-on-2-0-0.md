---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/blender/release-notes/blender-add-on-2-0-0.html"
breadcrumb-title: ''
description: Blender 추가 기능 버전 2.0.0의 릴리스 노트를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 추가 기능 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# 추가 기능 2.0.0

Substance 3D Addon 2.0은 Blender 사용자를 위한 혁신적인 업데이트로, 완전히 리팩터링된 플러그인 아키텍처를 특징으로 합니다. 이 재설계는 원활한 통합, 향상된 성능 및 향후 확장을 위한 유연한 토대에 중점을 둡니다. 이는 단순한 업그레이드가 아니라 Blender 내에서 Substance 재질을 처리하는 방법을 재구성하여 3D 전문가의 진화하는 요구 사항을 충족합니다.

<b>버전 2.0의 주요 내용:</b>

* 리팩터링된 아키텍처 - 향상된 성능 및 통합을 위해 개선된 플러그인 구조
* 향후 확장 지원 - 이번 업데이트를 통해 향후 새로운 기능을 손쉽게 추가할 수 있는 토대가 마련되었습니다
* 폭넓은 호환성 - Mac 사용자 지원을 포함하여 Blender 버전 3.0 이상과 완전히 호환됩니다.

<b>추가/업데이트:</b>

* [SRE] Substance 엔진 선택 지원(기본값은 GPU)
* [SRE] 텍스처를 내보낼 새로운 이미지 형식
* [SRE] 각 맵 유형에 대한 비트 심도 선택
* [BLD] 값 출력 지원
* [BLD] 문자열 입력 지원
* [SRE] 이미지 내보내기 대상에 대한 기본 임시 폴더를 선택하는 옵션이 추가됨

<b>고정:</b>

* [SRE] 전반적인 성능 향상
* [BLD] 통합 도구와 블렌더 간의 통신 문제 수정
* [BLD] 통합 도구 설치/시작 실패
* [BLD] Blender를 닫을 때 통합 도구가 종료되지 않음
* [BLD] 맵의 파일 유형을 변경할 때 재질이 업데이트되지 않음
* [SRE] 재질의 모든 맵은 항상 내보내집니다
* [SRE] 통합 도구는 계단식 배열을 사용하여 일반 맵을 내보냅니다.
* [SRE] Substance 로드가 완료되지 않음
* [SRE] 물리적 크기 단위가 장면에 조정되지 않음
* [BLD] Blender에서 생성된 사전 설정이 다른 통합에서 작동하지 않음
* [BLD] 재질이 사이클에서 업데이트되지 않음
* [BLD] 입력의 소프트 및 하드 제한이 무시됩니다.
* [BLD] 매개 변수를 조정할 때 색상 강도가 올바르게 업데이트되지 않음
* [SRE] 통합 도구 제거 실패
* [SRE] 재료를 여러 번 복제할 때 오류가 발생하는 문제를 수정했습니다.
* [SRE] 이제 이미지 노드의 색상 공간이 사용자 기본 설정에 맞게 조정됩니다.

<b>알려진 문제:</b>

* Blender v4.0 이상을 사용하는 경우 여러 번 활성화 및 비활성화한 후 소켓이 순서대로 정렬되지 않음
* Cltr+Z로 변경 취소 시 오류 발생
* .sbsar 파일 대신 빈 파일이나 폴더를 로드하면 플러그인이 손상될 수 있습니다
* 블렌더 헤드리스 모드 지원
