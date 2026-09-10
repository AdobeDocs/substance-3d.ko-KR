---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: 형상 캐싱을 사용하여 미리 처리된 메시 데이터를 보존하고 후속 베이킹 작업의 속도를 크게 높일 수 있습니다.
helpx_creative_field: ""
helpx_description: bakers > Features > Geometry Cache
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 형상 캐시
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# 형상 캐시

베이킹할 때, 메시는 베이킹 공정과 양립할 수 있는 포맷으로 정제되기 위해 전처리된다. 형상 캐시는 소스 메쉬가 변경되지 않는 한 나중에 이 작업을 다시 수행하지 않도록 미리 처리된 형상을 신속하게 다시 로드할 수 있는 방식으로 유지하는 방법입니다.

* **Substance Designer**&#x200B;에서 첫 번째 굽기가 실행된 후 모양 캐시가 만들어집니다. 그런 다음 캐시는 베이커 창이 닫힐 때까지 메모리에 보관됩니다.
* **Substance Painter**&#x200B;에서 모양 캐시는 첫 번째 베이크 후 소스 파일 옆에 **어스빈** 확장명을 가진 파일로 저장됩니다.

형상 캐시를 재사용하면 특히 베이커 설정을 수정하여 완벽한 결과를 얻을 때 베이킹 프로세스가 상당히 빨라집니다.
