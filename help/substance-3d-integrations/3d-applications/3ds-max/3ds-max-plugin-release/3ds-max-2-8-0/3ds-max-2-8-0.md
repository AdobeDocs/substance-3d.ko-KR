---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-8-0.html"
breadcrumb-title: ''
description: 3ds Max 플러그인 버전 2.8.0의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# 3ds Max 2.8.0

<b>추가/업데이트됨:
</b>

* 매개 변수의 조건부 가시성(&#39;보이는 경우&#39;)을 지원합니다. 이제 조건이 충족되지 않으면 매개 변수가 숨겨지고 해당 그룹은 계속 표시됩니다.
* 3ds Max 플러그인에서 Corona 렌더러를 버전 10으로 업그레이드하여 렌더링 기능을 개선하고
* 최신 업데이트는 Substance을 사용할 때 3ds Max 2024의 렌더링 속도 및 CPU 사용률을 크게 개선하여 3ds Max 2022에서 관찰된 효율과 성능을 더욱 가깝게 맞춥니다.

<b>고정:</b>

* 각 매개 변수에 대한 실제 범위 내에서 키보드 입력 값을 제한하여 슬라이더 컨트롤 및 수동 값 조정 문제를 방지하도록 Substance 플러그인을 개선했습니다.
* Slate Material Editor 내에서 Substance2 텍스처 변환(.sbsar)을 복사하면 복사된 노드가 의도치 않게 중단되어 d3d11.dll과 관련된 충돌이 발생할 수 있는 문제를 해결했습니다.
* Corona Interactive로 사용자 정의/편집된 복사된 재질 재질(.sbsar)을 렌더링할 때 3ds Max에서 충돌 문제를 해결했습니다.
* 정수 3 및 4 값에 대한 슬라이더가 응답하지 않고 수동 숫자 입력만 값을 업데이트하던 3ds Max의 Substance2 노드 문제를 수정했습니다. 또한 이러한 값이 float 형식으로 잘못 표시되었습니다. 이제 슬라이더가 작동하여 의도한 값 유형을 정확하게 반영합니다.
* 3ds Max 2021에서 Corona Render 시 Substance 재질이 뷰포트에 올바르게 표시되지만 파일을 다른 PC로 전송할 때 회색으로 렌더링되는 문제를 해결했습니다. 적절한 렌더링을 위해 사용자가 더 이상 재질을 처음부터 설정하거나 사전 설정을 로드할 필요가 없습니다.
* Slate Material Editor에서 충돌 노드를 복제하려고 할 때 3ds Max 플러그인의 Substance 문제를 해결했습니다.
* 3ds Max를 다시 시작한 후 Substance 플러그인의 CPU 코어 제한 설정이 저장되지 않아 사용자가 구성한 값이 세션 간에 유지되도록 하는 문제를 해결했습니다.

이 버전은 3ds Max 2021, 2022 및 2023용으로 출시되었습니다.
