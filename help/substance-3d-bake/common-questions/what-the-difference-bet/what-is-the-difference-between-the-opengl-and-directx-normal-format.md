---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/what-is-the-difference-between-the-opengl-and-directx-normal-format.html"
breadcrumb-title: ''
description: OpenGL과 DirectX 표준 맵 포맷의 차이점과 각 글꼴을 사용해야 하는 경우를 살펴보세요.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What is the difference between the OpenGL and DirectX normal format "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'OpenGL과 DirectX 표준 형식의 차이점은 무엇입니까? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---


# OpenGL과 DirectX 표준 형식의 차이점은 무엇입니까?

>[!WARNING]
>
> **질문**
> 
> OpenGL과 DirectX 표준 형식의 차이점은 무엇입니까?

>[!NOTE]
>
> **설명**
> 
> OpenGL 및 DirectX은 프로그래머가 응용 프로그램에서 GPU(그래픽 처리 장치)와 대화하기 위해 사용하는 두 개의 그래픽 API(함수 집합)입니다. 노멀 맵 측면에서 차이는 RGB 텍스처의 녹색 채널을 어떻게 해석해야 하는가로 귀결된다. OpenGL에서는 첫 번째 픽셀이 맨 아래에 있고 DirectX은 맨 위에 있을 것으로 예상합니다. 이러한 이유로 다양한 기술적 논의에서 노멀 맵의 녹색 채널을 반전하여 픽셀 값을 반전시킬 때(처음 이 반전될 때) 더 잘 작동하는지 확인하는 것이 좋습니다. OpenGL은 **Y+**(위쪽)이라고 할 수 있고 DirectX은 **Y-**(아래쪽)이라고 할 수 있습니다.
> 
> 사용할 형식을 알아보려면 텍스처를 사용할 대상 응용 프로그램을 참조하십시오.
