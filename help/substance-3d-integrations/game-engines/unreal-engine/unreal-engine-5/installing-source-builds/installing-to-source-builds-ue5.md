---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/installing-to-source-builds-ue5.html"
breadcrumb-title: ''
description: 사용자 정의 엔진 수정을 위한 Unreal Engine 5 소스 빌드에 Substance 3D 플러그인을 설치합니다.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 소스 빌드에 설치 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# 소스 빌드에 설치 - UE5

Substance 플러그인은 소스에서 빌드된 Unreal Engine 버전과 함께 사용할 수 있습니다. 이렇게 하려면 플러그인을 C++project 폴더 또는 소스 빌드의 엔진 폴더에 설치할 수 있습니다.

>[!NOTE]
>
> 이러한 방법을 사용하려면 마켓플레이스에서 다운로드한 플러그인 버전이 있어야 합니다. Substance 플러그인 폴더는 컴퓨터와 UE 빌드 간에 전송할 수 있습니다.

## C++ 프로젝트 폴더에 설치

1. 프로젝트 폴더에 플러그인 폴더가 아직 없다면 이 폴더를 만듭니다.
1. Plugins 폴더 내에서 런타임 폴더를 만듭니다.
1. 런타임 폴더 내에 Substance 폴더를 배치합니다. LINUX 사용자: 3단계 이후 Substance 폴더에서 &quot;include&quot; 폴더를 찾아 이름을 바꾸면 &quot;i&quot;를 대문자로 사용합니다(include > 포함).
1. Unreal 엔진을 실행합니다.
1. 시작 관리자를 통해 C++ 프로젝트를 엽니다.
1. 프로젝트를 시작한 후 Unreal Engine에서 시작하기 전에 플러그인 구성 요소를 다시 빌드할지 묻는 메시지가 표시되며 [예]를 선택합니다. 이 작업은 Microsoft Visual Studio(Windows, Linux) 또는 Xcode(Mac)를 통해 수행됩니다.
1. Unreal 엔진이 닫히지만 구성 요소가 백그라운드에서 빌드됩니다. 이 과정은 약 5분 정도 소요될 수 있습니다. 작업이 완료되면 프로젝트가 열립니다. 실패할 경우 오류 창이 표시됩니다.

## 엔진 폴더에 설치

>[!NOTE]
>
> 플러그인을 Engine 폴더에 설치하려면 먼저 위의 단계를 따라 플러그인 Binaries 폴더를 다시 작성해야 합니다.

1. 프로젝트 폴더 > Substance > 런타임 내에서 플러그인 폴더를 복사합니다.
1. Unreal Engine 버전 폴더를 열고 엔진 > 플러그인 > Marketplace 로 이동합니다.
1. Substance 폴더를 붙여넣습니다.
1. 언리얼 엔진 편집기를 엽니다. 원하는 경우 새 프로젝트를 만듭니다.
1. 플러그인 메뉴를 열고 Substance 플러그인이 활성화되어 있는지 확인합니다.
