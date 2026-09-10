---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/troubleshooting.html"
breadcrumb-title: ''
description: 시스템 콘솔을 사용하여 Blender에서 Substance 3D 추가 기능과 관련된 일반적인 문제를 진단하고 해결합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 문제 해결
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# 문제 해결

시스템 콘솔을 사용하여 추가 기능을 사용하는 동안 발생한 오류를 진단할 수 있습니다. 블렌더의 시스템 콘솔 창은 운영 체제에 따라 다르게 열립니다. 자세한 지침은 Blender의 시스템 콘솔 [설명서 페이지](https://docs.blender.org/manual/en/2.79/advanced/command_line/introduction.html#console-window-status-and-error-messages)의 단계를 따르십시오. 콘솔 출력은 텍스처가 로드되지 않거나 재료가 처리 중에 멈춰 있는 등 예기치 않은 문제가 발생할 때 유용할 수 있습니다.

버그를 보고하려면 [Substance 디스코드 서버](https://discord.com/invite/substance3d)에서 #substance-blender-beta 채널에 가입하거나 [Adobe 커뮤니티](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender)를 방문하세요. 콘솔 로그의 관련 정보와 문제에 대한 복제 단계를 보고서에 포함할 수 있습니다.

## 일반적인 문제 및 해결 방법

* *WMIC 관련 콘솔 오류*
  * *경우에 따라 Windows 설치에는 WMIC가 포함되지 않습니다. 이 경우 필요합니다. 이 문제를 수동으로 해결하는 방법은 다음과 같습니다.*
    * 설정 - 시스템 - 선택적 기능으로 이동합니다.
    * &quot;기능 보기&quot;를 선택한 다음 &quot; 옵션 기능 추가&quot;를 선택합니다.
    * 그러면 새 창이 나타나며 목록을 아래로 스크롤하여 WMIC를 찾고 확인란을 선택한 후 다음 을 누르고 다음 창에서 추가 를 누릅니다.
    * 이제 최근 작업에서 WMIC 설치 진행률을 보여 주는 새 창으로 이동합니다.
    * *다운로드하는 데 몇 분 정도 걸릴 수 있습니다. 그런 다음 컴퓨터를 재설정하고 Blender와 추가 기능을 다시 시작합니다. Substance 3D 패널에서 로드를 클릭하면 이제 파일 브라우저 창이 표시됩니다.*
  * 그래도 문제가 해결되지 않으면 PATH 변수에 WMIC를 정의해야 할 수도 있습니다. 특정 버전의 Windows에 대한 설명서를 참조하십시오.
* *추가 기능을 업데이트하고 재질을 로드한 후에는 일부 설정이 Substance 3D 패널에 나타나지 않습니다.*
  * 이 문제는 이전 파일이 시스템에 계속 캐시될 수 있기 때문에 추가 기능의 이전 버전을 제거하고 동일한 세션에 최신 버전을 설치할 때 발생할 수 있습니다.\
    Blender를 다시 시작하면 변경 내용이 적용됩니다.
* *추가 기능을 설치할 때 문제가 발생했습니다./ 세션 간에 자료가 처리되지 않습니다. / 재질은 세션 간에 텍스처를 생성하지 않습니다. / .sbsar 파일을 로드하는 동안 오류가 발생했습니다.*
  * 이 문제는 통합 도구 설치 시 발생할 수 있으며 일반적으로 도구를 수동으로 제거하여 해결합니다. 수동 제거 지침을 보려면 [추가 기능 제거](../../../3d-applications/blender/uninstalling-the-add-on/uninstalling-the-add-on.md) 페이지를 방문하세요.
* *순환 렌더링 보기에서 재질이 업데이트되지 않음*.
  * 기본적으로 추가 기능은 주기 렌더링 보기에서 텍스처를 업데이트하지 않습니다. 그러나 추가 기능 환경 설정에서 <b>주기 자동 업데이트 텍스처</b>을 활성화하여 해당 프로필을 강제로 업데이트할 수 있습니다.
* 사이클 렌더링 보기에서 저장하는 동안 매개 변수가 되돌아갑니다.
  * 이것은 시각적 전용인 블렌더 측에서의 알려진 캐싱 문제입니다. 저장할 때, 생성된 텍스처 파일을 업데이트하기 위해 원격 엔진으로 메시지가 전송되지 않습니다. 텍스처는 사이클 렌더링 보기에서 벗어나 다시 전환하면 정상적으로 표시됩니다.
* *매개 변수를 실행 취소/변경한 후에는 재질이 더 이상 업데이트되지 않습니다.*
  * 작업을 취소한 후 재질이 업데이트되지 않을 수 있습니다. 매개 변수는 이전 상태로 되돌아가지만, 텍스처는 일치하도록 실행 취소되지 않습니다. 텍스처를 다시 업데이트하려면 새로 고침 단추를 사용하여 매개 변수를 기본값으로 되돌리고 텍스처를 다시 로드합니다.
* *Substance Designer에서 설정한 색상이 Blender의 색상 피커에서 약간 다르게 나타나며 색상 값이 동일하지 않습니다.*
  * Blender는 Blender 색상 피커의 색상에만 감마 교정을 적용합니다. 이로 인해 색상 피커가 일치하지 않지만 Substance에 나타나는 색상은 텍스처 앱에 설정된 값에 정확합니다.
* Windows에서 자료를 로드할 때 *&quot;wmic가 인식되지 않음&quot; 콘솔 오류가 발생합니다.*
  * 이 문제는 C:\Windows\System32\wbem\ 이 PATH 시스템 변수에 포함되어 있지 않을 때 발생합니다. 특정 버전의 Windows에 대한 설명서를 참조하십시오.
* Mac에서 *&quot;잘못된 CPU 유형이 실행 가능합니다&quot; 오류가 발생했습니다.*
  * 이 문제는 ARM Mac 컴퓨터에서 Rosetta가 활성화되지 않은 경우 발생합니다. 자세한 내용은 [Apple의 Rosetta 페이지](https://support.apple.com/en-us/102527)를 참조하세요. 또한 자세한 지침은 이 [설치 안내서](https://medium.com/@jithmisha/fix-for-macbook-air-m1-m2-bad-cpu-type-in-executable-error-3719a0a1cb6)를 참조하세요.
* *새로 고침 단추를 사용하거나 매개 변수를 업데이트할 때 셰이더 그래프에 대한 수정 작업이 실행 취소됩니다.*
  * 추가 기능은 변경 또는 새로 고침 후 그래프의 연결을 새로 고쳤습니다. 이 문제를 해결하려면 .sbsar에서 만든 블렌더 재질을 복제하고 원하는 새 이름을 지정합니다. 복제에 노드만 추가합니다. 텍스처는 사용자가 추가한 노드를 유지하면서 노드 그룹에서 업데이트됩니다. 새로 고치는 경우 이러한 노드를 복사한 후 새로 고침 후 새 그래프에 다시 붙여넣습니다.
