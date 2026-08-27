---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-1.html"
breadcrumb-title: ''
description: Blender 추가 기능 버전 0.9.1의 릴리스 노트를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 0.9.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 추가 기능 0.9.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# 추가 기능 0.9.1

**추가 기능 버전 0.91에 대한 릴리스 정보+**

* 참고: *플러그인 버전 0.91+은(는) 이전 버전의 플러그인과 호환되지 않습니다.*
* 플러그인의 성능과 안정성을 개선하기 위해 내부 코드베이스의 재아키텍처
* 전반적인 사용자 환경을 개선하기 위해 개선된 UI
* 기본 타일링을 수정할 수 있는 UI를 추가함
* 순환 렌더링 보기에서 텍스처 업데이트 지원이 추가되었습니다.
* Substance 로드 실패 여부를 알리기 위해 콘솔에서 오류 처리가 추가됨
* 빠른 작업으로 유동 메뉴 업데이트됨

**환경 설정 섹션: 추가/업데이트:**

* 이미지 형식 내보내기 매개 변수. Blender에서 생성된 이미지를 Substance 재질의 이미지 입력으로 사용할 때 이 형식을 사용하여 해당 이미지를 시간 폴더에 저장합니다.
* Sbsar 라이브러리 경로; [불러오기] 단추를 사용하여 Substance 파일을 검색할 때 기본적으로 열리는 폴더를 지정합니다.
* Substance 3d Painter에서 저장하지 않은 파일 내보내기를 처리하는 데 사용하는 경로를 에뮬레이션하는 기본 텍스처 내보내기 경로(시간 폴더)
* $matName과 같은 키를 사용하여 하위 폴더를 만드는 옵션을 사용하여 위와 동일한 상대 경로 텍스처
* Sbsar 파일 프로젝트를 저장할 때 혼합 파일에 사용된 sbsar 파일을 패키지하는 하위 폴더 만들기의 상대 경로
* 환경 설정에서 다른 셰이더 네트워크를 동적으로 설정하는 기능 - 셰이더 네트워크에서 셰이더 요구 사항에 따라 셰이더마다 다른 변수를 설정하는 기능
* 셰이더 네트워크의 출력 섹션에서 출력이 기본적으로 활성화되어 있는지 여부를 설정할 수 있습니다
* 색상 공간 설정 기능(srgb뿐만 아니라 ACES, 선형 exr 및 블렌더 필터 워크플로우를 지원함)
* 이미지 형식 및 비트 심도의 기본 선택
* 셰이더에 정의되어 있지 않은 출력 사용에 대한 값을 설정하는 제네릭 출력입니다. 예를 들어 마스크와 같이 셰이더에 의해 기본적으로 사용되지 않는 다른 출력이 있는 경우입니다.
* 출력 유형을 변경하는 필터입니다(활성화된 출력만 1개, 셰이더와 Substance에 있는 모든 출력 2개, Substance에서 사용할 수 있는 모든 출력 3개).
* 사용자 정의 단축키 지원(편집됨)

**Substance 3D 패널 섹션: 추가/업데이트:**

* 타일링 및 해상도 매개변수 값을 조정하고 잠그는 기능
* 업데이트된 사전 설정 UI - 사용자에게 제공하고자 하는 그래프 유형을 변경하는 셰이더 유형 드롭다운
* 이미지 입력 매개 변수를 믹서에 사용된 표준 이미지 입력으로 변경했습니다. 이제 파일뿐만 아니라 블렌더 이미지도 사용할 수 있습니다
* 언제든지 여러 Blender 인스턴스에서 작업할 수 있습니다.
* 뷰포트에서 재질을 선택하면 Substance 3D 패널에서 재질이 자동으로 강조 표시되도록 지원
