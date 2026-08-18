---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/cinema-4d/attribute-manager.html"
breadcrumb-title: ''
description: Cinema 4D의 특성 관리자를 사용하여 Substance 에셋 속성과 재질 설정을 구성합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Attribute Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 속성 관리자
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# 속성 관리자

Cinema 4D의 속성 관리자에는 Substance 에셋에 대한 새로운 모드가 있습니다.

Substance 에셋 관리자에서 Substance을 선택하면 속성 관리자가 자동으로 Substance 에셋 모드로 전환됩니다. 속성 관리자의 모드 메뉴에서 이 모드로 수동으로 전환할 수도 있습니다.

Substance 에셋 모드에서는 Substance의 모든 입력에 액세스할 수 있으며 모든 출력 채널에 대한 개요도 사용할 수 있습니다.

![](../../../assets/cinema-4d-9.png){width="500px"}

## Substance 입력 그룹화

Substance 입력을 그룹화하면 이러한 그룹이 속성 관리자에 표시됩니다. 미리 정의된 두 개의 그룹이 있습니다. **기본 속성** 및 **이미지 입력**.

* 기본 Substance Designer 그룹에는 속성의 그룹에 할당되지 않은 모든 입력이 표시됩니다.
* 이름에서 알 수 있듯이, 외부 이미지에 연결된 모든 Substance 입력은 [이미지 입력] 그룹에 수집됩니다.

## 파일 이름 매개 변수

Attribute Manager 의 Filename 매개 변수를 사용하면 Substance 에셋을 장면에 로드한 후 해당 에셋의 파일 위치를 변경할 수 있습니다.

![](../../../assets/cinema-4d-10.png){width="500px"}

이 기능은 Substance 파일을 재배치할 때뿐만 아니라 전혀 다른 Substance과 교환할 때도 유용합니다.

이 경우 이전 Substance 출력 채널에 대한 기존 참조를 새 Substance에 다시 매핑할지 여부를 사용자에게 묻습니다.

![](../../../assets/cinema-4d-11.png){width="500px"}

질문에 &#39;아니요&#39;로 대답하면 이전 Substance에 대한 링크가 모든 Substance 셰이더에서 삭제됩니다. 출력 채널을 다시 매핑하기 위해 플러그인은 먼저 동일한 유형의 출력 채널을 검색한 다음 동일한 이름을 사용합니다.

## 매개 변수 Tri-state

여러 Substance을 동시에 선택하면 이러한 Substance 간에 공유된 입력은 세 상태로 표시되며 Cinema 4D의 다른 모든 매개변수와 마찬가지로 선택한 모든 Substance에 대해 동시에 편집할 수 있습니다.

이러한 경우 출력 채널은 아래와 같이 표시됩니다.

![](../../../assets/cinema-4d-12.png){width="300px"}
