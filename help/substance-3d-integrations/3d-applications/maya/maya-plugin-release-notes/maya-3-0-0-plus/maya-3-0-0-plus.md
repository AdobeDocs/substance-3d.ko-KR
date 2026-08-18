---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-3-0-0-plus.html"
breadcrumb-title: ''
description: Maya 플러그인 버전 3.0.0 이상용 릴리스 노트를 검토하여 새로운 기능, 개선 사항, 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > Maya 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Maya 3.0.0+

## Maya 3.0.3

<b>추가/업데이트:</b>

* Maya 플러그인의 캐싱 시스템은 수동 재전송이 활성화된 상태로 초기 네트워크 생성 시 한 번만 캐싱하도록 개선되었습니다.
* Maya 플러그인에서 &quot;substance&quot; 폴더의 위치를 변경하는 옵션을 제공했습니다.
* Autodesk의 Python 3.12 업데이트와 호환되도록 Maya 플러그인의 워크플로우 가져오기 시스템을 업데이트했습니다.
* Substance 플러그인 아이콘이 최신 아이콘으로 업데이트되었습니다.
* 플러그인에서 커넥터를 사용하여 사전 설정을 보내고 받을 수 있는 기능이 추가되었습니다.

<b>고정:</b>

* Maya용 Substance 플러그인을 로드/언로드하면 오류 화면이 생성되고 충돌하는 문제가 해결되었습니다.
* 특히 .exr 파일이 올바르게 참조되도록 하고, 큰 장면에서 캐싱 관련 고정을 줄이는 등의 캐싱 문제가 해결되었습니다.
* SBSAR 파일이 Maya 플러그인에 로드될 때 샘플 창의 재질 미리 보기가 표시되지 않는 문제를 해결했습니다.
* 하나 이상의 SBSAR가 이미 Hypershade에 있는 경우 커넥터가 SBSAR 파일을 수신하지 못하는 문제를 해결했습니다.
