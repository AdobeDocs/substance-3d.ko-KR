---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/modo/parameters.html"
breadcrumb-title: ''
description: MODO에서 Substance 속성 패널을 통해 Substance 재질 매개변수를 수정하여 재질을 사용자 정의합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 매개변수
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# 매개변수

Substance은 일련의 핵심 매개 변수를 가집니다. 이러한 매개 변수는 Substance, 출력 및 수정으로 구분됩니다. 이러한 속성은 [Substance 속성] 패널에서 찾을 수 있습니다.\
Substance Source Substance에 기술 매개 변수 및 채널이 포함됩니다. [채널] 옵션은 MODO에서 영향을 주지 않습니다. 출력은 [출력] 섹션을 사용하여 활성화/비활성화됩니다.

![](../../../assets/parameters-4.png){width="300px"}

## Substance

Substance에 기본 매개 변수 집합이 있으며, [Substance 속성] 패널의 [Substance] 범주에서 확인할 수 있습니다.

* **Substance 다시 로드:** 이 매개 변수를 사용하면 Substance을 다시 로드할 수 있습니다. 이는 Substance Designer과 함께 사용하도록 설계되었습니다. 사용자 정의 Substance에서 작업 중이고 새 조정 또는 출력을 추가한 경우 새로 게시된 Substance을 다시 MODO로 다시 로드할 수 있습니다. 새 조정 및 출력이 추가되고 이전 조정 설정이 유지됩니다.
* **음영 모드:** 이 매개 변수를 사용하면 Substance에 사용할 음영 모드를 설정할 수 있습니다. Principled (기본값), Unreal, Unity 또는 glTF.
* **Substance 재설정:** 이 매개 변수는 비틀기를 기본 설정으로 재설정합니다.
* **그래프 선택:** Substance 파일에서 재질을 만들 그래프를 선택할 수 있습니다.
* **사전 설정 불러오기:** Substance 조정 매개 변수를 구성하는 사전 설정을 불러올 수 있습니다. 사전 설정은 Substance Player을 사용하여 만들 수 있습니다. 사전 설정 파일은 .sbsprs 파일 유형입니다. 사전 설정을 로드했으면 사전 설정 드롭다운을 클릭하고 사전 설정을 선택해야 합니다. .sbspr에 여러 사전 설정이 포함될 수 있기 때문입니다.
* **사전 설정 저장:** 사전 설정을 저장할 수 있습니다.
* **사전 설정 선택:** Substance 파일에 포함된 사전 설정을 선택하거나 MODO 내에 저장된 사전 설정에서 선택할 수 있습니다.
* **디스크로 굽기:** 이 매개 변수는 Substance에서 생성된 텍스처를 비트맵 파일로 굽습니다.
* **출력 크기:** 이 매개 변수는 텍스처의 크기를 설정된 크기로 동적으로 조정합니다. Substance 엔진이 텍스처를 원하는 크기로 재생성합니다.
* **임의 시드:** 이 매개 변수는 Substance의 프로시저 생성을 변경합니다. 이 매개 변수는 동일한 Substance의 임의 버전을 만드는 데 유용합니다. 이를 통해 Substance 매개 변수를 빠르게 변경하여 새로운 버전의 텍스처를 생성할 수 있습니다

## 출력

[출력] 옵션을 사용하여 Substance 출력을 활성화하거나 비활성화할 수 있습니다. 출력은 Substance 엔진에서 생성되고 셰이더 트리에서 텍스처로 렌더링되는 출력입니다.

![](../../../assets/outputs-02.png){width="300px"}

## 트위크스

트위크는 Substance 파일에서 작성되고 MODO에서 편집할 수 있는 매개 변수입니다. 채널을 선택할 수 있으며 항목 모드에서 Channel Haul을 사용하여 팝업 컨트롤러에서 컨트롤을 함께 가져올 수 있습니다.

![](../../../assets/haul.png){width="300px"}
