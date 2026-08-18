---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/working-with-emissive.html"
breadcrumb-title: ''
description: MODO의 Substance 재료에 대한 발광 특성을 구성하여 광도 및 색상 설정을 제어합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Emissive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Emissive를 사용한 작업
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Emissive를 사용한 작업

## 발광(광도 및 색상)을 사용한 작업

Substance은 옵션으로 방출 출력을 가질 수 있습니다. 이것을 MODO에서 야광량과 색으로 사용할 수 있습니다. 방출 출력을 활성화하면 광도량 효과로 설정됩니다. 기본적으로 이 채널은 [텍스처 이미지 스틸] 탭에서 [선형]으로 해석됩니다.\
셰이더 트리에서 텍스처를 마우스 오른쪽 단추로 클릭하고 복제를 선택합니다. 그런 다음 복제된 발광 텍스처를 발광 색상 효과로 설정합니다. 그런 다음 광도량 효과를 구동하는 텍스처에 대해 높은 값과 낮은 값을 변경하여 값을 더욱 강화할 수 있습니다.

>[!NOTE]
>
> 야광 색상으로 설정된 텍스처의 경우, 이미지 스틸 탭에서 해석을 sRGB로 설정해야 합니다.

흐림 효과를 얻으려면 렌더링 패널에서 흐림 을 활성화하고 한계값과 반경을 설정해야 합니다.

![](../../../assets/bloom.png)

Unreal 및 Unity 재질의 경우 Emissive 출력은 특히 이 재질에 의해 처리됩니다.\
Unreal = Unreal Emissive\
유니티 = 유니티 방출

비실시간 발광 및 단일 발광 텍스처는 이미지 스틸 탭에서 선형에서 sRGB로 변경해야 합니다.
