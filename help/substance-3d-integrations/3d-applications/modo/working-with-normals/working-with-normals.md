---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/working-with-normals.html"
breadcrumb-title: ''
description: MODO에서 노멀 맵 방향 설정을 구성하여 Substance 재질을 사용한 노멀 맵 렌더링이 올바르게 수행되도록 합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Normals
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 표준 작업
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# 표준 작업

일반 데이터를 사용한 작업 - 올바른 방향 설정

스톡 Substance은 DX 일반 방향을 사용하도록 제작되었습니다. 그러나 MODO는 OGL을 사용합니다. 표준 형식(Normal Format) 매개변수를 1.0으로 설정하여 표준을 뒤집을 수 있습니다. Substance 플러그인은 Substance에 설정된 매개 변수만 해석합니다. &quot;normal\_format&quot; 매개 변수가 없는 Substance은 Substance 작성자가 이 컨트롤을 사용자 지정 Substance에 추가하는 데 달려 있습니다. 이 매개 변수가 없는 Substance이 발생한 경우 노멀 맵의 텍스처 레이어에서 녹색 채널을 뒤집어 방향을 수정할 수 있습니다.

>[!NOTE]
>
> 녹색 채널을 뒤집는 것은 Substance의 기본 방향이 잘못되고 작성자가 Substance 매개 변수에서 표준을 뒤집는 컨트롤을 만들지 않은 경우에만 가능합니다

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/normal-1.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/invert-2.png)

</td>
</tr>
</table>
