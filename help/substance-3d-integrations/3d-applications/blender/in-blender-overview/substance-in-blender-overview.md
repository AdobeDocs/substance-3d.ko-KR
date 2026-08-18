---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/blender/substance-in-blender-overview.html"
breadcrumb-title: ''
description: Blender용 Substance 3D 추가 기능과 프로젝트에서 Substance 재질을 가져오고 작업하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Substance in Blender Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 믹서의 Substance 개요
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---


# 믹서의 Substance 개요

## 플러그인 개요

Substance 3D 추가 기능을 통해 Substance 재질을 Blender로 가져올 수 있습니다. Substance 3D 패널을 사용하여 한 곳에서 프로젝트의 Substance 재질을 관리하고 사용자 정의할 수 있습니다. 추가 기능은 .sbsar 파일에서 텍스처 맵을 생성하고 이를 사용하여 블렌더 재질을 만듭니다. 이러한 텍스처는 Substance 매개변수가 조정되면 자동으로 업데이트됩니다.

## Substance 재료 가져오기

1. Substance 3D 패널에서 **로드** 단추를 클릭합니다.
1. 창이 열리면 .sbsar 파일이 저장된 위치로 이동하여 하나 이상을 선택합니다. 그런 다음 **Substance 재질 불러오기** 단추를 클릭합니다.
1. 재질 패널에서 구 아이콘을 클릭하여 드롭다운을 열고 Substance 재질을 선택합니다. 그러면 현재 슬롯에 재질이 할당됩니다. 또는 Substance 3D 패널의 [적용] 버튼을 사용하여 현재 할당을 재정의하지 않는 새 재질 슬롯에 재질을 할당할 수 있습니다.

>[!NOTE]
>
> 개체에 재질이 없는 경우 **적용** 단추를 사용하면 Substance 재질이 자동으로 첨부됩니다.

![](../../../assets/blender-overview-steps.png)

## Substance 3D 패널

Substance 3D 패널은 프로젝트에서 Substance 재질을 관리하고 개별 매개 변수를 조정하는 데 사용됩니다. [그래프 매개 변수] 섹션에는 텍스처 해상도, 타일링, 임의화 및 사전 설정에 대한 컨트롤이 있습니다. [출력] 섹션에는 생성된 텍스처의 이미지 형식에 대한 컨트롤이 있습니다. 여기서 Substance 매개 변수 섹션은 Substance 매개 변수를 조정할 수 있는 위치입니다.

자세한 내용은 [Substance 3D 패널](../../../3d-applications/blender/the-3d-panel/the-substance-3d-panel.md) 페이지를 참조하세요.

## 환경 설정

추가 기능 환경 설정에서 기본 비헤이비어 및 기타 설정을 조정할 수 있습니다. &quot;자재 자동 첨부&quot;를 활성화하여 자동으로 Substance 자재를 객체에 첨부하고 현재 자재 지정을 무효화할 수 있습니다. &quot;선택한 개체의 재질을 자동으로 강조 표시&quot;하면 해당 재질을 가진 개체를 선택하면 Substance 3D 패널에서 강조 표시된 재질이 변경됩니다. &quot;순환 자동 업데이트 텍스처&quot;를 활성화하면 순환 렌더링 보기를 사용하는 동안 3D 뷰포트에서 텍스처를 업데이트할 수 있습니다.

변위는 출력 섹션의 Height 토글을 사용하여 활성화할 수 있습니다. 여기에서 각 출력의 파일 형식 및 비트 심도를 조정할 수도 있습니다.

자세한 내용은 [환경 설정](../../../3d-applications/blender/preferences/preferences.md) 페이지를 참조하세요.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-1-v2.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-2-v2.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-3.png)

</td>
</tr>
</table>

## 더 많은 Substance 재질 찾기

수천 개에 이르는 전문적으로 제작된 자료와 기타 에셋을 [Substance 3D Assets 페이지](https://helpx.adobe.com/kr/substance-3d/unlisted/assets.html)에서 다운로드할 수 있습니다. 커뮤니티에서 무료로 공유한 더 많은 에셋은 [Substance 3D 커뮤니티 에셋 페이지](https://helpx.adobe.com/kr/substance-3d/unlisted/community-assets.html)에서 찾을 수 있습니다.

## 커뮤니티

일반적인 도움말, 피드백 또는 결함을 보고하려면 [Substance 디스코드 서버](https://discord.com/invite/substance3d) 또는 [Adobe 커뮤니티](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender)에서 #substance-blender-beta 채널에 가입하십시오.
