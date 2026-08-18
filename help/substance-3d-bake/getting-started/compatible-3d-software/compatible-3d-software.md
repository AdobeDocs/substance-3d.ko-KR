---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Substance Baker와 호환되는 3D 소프트웨어를 알아보고 최적의 베이킹 결과를 위해 메시를 준비하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Compatible 3D software
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 호환되는 3D 소프트웨어
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---


# 호환되는 3D 소프트웨어

대부분의 3D 소프트웨어는 메시 형상을 애플리케이션에서 지원하는 파일 형식의 다각형으로 내보내는 한 Substance Baker와 호환됩니다.

그러나 이러한 메시를 내보낼 때 모든 소프트웨어가 기능과 품질에 있어 동등한 것은 아닙니다. 메시를 제대로 청소하고 베이커와 호환되도록 하는 것이 중요한 이유다. 망을 준비하는 방법에 대한 자세한 내용은 다양한 [안내선](../../guides/performances-and-opt/performances-and-optimizations.md)을 참조하세요.

## 소프트웨어 호환성

다음은 일반적으로 알려진 3D 소프트웨어 및 베이커와의 호환성 목록입니다.

| *이름* | *상태* |
| --- | --- |
| **블렌더** | 호환 가능: 내보내기 전에 수정자를 병합해야 합니다. |
| **마야** | 호환 가능: 내보내기 전에 변형 및 삭제 내역을 고정해야 합니다. |
| **3DS 최대** | 호환 가능: 내보내기 전에 xForm 재설정이 필요합니다. |
| **MODO** | 호환 가능: &quot;Unreal Static Mesh&quot;로 설정된 게임 탭 내보내기 도구를 사용하는 것이 좋습니다. |
| **Cinema 4D** | 호환 가능: 내보내기 전에 수정자를 병합해야 합니다. |
| **zBrush** | 호환되지 않음: 낮은 폴리 메시는 먼저 다른 3D 애플리케이션에서 처리 및 정리해야 합니다. 호환 가능: 베이킹용 하이 폴리 메쉬. |

## 파일 포맷

형상을 구울 때는 사용되는 파일 형식도 고려해야 합니다. 파일 포맷은 메쉬에 저장될 정보의 양을 정의합니다.

너무 많은 정보를 가지고 있는 것은 때로는 해로울 수 있고 오류를 초래할 수 있습니다. 일반적으로 문제를 해결하고 범인이 베이커 자체에 있는지 또는 3D 소프트웨어에서 왔는지 확인하는 쉬운 방법이 될 수 있으므로 오류가 발생할 때 다른 파일 형식을 사용하는 것이 좋습니다.

Bellow는 베이커가 지원하는 가장 일반적인 두 가지 파일 형식에 대한 간략한 개요입니다.

| 파일 포맷 | 정보 |
| --- | --- |
| **FBX** | Autodesk FBX (Filmbox)는 Autodesk Software에서 사용하는 기본 파일 형식이며 텍스트 또는 바이너리로 작성할 수 있습니다.  다음을 지원합니다.<ul data-preserve-html="true"><li data-preserve-html="true">UV(복수 세트)</li><li data-preserve-html="true">꼭지점, 탄젠트 및 이항</li><li data-preserve-html="true">꼭지점 색상</li><li data-preserve-html="true">삼각형 얼굴, 사각형 얼굴 및 N-Gon 얼굴</li><li data-preserve-html="true">카메라</li><li data-preserve-html="true">조명</li><li data-preserve-html="true">메쉬 세분</li><li data-preserve-html="true">그룹 다듬기</li><li data-preserve-html="true">재질 정보(예: 색상)</li><li data-preserve-html="true">비트맵</li></ul> |
| **OBJ** | Wavefront OBJ는 를 지원하는 매우 간단한 텍스트 기반 파일 형식입니다.<ul data-preserve-html="true"><li data-preserve-html="true">UV(한 세트만)</li><li data-preserve-html="true">꼭지점 수직</li><li data-preserve-html="true">꼭지점 색상(Pixologic zBrush에서 내보낸 경우에만)</li><li data-preserve-html="true">삼각형 얼굴, 사각형 얼굴 및 N-Gon 얼굴</li><li data-preserve-html="true">재질 색상(<strong>mtl</strong> 파일이 있는 경우)</li></ul> |
