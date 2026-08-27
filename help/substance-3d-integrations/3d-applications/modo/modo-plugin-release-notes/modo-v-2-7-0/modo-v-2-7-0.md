---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/modo/modo-plugin-release-notes/modo-v-2-7-0.html"
breadcrumb-title: ''
description: MODO 플러그인 버전 2.7.0의 릴리스 정보를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Plugin Release Notes > Modo v. 2.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 모도 대 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---


# 모도 대 2.7.0

* 다양한 충돌 수정 사항
* 32비트 부동 지원
* CPU 엔진에서는 4k 텍스처가, GPU 엔진에서는 8k 텍스처가 지원됩니다
* 플러그인 릴리스에 대한 새 LPK 형식
* Substance 플러그인의 새 키트 메뉴
* glTF / MODO 12.0에 대한 Principled 셰이더 지원
* Substance 파일에 대한 상대 경로 추가
* Linux 지원
* 사전 설정 로드 및 저장을 위한 새로운 UI
* 포함된 사전 설정은 Designer에서 로드됩니다.
* GPU 메모리 경고 상자 제거됨
* 편집된 사전 설정 로드/저장 명령

  사용할 수 있는 새 명령은 다음과 같습니다.

  **substance.getsbsname** substance 개체의 식별자를 내부 이름으로 변환합니다

  다음은 모두 substance.getsbsname에서 얻은 적절한 내부 이름입니다.

  **substance.setpreset** Substance의 현재 사전 설정을 인덱스 **substance.getpresetindex**&#x200B;에 설정합니다. 현재 사전 설정 인덱스 **substance.getpresetat**&#x200B;지정된 **index substance.getpresetcount**&#x200B;에서 사전 설정의 문자열 이름을 반환합니다. Substance이 가지는 사전 설정의 수를 반환합니다.**substance.savepresetfile** 현재 구성의 사전 설정을 지정된 파일 경로에 저장합니다. **substance.loadpresetfile** 파일 경로가 지정된 Substance에 사전 설정 파일을 로드합니다.

  UI 명령:

  사전 설정 **substance.savepresetui**&#x200B;을(를) 로드하는 **substance.loadpresetui** UI 명령 사전 설정을 저장하는 **substance.selectpresetui** UI 명령 사전 설정을 설정하는 UI
