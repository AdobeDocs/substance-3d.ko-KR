---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-bake/common-questions/texture-baked-outside-of-substance-software-looks-incorrect.html"
breadcrumb-title: ''
description: Substance 소프트웨어 외부에서 구워진 텍스처가 잘못 표시되는 이유를 해결하고 색상 공간 문제를 해결하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Texture baked outside of Substance software looks incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 소프트웨어의 외부에서 만들어진 텍스처가 잘못 보임
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Substance 소프트웨어의 외부에서 만들어진 텍스처가 잘못 보임

>[!WARNING]
>
> **질문**
> 
> Substance Painter에서 Substance Baker가 아닌 외부 애플리케이션으로 구운 텍스처가 잘못 보이는 이유는 무엇입니까?

>[!NOTE]
>
> **해결 방법**
> 
> 다음과 같은 여러 가지 요인으로 인해 문제가 발생할 수 있으므로 이 문제에 대한 즉각적인 해결 방법은 없습니다 .
> 
> * Substance 소프트웨어와 외부 응용 프로그램 간의 일반 형식이 동일한지 확인합니다. OpenGL은 [X+, Y+, Z+]이고 DirectX은 [X+, Y-, Z+]입니다.
>   * Substance Painter에서 일반 형식은 [프로젝트 구성](https://experienceleague.adobe.com/ko/docs/substance-3d-painter/using/interface/project-configuration)에서 변경할 수 있습니다.
>   * Substance Designer에서 일반 형식은 [프로젝트 환경 설정](https://experienceleague.adobe.com/ko/docs/substance-3d-designer/using/workspace/preferences/project-settings)에서 변경할 수 있습니다.
> * Substance 소프트웨어에서 메쉬를 구워 가져오기 전에 메쉬가 삼각측정되었는지 확인합니다. 자세한 내용은 [이 페이지](../../guides/triangulating-before-bak/triangulating-before-baking.md)를 참조하세요.
