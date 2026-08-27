---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/live-link-in-ue4.html"
breadcrumb-title: ''
description: Unreal Engine 4의 Live Link 를 사용하여 Painter과 UE4 간에 실시간으로 Substance 자료를 동기화합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Live Link in UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UE4의 라이브 링크
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# UE4의 라이브 링크

>[!WARNING]
>
> Unreal Engine의 라이브 링크는 더 이상 지원되지 않습니다. Live Link가 사용되는 이전 버전의 플러그인이 있는 사용자는 계속 이 기능을 사용할 수 있습니다.

>[!WARNING]
>
> Live Link가 UE4 BSP 메시에서 작동하지 않습니다. 보내는 에셋은 UE4 프로젝트로 가져온 모델 파일이어야 합니다

## Substance Painter 링크 설정

1. Substance Painter 열기
1. 콘텐츠 브라우저에서 Painter으로 보낼 에셋을 마우스 오른쪽 버튼으로 클릭하고 &quot;Painter으로 보내기&quot;를 선택합니다.

   ![](../../../../assets/link1-22.png){width="400px"}
1. Substance Painter에 메쉬가 표시되면 텍스처링을 시작할 수 있습니다. 작업하면서 텍스처는 UE4로 전송되고 재질에 적용됩니다. 도구 모음의 UE4 아이콘에 있는 녹색 점은 링크가 라이브 상태이고 텍스처를 보내고 있음을 나타냅니다.

   ![](../../../../assets/icon-12.png)

   1. 플러그인의 구성 옵션에서 데이터 스트리밍을 일시 중지할 수 있습니다. Plugins>dcc-live-link 로 이동하고 구성을 선택합니다. UE4로 데이터를 보내지 못하도록 일시 중지하려면 스트리밍 사용을 비활성화합니다.

      ![](https://helpx-prod.scene7.com/is/image/HelpxProd/config-6?$png$&jpegSize=100&wid=393)
1. Painter의 텍스처는 콘텐츠 브라우저에 표시되고 UE4의 재질에 적용됩니다.

   ![](../../../../assets/link3-11.png){width="500px"}
1. Substance Painter 프로젝트(.spp)가 &quot;.sp&quot;라는 레이블이 붙은 폴더의 UE4 프로젝트 폴더에 만들어집니다

   ![](../../../../assets/link4-5.png)

## Substance Painter에 대한 링크 재설정

Painter 또는 Unity를 닫은 후 마지막에 중단한 위치로 돌아갈 수 있습니다.

1. Unity 프로젝트>에셋>.sp 폴더에 있는 Substance Painter에서 .spp 프로젝트를 엽니다.
1. 콘텐츠 브라우저에서 메시를 마우스 오른쪽 버튼으로 클릭하고 &quot;Painter으로 보내기&quot;를 선택하여 링크를 다시 설정합니다.

   ![](../../../../assets/link5-3.png){width="600px"}
