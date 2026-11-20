---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ""
description: 3ds Max용 Substance 플러그인과 프로젝트에서 Substance 재질을 가져오고 사용하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max의 Substance 개요
user-guide-description: ""
user-guide-title: ""
source-git-commit: a167bcd2c2f0af70b3a4dc37eafc85145c79c590
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%
---

# 3ds Max의 Substance 개요

## 플러그인 개요

## Substance 열기

1. 슬레이트 편집기를 열고 Substance을 검색하고 Substance2 노드를 보기로 드래그합니다.
1. Substance 노드를 두 번 클릭하여 속성을 활성화하고 Substance 패키지 브라우저에서 Substance을 로드합니다.

   >[!NOTE]
   >
   > .sbsar 파일을 [슬레이트 편집기]로 끌어 놓으면 노드가 자동으로 만들어지고 sbar를 가져올 수도 있습니다.

1. Substance에 여러 그래프가 포함된 경우 [선택한 그래프] 드롭다운 메뉴에서 자료로 출력할 그래프를 선택할 수 있습니다.

   ![](../../../assets/max1.png)

1. Substance 노드가 선택된 상태에서 Substance 메뉴로 이동하여 지원되는 렌더러를 선택합니다. 재질이 만들어지고 개체에 적용될 준비가 됩니다. Substance 텍스처가 렌더링 재질에 후크됩니다.

>[!NOTE]
>
> **&quot;Substance2&quot;** 노드를 선택한 후에는 **로드 Substance...**&#x200B;를 먼저 클릭하여 sbsar 파일을 선택한 다음 상단 메뉴에서 지원되는 렌더러(예: &quot;Arnold로 Substance&quot;)를 선택해야 합니다.
>
>지원 렌더러로는 Arnold, V-Ray, Corona 및 Octane 등이 있습니다. [OpenPBR 재질을 사용하는 방법을 알아보려면 3DS Max의 워크플로우에 대해 알아보세요.](../using-workflows-3ds-max/using-workflows-in-3ds-max.md)

![](../../../assets/max3.png)

## 해상도 변경

1. [Substance 출력 설정]에서 계산된 Substance 텍스처에 원하는 해상도를 설정합니다.
1. 최대 8K의 해상도에 대해 [Substance 설정](../../../3d-applications/3ds-max/settings-1/substance-settings.md)에 설정된 GPU 엔진을 사용하고 있는지 확인하십시오.

   ![](../../../assets/max6.png)

## 매개변수 변경

1. Substance 노드를 두 번 클릭하여 매개변수 창에 Substance 매개변수를 로드합니다.
1. 매개 변수를 변경하여 Substance 텍스처를 자동으로 업데이트합니다.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## 출력 미리 보기 설정

Substance 노드의 축소판에 대해 특정 채널을 설정할 수 있습니다.

1. [출력 미리 보기] 드롭다운에서 노드 축소판에 사용할 채널을 선택합니다.

   ![](../../../assets/max7.png)

## 타일링 Substance

[좌표] 속성을 사용하여 Substance 텍스처를 바둑판식으로 배열하고 [채널 매핑]을 설정할 수 있습니다.

![](../../../assets/max10.png)
