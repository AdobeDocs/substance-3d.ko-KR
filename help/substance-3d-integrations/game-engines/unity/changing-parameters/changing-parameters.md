---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unity/changing-parameters.html"
breadcrumb-title: ''
description: Unity에서 Substance 재질 매개변수를 수정하여 런타임에 재질 모양과 속성을 사용자 정의합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Changing parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 매개 변수 변경
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# 매개 변수 변경

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

Substance 재질에 대한 매개 변수는 Substance 그래프 개체(SGO)에서 액세스할 수 있습니다.

1. [프로젝트] 창에서 사용자 정의할 그래프의 sbsar 파일 로고를 선택합니다. SBSAR에 녹색 &quot;SBSAR&quot; 로고가 있습니다.

   ![](../../../assets/screen-shot-2022-03-29-at-2-27-56-pm.png)

## 절차 등록 정보

1. **모든 출력 생성**: Substance sbsar 파일에서 모든 출력을 생성합니다. 기본적으로 표준 셰이더에서 사용하는 출력만 생성됩니다.
1. **밉맵 생성**: 각 Substance 출력에 대한 밉을 생성합니다.
1. **임의 시드**: 이 단추는 Substance 그래프에서 텍스처를 생성하는 데 사용하는 임의 시드를 변경합니다. 이 값을 변경하면 시드 값을 기반으로 계산된 텍스처에 대한 새 결과가 생성됩니다.
1. Substance 파일에 표시되는 매개 변수는 Unity에서 사용할 수 있습니다. Editor 컨트롤은 Substance에 대해 만든 매개 변수의 형식을 기반으로 합니다.
1. **사전 설정 처리:** Substance 사전 설정 파일(sbsars)을 내보내거나 가져올 수 있습니다. 사전 설정을 내보내면 해당 Substance의 매개 변수 설정을 기반으로 사전 설정 파일이 만들어집니다. Substance Designer 및 Substance Player에서 사전 설정 파일을 내보낸 다음 사전 설정 가져오기 버튼을 사용하여 가져올 수 있습니다. 이는 응용 프로그램과 팀 간에 Substance 사전 설정을 공유하는 데 유용합니다.

</td>
<td style="border: 0;" valign="top">

![](../../../assets/changing-parameters.png)

</td>
</tr>
</table>
