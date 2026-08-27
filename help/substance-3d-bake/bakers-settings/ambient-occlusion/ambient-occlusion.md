---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: 앰비언트 오클루전 베이커를 사용하여 빠른 GPU 가속 알고리즘을 사용하여 주변 그림자 텍스처를 생성하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 앰비언트 오클루전
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 4%

---


# 앰비언트 오클루전

앰비언트 오클루전 베이커를 사용하면 주변 그림자 텍스처를 베이킹할 수 있습니다. 이 제빵사는 GPU에서 실행되는 빠른 알고리즘을 사용합니다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷

>[!WARNING]
>
> * 이 베이커는 이전 GPU에서 지원되지 않을 수 있습니다.
> * 로우엔드/모바일 GPU에서 고해상도로 굽는 행위는 충돌으로 이어질 수 있습니다.

## 매개변수

| *이름* | *설명* |
| --- | --- |
| **표준 맵** | 베이커 계산 중에 고려될 메시 표면의 추가 형상 세부 정보를 제공하는 데 사용할 수 있는 입력 노멀 맵 파일입니다. 이 매개 변수는 선택 사항입니다. |
| **월드 스페이스** | 활성화된 경우 입력 노멀 맵이 접선 공간 대신 월드 스페이스에 있음을 지정합니다. 입력 노멀 맵을 제공하지 않으면 이 매개 변수는 무시되거나 비활성화됩니다. |
| **표준 반전** | 반전된 표준으로 앰비언트 오클루전 맵을 계산합니다(두께 맵을 생성하는 데 사용할 수 있음). |
| **선택하지 않은 메시 부분 사용** | 메시의 선택되지 않은 메시 부분을 사용하여 앰비언트 오클루전 맵을 구웁니다. |
| **품질** | 앰비언트 오클루전 맵의 품질을 선택합니다. 고품질일수록 계산 속도가 느립니다.사용 가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>낮음</strong>(3단계)</li><li data-preserve-html="true"><strong>보통</strong>(기본값, 5단계)</li><li data-preserve-html="true"><strong>높음</strong>(10 패스)</li><li data-preserve-html="true"><strong>매우 높음</strong>(16 패스)</li></ul> |
| **정밀도 편향** | 주변 오클루전의 정밀도입니다. 값이 낮을수록 정밀도가 높아지지만 더 큰 아티팩트가 생성될 수 있습니다. |
| **거리 페이드** | 앰비언트 오클루전 확산 |
