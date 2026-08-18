---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: 베이커 출력이 완전히 검정색이거나 비어 있는 이유를 해결하고 메쉬 및 UV 문제를 해결하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baker output is fully black or empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 베이커 출력이 완전히 검정색이거나 비어 있음
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# 베이커 출력이 완전히 검정색이거나 비어 있음

>[!WARNING]
>
> **문제**
> 
> 베이커의 결과는 검정색이거나 비어 있는 텍스처입니다.
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **설명**
> 
> 검정색 텍스처는 제빵사가 결과를 출력하는 데 필요한 정보를 찾을 수 없었음을 의미합니다. 예를 들어, 베이킹 프로세스에서는 낮은 폴리와 일치하는 높은 폴리 메시를 찾지 못하여 비교할 대상이 없습니다.

>[!NOTE]
>
> **해결 방법**
> 
> * 베이커에 필요한 높은 폴리 메시가 제대로 로드되었는지 확인합니다(오류는 로그 파일/창 참조).
> * 낮은 폴리 또는 높은 폴리 메시가 너무 크지 않은지(1km 이상) 또는 너무 작은지(1cm 미만) 확인합니다.
> * 베이커가 메시를 읽거나 처리할 수 있는지 확인합니다(오류는 로그 파일/창 참조).
> * [이름별 일치](../../features/matching-by-name/matching-by-name.md) 기능이 제대로 설정되지 않았는지 확인합니다(일부 개체가 서로 제외되고 겹치지 않을 수 있음).
> * 낮은 폴리 UV가 0-1 범위 내에 있는지 확인합니다.
