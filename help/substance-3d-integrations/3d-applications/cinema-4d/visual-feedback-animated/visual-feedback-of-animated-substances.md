---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/visual-feedback-of-animated-substances.html"
breadcrumb-title: ''
description: Cinema 4D에서 애니메이션 미리 보기를 활성화하여 뷰포트에서 애니메이션 Substance 재질에 대한 시각적 피드백을 확인할 수 있습니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Visual Feedback of Animated Substances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 애니메이션 Substance에 대한 시각적 피드백
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 3%

---


# 애니메이션 Substance에 대한 시각적 피드백

Cinema 4D 뷰포트에서 애니메이션 Substance을 시각적으로 피드백하려면 해당 재질에 대해 애니메이션 미리 보기 옵션을 활성화해야 합니다.

이 옵션은 [재질 편집기] 아래의 [편집기] (아래 참조)에서 찾을 수 있습니다. 재료 생성(Create Material(s)) 명령을 사용하여 재료를 생성한 경우에는 이 옵션이 기본적으로 활성화됩니다.

![](../../../assets/cinema-4d-13.png){width="500px"}


## 재료 생성

Substance Asset Manager의 재질 만들기 명령을 사용하면 Substance을 사용하여 Cinema 4D 재질을 쉽고 빠르게 만들 수 있습니다.

따라서 다음 채널 매핑이 사용됩니다.

|  |  |
| --- | --- |
| **Substance 출력 채널** | **Cinema 4D 재질 채널** |
| 확산 | 색상 |
| 배출 | 광도 |
| 반사 | 반사도 |
| 환경 | 환경 |
| 범프 | 범프 |
| 불투명도 | 알파 |
| 반사 | 반사도/기본 Specular |
| 높이 | 변위 |
| 표준 | 표준 |

이 관계식은 재료 생성(Create Material(s)) 명령에만 사용되며 생성된 재료를 나중에 수정할 수 있습니다. 이 명령을 사용하여 기본 재질을 빠르게 만든 다음 일부 채널만 수정하여 세부 조정할 수 있습니다.

Substance 셰이더 내에서는 위에 나열된 몇 가지 출력 채널로 제한되지 않지만 실제로 Substance에서 제공할 수 있는 모든 출력 채널을 사용할 수 있습니다.

## 수동으로 Substance 재료 생성

[재질 만들기] 명령을 사용하는 대신 Substance 셰이더를 사용하여 재질을 수동으로 만들 수도 있습니다.

재질 채널에서 Substance 셰이더를 선택하고 사용할 Substance을 드래그하기만 하면 됩니다. 다음 단계는 이 셰이더에 사용할 Substance의 출력 채널을 선택하는 것입니다.

다음과 같이 표시됩니다.

![](../../../assets/cinema-4d-15.png){width="800px"}

이 방법을 사용하면 창의력을 마음껏 발휘할 수 있으며, 다음 작업을 수행할 수 있습니다.

* Substance 출력 채널을 임의의 Cinema 4D 재질 채널에 할당합니다. 의도한 채널에서만 사용하도록 제한할 필요는 없습니다.
* 단일 Substance 출력 채널을 여러 Cinema 4D 재질 채널에 할당합니다.
* 여러 Substance의 출력 채널을 단일 Cinema 4D 자료에 할당합니다.

## 제한 사항

* Substance 입력 매개 변수의 키프레임은 타임라인에 표시되지만 Cinema 4D의 [파워] 슬라이더(뷰포트 아래의 [타임라인] 슬라이더)에는 표시되지 않습니다.
* 제한 사항으로 인해 Substance 출력 채널에는 사용자 정의 색상 프로필을 사용하지 않아야 합니다.
* 특정 상황에서는 Substance의 이미지 입력이 중단됩니다.\
  두 장면을 하나로 결합하는 Cinema 4D 병합... 명령. 이는 병합할 장면에 프로젝트 디렉터리의 이미지를 참조하는 이미지 입력이 있는 프로젝트 디렉터리에 Substance이 있는 경우 발생합니다. 이러한 경우, 이미지 입력은 이후에 수동으로 다시 연결되어야 할 것이다.
* Substance이 프로젝트 폴더(또는 전역 검색 경로 내 다른 위치)에 있는 경우에는 Cineware에서 작동하지 않습니다. 이 경우 Substance이 누락된 것처럼 빨간색으로 렌더링됩니다. 이 문제를 해결하려면 Substance 아카이브를 프로젝트 디렉토리 외부에 저장해야 하므로 절대 경로에서 참조합니다. 파일을 프로젝트 경로 외부로 이동한 후 Filename 매개 변수를 사용하여 파일 위치를 변경할 수 있습니다.
