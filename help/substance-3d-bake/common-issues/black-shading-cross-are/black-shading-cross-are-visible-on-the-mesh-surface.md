---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/common-issues/black-shading-cross-are-visible-on-the-mesh-surface.html"
breadcrumb-title: ''
description: 탄젠트 공간과 수직 계산을 수정하여 메시 표면에 표시되는 검은색 음영 가공물을 수정합니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Black shading cross are visible on the mesh surface
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시 표면에 검은색 음영 십자가 표시됨
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# 메시 표면에 검은색 음영 십자가 표시됨

조명 아래에서는 메쉬의 여러 영역에 검은색 음영 가공물이 나타납니다.

![](../../assets/black-shading-cross.jpg)


## 설명

검정색 음영 십자는 일반적으로 메쉬 형상이 변경되었거나 베이커가 수행한 계산과 다른 방식으로 계산되었기 때문에 노멀 맵이 메쉬와 일치하지 않음을 의미합니다. 예를 들어 메쉬의 삼각측정은 메쉬와 해당 노멀 맵을 렌더링하는 베이커와 뷰포트 간에 다릅니다.

## 해결 방법

메시 및 해당 노멀 맵이 표시된 응용 프로그램이 텍스처가 생성된 방식과 동기화되었는지 확인합니다. 이것은 다음을 의미합니다.

* 뷰어와 베이커 간의 접선 공간이 동일한지 확인합니다.
* 보기와 베이커 간에 표준 형식이 동일한지 확인합니다.
* 보는 사람과 제빵하는 사람 사이의 삼각 측량이 동일한지 확인합니다. 자세한 내용은 [이 페이지](../../guides/triangulating-before-bak/triangulating-before-baking.md)를 참조하세요.
