---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: 메시 삼각측정이 베이킹 결과에 어떤 영향을 미치는지 이해하고 형상을 준비하기 위한 모범 사례를 알아보십시오.
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 굽기 전 삼각 측량
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 굽기 전 삼각 측량

3D 메시는 면당 여러 테두리 가장자리를 가진 다각형으로 정의할 수 있습니다. 일반적으로 4개의 모서리를 통해, 때로는 그 이상(n-gons)을 거칩니다.\
소프트웨어는 (특히 GPU에서) 쉽게 관리하고 계산을 수행할 수 있기 때문에 나중에 다각형을 Trigons로 만들 수 있습니다.

## 삼각측량이 메시에 어떤 영향을 미칠 수 있습니까?

![](../../assets/triangulation.jpg)

Quad/N-Gons를 삼각형으로 변환하는 **표준 솔루션**&#x200B;이 없습니다. 위의 이미지에서 입증된 바와 같이, 여러 가지 선택이 유효합니다.\
베이커들은 우리가 특정한 알고리즘을 다른 알고리즘보다 선택하기 때문에 게임 엔진처럼 메시를 삼각형으로 다룰 가능성은 낮다.

## 굽기 전에 삼각측량하는 이유는 무엇인가요?

베이킹 프로세스에서는 형상을 읽은 다음 정보를 텍스처로 인코딩합니다.\
이러한 정보는 UV를 기반으로 하며 경우에 따라 메시 토폴로지에 있으므로 다른 소프트웨어가 텍스처를 적용할 때와 같은 방법으로 형상을 읽지 않으면 정보를 잘못 디코딩할 수 있습니다.

아래 이미지에서는 왼쪽 위에 낮은 폴리 메쉬가 있고 오른쪽 위에 높은 폴리 메쉬가 있습니다.\
바닥에는 높은 폴리에서 구운 노멀 맵이 있는 낮은 폴리가 있습니다. 왼쪽의 망은 베이킹할 때 Substance Painter이 사용한 것과 같은 삼각 측량을 사용한다. 오른쪽의 메시는 검은색 가공물을 표시하지 않고 표시합니다. 노멀 맵이 생성된 방법과 메시가 현재 삼각측정되는 방법이 일치하지 않기 때문입니다. 이 문제는 **메시 업데이트 및/또는 다시 굽기**&#x200B;를 통해 해결할 수 있습니다.

![](../../assets/example-triangulation-artifact.jpg)
