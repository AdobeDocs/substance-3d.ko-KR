---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-1.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.5.1의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# 유니티 .

2020년 5월 21일에 릴리스됨

추가됨

* 범용 렌더링 파이프라인 지원: Substance 텍스처는 자동으로 URP 셰이더와 재질을 사용합니다.

고정

* Substance CPU 엔진 최대 해상도 설정:
  * Substance 설정 메뉴의 필드 이름을 &quot;텍스처 클램프 \*\*&quot;에서 &quot;Substance CPU 엔진 최대 해상도&quot;로 업데이트했습니다.
  * 설정이 변경되면 모든 Substance 재질을 다시 가져온다는 경고 알림이 표시됩니다
* 설치 시 표시되는 불필요한 디버그 메시지를 제거했습니다(&quot;TextureClamp = 4096 Unity.Engine.Debug:Log(개체)&quot;).
* HDRP 프로젝트: Substance이 포함된 패키지를 가져올 때 표준 및 HDRP 재질 모두에 있는 재질 속성이 전달됩니다
* 반사 및 HDRP 마스크는 이전 Unity 버전에 있던 Substance 패키지의 Substance 재질을 가져올 때 예상대로 만들고 작동합니다
* 복제된 Substance 재질은 의도된 색상이 되며 복제 기능을 사용할 때 더 이상 노란색이 아닙니다
* Unity를 닫고 다시 열면 Substance 소스가 예상대로 로드됩니다.
* 패키지를 HDRP 프로젝트로 가져올 때 충돌 발생(간헐적)
* 슬라이더는 Substance 편집기가 색상(회색 음영)으로 설정된 노출 매개 변수가 있는 편집기 재질에 대해 예상대로 작동합니다
* 기본 해상도가 없는 Substance 그래프로 [사전 설정을 기본값으로 재설정]을 클릭하면 충돌이 발생함
* 출력 크기 매개 변수가 노출되지 않은 경우 Substance 재질의 출력 크기를 변경할 때 충돌이 발생합니다
* iOS 구축에 실패하지 않음
* Substance 재질을 사용하는 스크립트는 Windows 독립 실행형용으로 빌드할 때 실행됩니다
