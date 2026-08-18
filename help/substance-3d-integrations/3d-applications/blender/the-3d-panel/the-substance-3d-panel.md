---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/blender/the-substance-3d-panel.html"
breadcrumb-title: ''
description: Blender에서 Substance 3D 패널을 사용하여 재질, 매개 변수 및 출력을 관리하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > The Substance 3D Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D 패널
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---


# Substance 3D 패널

![](../../../assets/blender-substance3dpanel.png)

## 패널 컨트롤

**만들기** - 파일 브라우저를 열어 Substance 3D 재질을 선택합니다. 기본적으로 .sbsar 파일에서 생성된 텍스처를 사용하여 블렌더 재질을 만듭니다.

**적용** - 선택한 Substance 3D 재질을 선택한 개체에 새 재질 슬롯에 연결합니다. 이 경우 객체에 대한 이전 재료 지정이 무시되지 않습니다.

**Substance 3D 커뮤니티 에셋** - 웹 브라우저에서 Substance 3D 커뮤니티 에셋 페이지를 엽니다.

**Substance 3D Assets** - 웹 브라우저에서 Substance 3D Assets 원본 페이지를 엽니다.

**선택한 Substance 3D 재질 복제** - 선택한 Substance 3D 재질의 새 인스턴스를 로드합니다. 동일한 Substance 재료의 상이한 인스턴스들의 파라미터들은 서로 독립적으로 조정될 수 있다.

**새로 고침** - Substance 3D 재질을 다시 로드합니다.

>[!WARNING]
>
> **경고:**
> 
> 새로 고침 단추를 사용하면 셰이더 그래프에 대한 사용자 변경 내용을 실행 취소합니다. 새로 고치기 전에 사용자가 추가한 노드를 복사하여 새로 고침 후 그래프에 붙여넣습니다.

**제거** - 선택한 Substance 3D 재질을 패널에서 제거합니다.

>[!NOTE]
>
> Substance 재질에서 만든 블렌더 재질은 프로젝트에 남아 있습니다. 개체에서 수동으로 삭제하거나 제거할 수 있습니다.

**로드된 3D Substance 재질** - .blend 파일에 로드된 Substance 재질 목록을 표시합니다.

## 그래프 매개 변수

**출력 해상도** - [포함] 및 [Height] 해상도에 대한 드롭다운입니다. 이러한 값은 개별적으로 조정된 값에 연결 해제될 수 있습니다.

**임의화 및 임의화** - 임의화 단추는 임의값을 사용할 수 있는 매개 변수를 변경하기 위해 새 임의화 값을 생성합니다. 임의화는 수동으로 설정할 수도 있습니다.

## 사전 설정을 사용한 작업

SBSAR 파일이 사전 설정으로 게시될 수 있으며 [사전 설정] 드롭다운 상자에서 확인할 수 있습니다. 사용자 고유의 사전 설정을 만들려면 매개 변수를 원하는 대로 조정하고 **저장** 단추를 사용하십시오. 선택한 사전 설정을 .sbsprs 파일로 내보내거나 드롭다운 목록에서 선택한 사전 설정을 삭제하는 추가 옵션이 있습니다. **불러오기** 단추를 사용하여 .sbsprs 파일에서 사전 설정을 가져올 수 있습니다.

## Substance 매개 변수

Substance Designer에 노출된 매개 변수는 Substance 매개 변수 컨트롤을 사용하여 조정할 수 있습니다. 이러한 매개 변수는 Substance 재질 제작자가 설정하며 재질에 따라 다릅니다. 이러한 매개변수를 조정하면 생성된 텍스처가 [로드된 3D Substance 재질] 섹션의 재질 이름 옆에 있는 처리 아이콘으로 업데이트됩니다.

출력 텍스처의 파일 형식은 드롭다운을 통해 전환하고 변경할 수 있습니다.

자세한 내용은 Designer 문서 페이지에서 [매개 변수 노출](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter)을 참조하세요.

## 기술 매개 변수

Substance 자료에는 기술 매개변수 세트가 있을 수 있습니다. 색상 교정 및 기타 재질 조정을 위한 추가 컨트롤입니다.
