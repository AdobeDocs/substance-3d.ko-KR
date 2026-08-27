---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/3ds-max/troubleshooting.html"
breadcrumb-title: ''
description: 오류 메시지에 대해 Script Listener를 사용하여 3ds Max에서 Substance 플러그인 문제를 진단하고 해결합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 문제 해결
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 1%

---


# 문제 해결

Scripting Listener를 사용하여 플러그인을 사용하는 동안 발생한 오류를 진단할 수 있습니다. 스크립트 리스너를 열려면 [스크립팅 메뉴] > [스크립트 리스너]로 이동합니다. 플러그인 사용 중에 오류가 발생하면 해당 오류 메시지가 이 Script Listener 창에 인쇄됩니다. 자세한 내용은 [공식 스크립트 편집기 설명서](https://help.autodesk.com/view/3DSMAX/2023/ENU/?guid=GUID-C8019A8A-207F-48A0-985E-18D47FAD8F36)를 참조하십시오.

버그를 보고하려면 [Substance 디스코드 서버](https://discord.com/invite/substance3d)에서 #3dsmax-plugin 채널에 가입하거나 [Adobe 커뮤니티](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax)를 방문하세요. 콘솔 로그의 관련 정보와 문제에 대한 복제 단계를 보고서에 포함할 수 있습니다.

## 알려진 문제

* *확산 출력을 사용하는 .sbsar를 확산기를 사용하지 않는 .sbsar로 바꾸면 누락된 확산기가 연결 해제되어 검정 렌더링이 이루어집니다.*
  * 다중 출력 노드에 대해 예상된 동작입니다. 이러한 .sbsars를 동일한 노드를 사용하여 로드하는 대신 각 노드에 서로 다른 Substance 노드를 사용하는 것이 좋습니다.
