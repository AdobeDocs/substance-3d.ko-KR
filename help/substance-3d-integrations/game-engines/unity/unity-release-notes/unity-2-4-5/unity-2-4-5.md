---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-5.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.4.5의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# 유니티 .

2020년 4월 6일에 릴리스됨

* 추가됨: 2019.3 API를 사용한 HDRP 에셋 확인
* 추가됨: Substance 엔진 7.2 업데이트 - 소스의 일부 Substance 재질이 작동하지 않음 수정
* 추가됨: CPU 해상도에 맞게 대상 설정 업데이트
* 추가됨: CPU 엔진 최대 해상도 설정(4k 또는 2k 설정)
* 추가됨: HDRP 프로젝트 내에서 비-HDRP Substance 변환
* 수정: 대량의 Substance을 가져올 때 충돌이 발생합니다
* 수정: Substance 매개 변수를 변경한 후 재생 모드에서 다시 가져오기를 클릭할 때 예외가 발생했습니다.
* 수정: 기본값을 4K로 설정하기 위한 사용자 환경 설정의 출력(텍스처) 해상도 확인(CPU 엔진을 2K로 닫는 API)
* 수정: 재생 모드에서 Substance 그래프에 있는 &#39;Mip 맵 생성&#39;을 클릭한 다음 매개 변수를 변경하면 무한 중단됩니다.
* 수정: HDRP 프로젝트에서 Substance 플러그인을 사용할 때 Raw 압축 세트를 사용하면 greyscale 텍스처가 Alpha 8로 설정됩니다.
* 수정: 재생 모드에서 GameObject 선택 해제됨
* 고정: 거칠기 맵이 매개 변수 변경으로 업데이트되지 않음
* 수정: HDRP의 일부 Substance 파일에 대해 마스크 출력이 올바르게 생성되지 않습니다.
* 수정: 두 옵션 간에 압축된 알파 맵 드롭다운을 전환할 때 충돌이 발생합니다
* 수정: Substance 재질에서 다른 쪽을 클릭하면 GPU 인스턴스 확인란이 되돌아갑니다.
* 수정: Duplicate() 함수를 사용할 때 복제된 Substance 그래프에 Smoothness이 금속의 알파에 제대로 채워지지 않습니다.
* 수정: 빌드 대상을 Android로 전환하면 텍스처를 수동으로 다시 가져올 때까지 잘못된 형식이 됩니다.
* 수정: Unity에서 Substance 파일을 삭제하면 NullReferenceException이 발생합니다.
* 수정: 이전 버전에 대해 Unity 2019.3 HDRP API를 사용하지 않도록 설정

알려진 문제:

* 에미션 확인란은 기본적으로 활성화되어 있지 않으며, Substance 가져오기 시 HDR 값은 검정으로 설정됩니다.
* 표준 Substance 재질이 있는 패키지의 재질 속성은 가져올 때 전달되지 않습니다.
* 2017-2019/2020에서의 업데이트가 HDRP에서 작동하지 않음
* 대상 설정에서 4096을 선택한 상태에서(적용을 클릭하지 않고) 설정 메뉴에서 2048 클램프 옵션을 클릭하면 콘솔 로그에 오류가 발생합니다
