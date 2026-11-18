---
description: 3ds Max 플러그인 버전 3.0.0 이상의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
title: 3Ds Max 3.1.0+
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%
---

# 3ds Max 3.1.0+

## 3ds Max 3.1.1

**출시일:** 2026년 11월 18일

**호환 대상:** 3ds Max 2025 이상

### 추가됨/업데이트됨

* Substance 엔진 업데이트(9.6.1.) 보안 수정 사항 포함
* 3ds Max 2025, 2026 및 2027 OpenPBR 지원(Arnold 및 V-Ray)

### 알려진 제한 사항

* 방출 가중치: emission_weight 매개변수는 OpenPBR 1.1 사양의 일부가 아니며 자동으로 연결되지 않습니다. 워크플로우를 적용한 후 자재에서 배출을 사용하는 경우 OpenPBR 노드에서 배출 가중치 값을 수동으로 설정합니다.
* 렌더러 간 시각적 차이: Substance 3D Designer의 재질 미리 보기와 Arnold 또는 V-Ray의 렌더링된 결과 간의 일부 차이는 각 렌더러의 OpenPBR 사양 구현 과정에서 차이로 인해 발생하며, 구현이 수렴됨에 따라 향상됩니다.
* Substance 3D Painter 12.2.0에서 내보낸 SBSAR 파일. 또는 이전 버전은 OpenPBR 워크플로우를 사용할 때 올바르게 연결되지 않을 수 있습니다.

## 3ds Max 3.1.0

**출시일:** 2026년 11월 18일

**호환 제품:** 3ds Max 2024

### 추가됨/업데이트됨

* Substance 엔진 업데이트(9.6.1.) 보안 수정 사항 포함
