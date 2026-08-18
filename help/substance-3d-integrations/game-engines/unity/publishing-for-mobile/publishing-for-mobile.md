---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/publishing-for-mobile.html"
breadcrumb-title: ''
description: 설정 및 텍스처 해상도를 조정하여 Unity에서 모바일 플랫폼용 Substance 재질을 최적화합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Publishing for Mobile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 모바일용 게시
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# 모바일용 게시

>[!NOTE]
>
> **모바일 장치의 텍스처 크기**
> 
> Unity Editor에서 설정된 텍스처의 해상도는 앱 바이너리에 게시되는 크기입니다. Substance 재질의 해상도를 낮추면 더 작은 파일 크기의 텍스처가 만들어집니다.

## 플랫폼

## Apple iOS

1. iOS 모듈이 해당 Unity 버전에 대해 다운로드되었는지 확인합니다.
1. Unity에서 빌드 대상을 iOS으로 변경합니다.
1. 플레이어 설정을 열고 &#39;Identification - Bundle Identifier&#39; 필드를 더 고유한 항목으로 변경합니다. (예: com.Adobe.iosProject)
1. 게임을 빌드하고 실행합니다.
1. Xcode에서 iOS 디바이스를 클릭하고 &#39;서명 - 팀&#39; 드롭다운을 개발자 팀 ID로 변경합니다.
1. iOS 장치에서 &#39;설정 - 일반 - 장치 관리&#39;로 이동하고 표시되는 개발자 팀 ID에서 &#39;신뢰&#39;를 클릭합니다.
1. &#39;현재 구성표 빌드 및 실행&#39; 단추(재생 단추)를 클릭하여 Xcode 빌드를 다시 실행합니다.
1. iOS 디바이스에서 게임이 실행되고 있어야 합니다.

## 안드로이드

1. 해당 Unity 버전용으로 Android 모듈이 다운로드되었는지 확인합니다.
1. Unity에서 빌드 대상을 Android로 변경합니다.
1. 플레이어 설정을 열고 &#39;Identification - Bundle Identifier&#39; 필드를 더 고유한 항목으로 변경합니다. (예: com.androidProject)
1. 게임을 빌드하고 실행합니다.
1. 게임은 안드로이드 장치에서 실행해야합니다.
