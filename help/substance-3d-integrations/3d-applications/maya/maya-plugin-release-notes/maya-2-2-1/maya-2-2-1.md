---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-2-1.html"
breadcrumb-title: ''
description: Maya 플러그인 버전 2.2.1의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.2.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.2.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Maya 2.2.1

Maya 2.2.1 릴리스:

* Substance 엔진을 8.3.0으로 업데이트
* Arnold에 대한 기본 지원을 추가하여 디스크에 대한 캐시 필요 제거
* 이 옵션은 설정에서 렌더링 확장을 활성화하고 Maya를 다시 시작한 후에 사용할 수 있습니다
* 지원되는 버전은 다음과 같습니다.
* Maya 2017 - MtoA 3.1.0/Arnold 5.2.0
* Maya 2018 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0
* Maya 2019 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2020 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2022 - MtoA 4.2.1/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Windows 및 MacOS의 설치 디렉터리 업데이트
* 이제 MacOS/Windows의 바이너리가 Adobe 인증서를 사용하여 서명됩니다.
* 이제 sbsar의 작성자가 [알레르기성] 또는 [Adobe]일 때 [알레고리성]만 있는 것이 아니라 채널 토글이 숨겨집니다.
* 워크플로우 복제, 덮어쓰기, 이름 변경 및 삭제 기능이 추가된 새 워크플로우 UI가 추가되었습니다.

다음과 같은 새로운 스크립팅 명령이 추가되었습니다.

substancemaya

substanceGetEnableRenderingExtensions

substanceSetEnableRenderingExtensions

substanceworkflow.py

substanceWorkflowIsReadOnly

substanceWorkflowRenameWorkflow

substanceWorkflowDuplicateWorkflow

substanceWorkflowOverwriteWorkflow

substanceWorkflowRemoveWorkflow

버그 수정:

* 설정 대화 상자를 열 때 오류 수정
* PYC이 생성되었을 때 워크플로 기능이 더 이상 실패하지 않음

이 버전은 Linux, MacOS 및 Windows의 Maya 2017, 2018, 2019, 2020 및 2022와 MacOS 및 Windows의 Maya LT 2018, 2019 및 2020용으로 출시되었습니다
