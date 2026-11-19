---
description: Maya 플러그인 버전 3.0.0 이상용 릴리스 노트를 검토하여 새로운 기능, 개선 사항, 버그 수정에 대해 알아보십시오.
title: Maya 3.0.0
source-git-commit: 6453364f7dafa75c5bb2531a8707257498953e23
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%
---

# Maya 3.1.0+

## Maya 3.1.1

**출시일:** 2026년 11월 18일

**호환 대상:** Maya 2025 이상

### 추가됨/업데이트됨

* Substance 엔진 업데이트(9.6.1.) 보안 수정 사항 포함
* Maya 2025, 2026 및 2027(Arnold 및 V-Ray)의 OpenPBR 지원

### 알려진 제한 사항

* 방출 가중치: emission_weight 매개변수는 OpenPBR 1.1 사양의 일부가 아니며 자동으로 연결되지 않습니다. 워크플로우를 적용한 후 자재에서 배출을 사용하는 경우 OpenPBR 노드에서 배출 가중치 값을 수동으로 설정합니다.
* OpenPBR - V-선 — 서브서피스 반지름 배율: OpenPBR - V-선 워크플로우를 사용하는 경우 subsurface_radius_scale은 0의 값을 반환할 수 있습니다. 이 경우 연결을 제거하고 V-Ray 노드에서 수동으로 값을 설정합니다.
* 렌더러 간 시각적 차이: Substance 3D Designer의 재질 미리 보기와 Arnold 또는 V-Ray의 렌더링된 결과 간의 일부 차이는 각 렌더러의 OpenPBR 사양 구현 과정에서 차이로 인해 발생하며, 구현이 수렴됨에 따라 향상됩니다.
* Substance 3D Painter 12.2.0에서 내보낸 SBSAR 파일. 또는 이전 버전은 OpenPBR 워크플로우를 사용할 때 올바르게 연결되지 않을 수 있습니다.

## Maya 3.1.0

**출시일:** 2026년 11월 18일

**호환 대상:** Maya 2024

### 추가됨/업데이트됨

* Substance 엔진 업데이트(9.6.1.) 보안 수정 사항 포함
