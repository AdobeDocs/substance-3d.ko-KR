---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-4.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.4.4의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# 유니티 .

2020년 2월 릴리스됨

* 추가: 2019.3에 대한 적절한 지원: Substance 플러그인 스크립팅 가능 개체를 깬 Unity API 변경 사항을 수정했습니다. 2019.3 API 업데이트로 작업할 수 있도록 재작업한 개체입니다. 수정 - 사용자 정의 재질을 사용하면 기존 재생에서 재질이 검은색으로 변합니다.
* 수정 - 스크립트에서 Duplicate() 함수를 사용한 다음 재생을 시작하고 종료할 때 충돌이 발생합니다.
* 고정 - 2019.3의 재질 타일링, 설정 및 셰이더 재설정
* Fixed - HDRP Material Shader가 매개 변수 변경 내용을 새로 고치지 않음
* 고정 - HDRP 마스크 맵이 업데이트되지 않음
* 고정 - 중복 함수에 대한 문자열 매개 변수 추가
* 수정 - 최신 Unity Stable에서 Linux 지원 수정
* 수정됨 - iOS에서 비트 코드를 비활성화해야 하는 경우의 주소 문제

알려진 문제:

* HDRP 에셋의 이름을 바꾸면 플러그인이 마스크 맵을 생성하지 않습니다.
* HDRP 프로젝트에서 Substance 플러그인을 사용할 때 Raw 압축을 사용하면 회색조 텍스처가 Alpha 8로 설정됩니다.
* GameObjects가 재생 모드에서 선택 해제됩니다.
* 재생 모드에서 Substance 그래프에 있는 &#39;Mip 맵 생성&#39;을 클릭하면 매개 변수가 무한대로 중단됩니다.
