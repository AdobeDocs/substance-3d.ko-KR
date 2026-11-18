---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/maya/substance-in-maya-overview.html"
breadcrumb-title: ""
description: Maya용 Substance 플러그인과 작업 과정에서 Substance 재질을 가져오고 사용하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance in Maya Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya Substance 개요
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%
---

# Maya Substance 개요

## 플러그인 개요

Maya 플러그인용 Substance을 사용하면 Maya에서 기존의 모든 Substance 3D 재질(.SBSAR 파일)을 직접 로드할 수 있습니다. Substance 3D 재질은 Substance 3D Designer 또는 Substance 3D Sampler에서 SBSAR 파일로 작성 및 내보내고, Substance 3D Assets 라이브러리와 같은 기존 라이브러리에서 다운로드할 수 있습니다. Maya 플러그인용 Substance은 Maya 재질을 만들고 출력 텍스처를 올바른 재질 채널 입력으로 보냅니다

>[!NOTE]
>
> [설정/환경 설정] ->Maya 플러그인 관리자에 플러그인이 로드되어 있는지 확인합니다

## Hypershade 노드 편집기에서 SBSAR 파일 열기

1. **Hypershade**&#x200B;을(를) 열고 **노드 편집기**&#x200B;에서 마우스 오른쪽 단추를 클릭한 후 표시 메뉴에서 위로 밀어 **노드 만들기**&#x200B;를 선택합니다. **노드 만들기 창**&#x200B;에서 **Substance 노드**&#x200B;를 검색하여 선택합니다.

   ![](../../../assets/createnode.png)

   Hypershade에서 **Substance 노드**&#x200B;를 클릭하여 선택합니다. 그러면 폴더 아이콘을 클릭하여 Substance 3D 재질(SBSAR 파일)을 로드할 수 있는 **재질 편집기**&#x200B;가 열립니다.

1. 또는 SBSAR 파일을 Maya의 **Hypershade Editor**&#x200B;로 끌어 놓고 자동으로 생성된 Substance 노드를 클릭하여 **재질 편집기**&#x200B;에서 옵션을 직접 보고 편집할 수 있습니다.

### 속성 편집기에서 SBSAR 매개 변수로 재생

![](../../../assets/1.png)

1. Substance에 여러 그래프가 포함되어 있으면 **선택한 그래프 드롭다운**&#x200B;이 채워집니다. 재질을 만드는 데 사용할 그래프를 선택합니다.

1. **그래프 정보 단추**&#x200B;는 Substance Designer으로 설정된 그래프 특성을 표시합니다.

1. **너비** 및 **Height** 값을 설정하여 해상도를 설정합니다. **비율 잠금**&#x200B;을 사용하지 않도록 설정하여 정사각형이 아닌 비율을 선택합니다.

1. 아놀드와 같은 렌더러에서 사용할 수 있도록 Substance 출력을 디스크로 구우려면 **출력을 디스크로 캐시**&#x200B;를 사용하도록 설정하십시오. 캐시된 파일은 Maya 파일 노드를 사용하여 플러그인에서 다시 읽습니다.

   ![](../../../assets/outputsettings.png)

1. 사용 중인 렌더러의 워크플로를 선택하고 **셰이더 네트워크 만들기 단추**&#x200B;를 클릭합니다. 렌더러 워크플로에 대해 셰이더 네트워크가 만들어집니다. 버전 3.1.1의 경우 워크플로 목록에서는 OpenPBR 셰이더 네트워크를 만드는 옵션도 제공합니다. 셰이더 네트워크가 생성되면 장면에 재질을 적용할 수 있습니다.

   ![](../../../assets/createnetwork.gif){width="1000px"}

## 문제 해결

버그를 보고하려면 [Substance 디스코드 서버](https://discord.com/invite/substance3d)에서 #maya-plugin 채널에 가입하거나 [Adobe 커뮤니티](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax)를 방문하세요. 콘솔 로그의 관련 정보와 모든 재생 단계를 포함하면 문제를 보다 효율적으로 진단하는 데 도움이 됩니다.