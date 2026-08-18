---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/bakers-settings/curvature.html"
breadcrumb-title: ''
description: 메쉬에서 곡률 정보를 추출하여 형상의 캐비티와 모서리를 강조하는 텍스처를 생성합니다.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 곡선
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%

---


# 곡선

곡률 베이커는 곡률 텍스처를 추출할 수 있습니다. 이 텍스처에는 형상과 관련된 캐비티와 모서리 정보가 포함됩니다.

텍스처 속성은 다음과 같이 정의됩니다.

* 검정색 값은 오목 영역을 나타냅니다.
* 흰색 값은 볼록 영역을 나타냅니다.
* 회색 값은 중간 영역(주로 평면)을 나타냅니다.

**사용 가능 대상:**

* Substance Designer
* Substance 자동화 툴킷
* Substance Painter

## 매개변수

| *매개 변수* | *설명* |
| --- | --- |
| **알고리즘** | 메쉬에서 곡률 정보가 계산되는 방법을 정의합니다. |
| **세부 정보** | 곡률 정보의 강도를 제어합니다. 값이 높으면 세부 사항은 더 많이, 미묘는 더 적게 표현할 수 있습니다. |
| **연결 사용** | 활성화되면 베이커는 한쪽에서 다른 쪽으로 테두리의 텍스트를 복사하여 UV 섬 사이의 이음새를 줄이려고 합니다. |
| **이음새** **강도** | **이음새 사용**&#x200B;을 사용하도록 설정한 경우 이 매개 변수는 이음새 수정 수준을 제어합니다. |
