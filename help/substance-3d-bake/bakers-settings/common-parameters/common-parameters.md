---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: 모든 베이커에 적용되는 일반적인 매개 변수와 최적의 텍스처 생성을 위해 매개 변수를 구성하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Common Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 공통 매개 변수
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 1%

---


# 공통 매개 변수

공통 매개 변수는 모든 제빵사에 적용됩니다. 이러한 매개 변수는 일반적으로 베이커가 하이 폴리 메시로 어떻게 움직이고 작업할지, 그러나 최종 텍스처가 어떻게 생성될지를 정의합니다. 이러한 매개 변수 중 일부는 특정 베이커에서 재정의할 수 있습니다.

이러한 매개 변수 대부분은 모든 소프트웨어(Substance 자동화 툴킷 포함)에서 사용할 수 있지만, 소프트웨어 작업 과정 및 구현에 따라 일부 매개 변수는 사용할 수 없거나 동작이 약간 다를 수 있습니다.

## 일반 매개 변수

이러한 매개 변수는 베이커가 텍스처를 생성하는 방식에 영향을 줍니다.

| *이름* | *설명* |
| --- | --- |
| **크기**(기본 크기 또는 출력 크기) | 베이킹 출력 텍스처 해상도를 제어합니다(픽셀 단위).사용 가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong>(기본값)</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>정사각형이 아닌 해상도도 지원됩니다(예: 2048x1024(2:1 비율). Substance Designer에서 이 매개 변수는 베이커 자체에 의해 재정의될 수 있습니다. |
| **형식** | 구워진 텍스처의 파일 형식입니다.*Substance Painter에서 사용할 수 없습니다.* [베이킹된 맵을 내보내는 방법](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)을 참조하세요. |
| **앤티 앨리어싱** | 앤티 앨리어싱을 제어하여 구운 텍스처의 품질을 향상시키고 다른 형상이 연결되는 경우 앨리어싱을 줄일 수 있습니다.앨리어싱에 대해 자세히 알아보려면 [UV 이음새에 앨리어싱](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) 및 [위키피디아에 앨리어싱](https://en.wikipedia.org/wiki/Aliasing)을 참조하십시오.사용 가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>없음</strong>(기본값)</li><li data-preserve-html="true"><strong>서브샘플링 2x2</strong></li><li data-preserve-html="true"><strong>서브샘플링 4x4</strong></li><li data-preserve-html="true"><strong>서브샘플링 8x8</strong></li></ul>  **참고:** 앤티 앨리어스를 사용하면 텍스처를 더 높은 해상도로 계산한 다음 원래 선택한 크기로 다시 다운스케일링하여 앤티 앨리어스를 적용할 수 있으므로 베이킹 시간이 상당히 늘어날 수 있습니다. 즉, 2x2 서브샘플링을 사용하는 2K 텍스처는 실제로 4K 텍스처를 계산합니다.때로는 서브샘플링을 증가시키기보다는 베이커에서 광선의 수를 증가시키는 것이 바람직하다. 너무 오래 기다리지 않고도 더 나은 결과를 얻을 수 있었다. |
| **UV 설정** | 구운 텍스처를 계산하는 데 사용할 낮은 폴리 메쉬의 UV를 제어합니다.*Substance Painter에서 사용할 수 없습니다.* |
|  |  |
| **확장(px)** | 제공된 픽셀의 양만큼 UV의 픽셀을 바깥 또는 그 테두리로 확장/확장합니다. 이 작업을 사용하면 이러한 테두리가 텍스처 픽셀과 완벽하게 정렬되지 않거나 텍스처 해상도가 감소하는 경우(예: 밉맵) UV 테두리에서 이음새가 생기지 않습니다. 베이킹 공정 이후에 적용되는 후공정입니다. 이것은 때때로 &quot;패딩&quot;이라고도 불릴 수 있습니다.확장에 대한 자세한 내용은 [UV 솔기의 앨리어싱](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) 및 [패딩](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/padding-134643719.html)을 참조하세요. |
| **확산 적용** | 활성화되면 UV 테두리를 기반으로 UV 외부가 매끄러운 그레이디언트 색상으로 채워집니다. 이 프로세스를 통해 텍스처 크기를 줄이면 안정적으로 유지되고 과도하게 표시되는 이음새(예: 밉맵)를 만들지 않습니다. 베이킹 공정 이후에 적용되는 후공정입니다. |
| **평균 표준** | 활성화된 경우 는 베이킹의 메쉬 일치 프로세스 중에 어느 방향으로 광선을 보낼지 알 수 있는 정점의 평균 법선을 계산합니다. 비활성화된 경우 광선은 메쉬의 원래 정점 표준을 따릅니다. |

## 높은 폴리 매개 변수

다음 매개 변수는 높은 폴리 대 낮은 폴리 메쉬 베이킹(&quot;메쉬 베이커&quot;)을 제어합니다.

| *이름* | *설명* |
| --- | --- |
| **HD 메시** | 상위-폴리 메쉬를 포함하는 파일(또는 Substance 패키지 리소스) 목록입니다. 베이킹 프로세스가 다른 정보를 계산하고 해당 메시 정보를 텍스처에 저장할 때 베이커가 메모리에 로드합니다. &quot;**고해상도로 낮음 사용**&quot;을 사용하도록 설정한 경우 이 목록이 무시됩니다. |
| **낮은 해상도를 높은 정의로 사용** 또는 **낮은 폴리 메시를 높은 폴리 메시로 사용** | 활성화되면 베이커에 제공되는 높은-폴리 메쉬 목록이 무시되고 낮은-폴리 메쉬가 대신 적용됩니다.이 매개 변수는 높은 폴리 메시로 직접 작업할 때 유용합니다. 예를 들어, 이 설정을 활성화한 상태로 하이 폴리 카용 앰비언트 오클루전 텍스처를 굽는 경우 광선 거리가 무시되고 베이커가 완벽한 베이크(광선 실수 또는 형상 불일치 없음)를 생성합니다. |
|  |  |
| **케이지로 거리 설정** 또는 **케이지 사용** | 광선 거리 값을 사용하는 대신 베이킹 프로세스에서 케이지 메시 파일을 사용할지 여부를 나타냅니다. 케이지는 광선 최대 거리와 방향을 제어합니다. |
| **Cage 파일** | 케이지가 포함된 메시 파일의 경로입니다. |
| **정면 값** 또는 **최대 정면 거리** | 광선이 경로를 따라 높은 폴리 형상을 찾기 시작할 낮은 폴리 표면 위의 거리를 제어합니다.*케이지를 사용할 때는 이 설정이 적용되지 않습니다.* |
| **후방 값** 또는 **최대 후방 거리** | 낮은 폴리 표면 아래에서 광선의 경로를 따라 높은 폴리 형상을 찾기 위해 광선이 멈추는 거리를 제어합니다.*케이지를 사용할 때는 이 설정이 적용되지 않습니다.* |
| **테두리 상자 기준** | 활성화되면, 광선 거리 및 다른 크기 기반 계산은 저-폴리 메시의 정규화된 공간에 기초한다. 비활성화된 경우 광선 거리 계산은 내보낼 때 낮은 폴리 메시(미터, 센티미터 등)에 지정된 단위를 기반으로 합니다.이 설정을 비활성화하고 객체에 정밀한 측정이 있는 경우 광선 거리를 수동으로 입력하는 것이 유용할 수 있습니다. |
|  |  |
| **일치** | 베이커가 낮은 도형과 높은 도형을 일치시키는 방법을 나타냅니다. 수동으로 메쉬를 분리(분해)시킬 필요 없이 베이킹 프로세스를 필터링하는 데 사용할 수 있습니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>항상</strong>(기본값): 낮은 폴리 메시가 모든 높은 폴리 메시와 일치합니다.</li><li data-preserve-html="true"><strong>메시 이름별</strong>: 메시 이름을 기준으로 필터링하여 원하지 않는 형상과 일치하지 않도록 합니다.</li></ul>일치하는 도형에 대해 자세히 알아보려면 [이름별 일치](../../features/matching-by-name/matching-by-name.md)를 참조하세요. |
| **접미사 일치** 또는 **높은 메시 접미사** **낮은 메시 접미사** | 메쉬 이름(Mesh name)은 이름별 일치(Matching By Name) 피쳐를 사용할 때 형상을 식별하고 함께 그룹화하는 접미사입니다. 사용 가능한 접미어:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>낮은 폴리 메시</strong>: 장면의 낮은 폴리 메시를 식별하는 접미어</li><li data-preserve-html="true"><strong>높은 폴리 메시</strong>: 장면의 높은 폴리 메시를 식별하는 접미어</li><li data-preserve-html="true"><strong>뒷면 무시</strong>: 특정 베이커가 무시해야 하는 망을 식별하는 접미어([메시에서 앰비언트 오클루전](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)와 유사)</li></ul>도형 일치에 대한 자세한 내용은 [이름별 일치](../../features/matching-by-name/matching-by-name.md) 를 참조하십시오. |
|  |  |
| **기울이기 교정 사용** | 활성화된 경우 광선 방향은 입력 텍스처에 따라 **평균 표준**&#x200B;이나 원래 모양 표준에서 계산됩니다. 텍스처의 검정색 값은 평균 표준 계산을 사용하고 흰색 값은 원래 메시 표준을 사용합니다.*Substance Painter에서 사용할 수 없습니다.* |
| **기울이기 맵** | 광선 투영을 기울이는 데 사용되는 텍스처 파일의 경로 |
| **기울이기 교정 반전** | 입력 텍스처의 판독값을 반전합니다(검정은 흰색이 되고 흰색은 검정이 됨). |
