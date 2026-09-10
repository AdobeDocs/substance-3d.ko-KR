---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-2-0.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 2.2.0의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.2.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# 유니티 .

## 2.2.0 릴리스 정보

**출시일: 2019년 1월 10일**

### 코어 플러그인:

* 업데이트된 Substance 엔진
* 향상된 코드 안정성
* **Unity 2018.3 지원**
* **.NET 4.x 지원**
* 2018.3년 Substance Source 지원
* Substance Source 착색 문제가 수정되었습니다.
* 이제 그래프와 해당 재질에 동일한 개체 이름이 포함됩니다
* Unity Pro 스킨 GUI 가독성 향상 추가
* 재질의 출력 할당에 대한 지원 추가
* sRGB 처리와 관련된 버그가 수정되었습니다.
* 사용자가 그래프의 모든 인스턴스를 삭제할 수 있는 버그를 수정했습니다.
* 런타임에 매개 변수를 변경하는 동안 Substance을 렌더링하려고 하면 한 번에 두 개만 렌더링될 수 있는 버그가 수정되었습니다.
* 이제 이전 Substance 파일이 포함된 패키지를 가져올 때 플러그인은 사용자에게 이전 Substance 데이터가 포함되어 있음을 알리고 Unity에서 패키지 파일을 가져오려고 할 때 해당 패키지 파일을 삭제합니다(따라서 손상된 파일이 있는 경우 사용자가 모든 항목을 수동으로 삭제할 필요가 없음)
* Substance 메뉴에 Substance 플러그인 관련 빌드 정보를 표시하는 &#39;정보&#39; 단추를 추가했습니다.
* Substance GUI에 마우스 오버 도구 설명을 추가하여 노출된 Substance 매개 변수 이름 표시
* Substance GUI에 탐색 버튼을 추가하여 Substance 그래프 및 자료에 연결
* [내용 브라우저]에 Substance 그래프/재질/텍스처에 대한 새 아이콘이 추가되었습니다.
* 콘텐츠 브라우저에서 Substance 축소판을 업데이트했습니다.
* Substance 재질 이름 앞면에서 .mat를 제거했습니다.
* Substance 그래프 및 재질의 이름을 변경하는 기능 추가
* Substance 그래프 해상도를 변경하면 해당 시점에 사용자가 강제로 변경을 적용하도록 하는 적용/되돌리기 팝업이 더 이상 표시되지 않습니다
* 사용자가 정의한 버그가 아니라 반사 프로세스에서 기본 Substance 해상도만 사용하는 버그가 수정되었습니다.
* Substance GUI에 색상 공간이 감마로 설정되어 있는지 사용자에게 알리는 마우스 오버 경고가 추가되었습니다
* Substance 그래프 인스턴스의 변경된 기능: 이제 Substance 그래프 GUI에서 생성된 각 인스턴스에 대한 메시지를 표시하지 않고 Substance에서 그래프 인스턴스를 생성할 수 있습니다.

### 스크립팅:

* 스크립트 지원을 위한 것이 아닌 일부 함수를 숨겼습니다.
* 스크립트를 통해 Substance 그래프 인스턴스를 복제하는 함수를 추가했습니다. Duplicate()
* C#을 통해 프로시저 입력 정보를 쿼리하기 위해 함수를 추가하고 &#39;InputProperties&#39; 요소의 배열을 반환합니다. GetInputProperties()
* 그래프에 입력이 있는지 확인하는 함수를 추가했지만 true/false를 반환합니다. HasInput(string inputName)
* visibleif 입력이 표시되는지 확인하는 함수를 추가함 true/false: IsInputVisible(string inputName)
* 렌더링 구성표가 다시 디자인되었습니다. 따라서 RenderSubstancesAsync()는 사용되지 않으며 graphName.RenderAsync()로 변경되었습니다

## 알려진 문제:

**핵심 Substance 플러그 인**

* iOS용으로 빌드하려면 사용자가 Xcode의 빌드 설정 메뉴에서 &#39;Bitcode 사용&#39;을 비활성화해야 합니다.
* 빌드 대상이 Android/iOS으로 설정된 경우 콘텐츠 브라우저에서 Substance 개체 미리 보기가 검정으로 표시됩니다.
* Substance 플러그인을 가져온 후 Alpha 버튼이 아닌 텍스처 GUI에서 Substance 버튼과 Mip 맵 미리보기 슬라이더가 누락됩니다
* 사용자는 스크립트를 통해 Substance 그래프 해상도를 정의하기 위해 2의 제곱을 사용해야 합니다
* Unity 패키지를 사용하여 내보내기/가져올 때 Substance 재질이 지속되지 않음
* Substance은 에셋 번들에서 작동하지 않습니다.
* 다시 가져오기 후 에셋 브라우저의 Substance 미리보기 아이콘이 모두 Substance 아이콘으로 변경됩니다
* 장면에 재질이 있는 Substance 그래프의 이름을 바꾸면 해당 재질이 배치된 개체에서 제거됩니다
* (Mac만 해당) Mac에서 플러그인을 업데이트하면 장면의 프리파브에서 Substance 재질이 제거됩니다.|

**스크립팅**

* 프로젝트가 빌드 설정에서 x86으로 설정되어 있으면 스크립팅이 런타임에 작동하지 않습니다
* 특정 빌드 플랫폼에서 il2cpp 스크립팅 백엔드를 사용하는 문제

**Substance Painter 라이브 링크**

* Substance 라이브 링크로 페인팅한 후 프로젝트를 빌드하면 페인팅된 메쉬가 다시 기본 재질로 설정됩니다
* AO 채널이 Painter 라이브 링크와 함께 전송되지 않음
* 여러 재질이 있는 메시는 Unity Live Link에서 작동하지 않습니다
* Unity LiveLink가 SimpleJson을 사용하는 방식은 프로젝트에서 SimpleJson의 다른 인스턴스와 충돌합니다
