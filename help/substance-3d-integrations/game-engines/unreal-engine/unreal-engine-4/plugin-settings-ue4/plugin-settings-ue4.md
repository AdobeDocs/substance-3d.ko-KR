---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/plugin-settings-ue4.html"
breadcrumb-title: ''
description: Unreal Engine 4에서 프로젝트 설정을 통해 Substance 플러그인 설정을 구성하여 플러그인 동작을 사용자 정의합니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Plugin Settings - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 플러그인 설정 - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---


# 플러그인 설정 - UE4

설정에 액세스하려면 편집>프로젝트 설정으로 이동하고 Substance 범주로 스크롤하여 플러그인을 클릭합니다.

![](../../../../assets/settings-36.png){width="400px"}

## 하드웨어 예산

메모리 예산은 Substance 엔진에 사용할 최대 메모리 양입니다. Substance 처리 속도를 높이기 위해 늘릴 수 있지만 시스템 리소스를 더 많이 소비합니다. ( 프로젝트 수준에서 증가하면 항상 도움이 되는 것은 아닙니다.)

CPU 코어는 Substance 엔진에서 사용하도록 허용된 코어 수입니다. 여기에는 물리적 코어와 하이퍼 스레드가 모두 포함됩니다. 할당된 수가 시스템에서 사용 가능한 코어보다 크면 기본적으로 사용 가능한 모든 코어를 사용합니다.

## 요리

요리하는 동안 제거된 Mip 레벨 수는 패키지에 대한 텍스처가 생성되는 방법을 변경합니다. 이 설정은 더 큰 텍스처 mip 수준을 더 이상 로드할 필요가 없으므로 로드 시간을 크게 개선하고 패키지 크기를 줄일 수 있습니다. 낮은 해상도/작은 LOD가 로드되고 가장 높은 해상도는 UE4에 의해 기본값으로 설정됩니다. 물질은 그런 다음 Substance 엔진을 통해 처리되고 고해상도 LOD로 런타임에 업데이트됩니다.

Substance 엔진은 CPU 또는 GPU일 수 있습니다. GPU 엔진을 사용하여 4K 텍스처를 만들 수 있습니다. CPU 엔진이 2K로 제한됩니다.

## 기본 생성:

SGM(Substance 생성 모드)은 텍스처가 생성되는 방식을 제어합니다. Substance에 대한 전역 설정입니다. SGM은 Substance 팩토리에서 Substance 단위로 변경할 수 있습니다.

**SGM Baked**: Substance 텍스처를 만듭니다. 런타임에 매개 변수를 변경하는 기능을 사용하지 않습니다.

**로드 동기화 시 SGM**: Substance을 로드하는 동안 응용 프로그램을 차단합니다.

**부하 동기화 및 캐시 시 SGM**: 디스크의 텍스처의 중간 결과를 캐시합니다.

**부하 비동기 SGM**: 비차단. Substance은 백그라운드에서 생성됩니다.

**비동기 및 캐시 로드의 SGM**: 디스크의 텍스처의 중간 결과를 캐시합니다.

***플랫폼 기본값은 비동기 로드 및 캐시***&#x200B;입니다.

## Substance 팩토리

Substance에 대한 SGM을 변경하려면 속성 매트릭스를 통해 Substance 팩토리 > 자산 작업 > 일괄 편집을 마우스 오른쪽 버튼으로 클릭합니다. 그런 다음 SGM을 변경할 수 있습니다.

![](../../../../assets/sgm.png){width="800px"}

## 최적화:

이렇게 하면 각 일괄 처리에 대해 Substance 엔진에 전달할 수 있는 비동기 물질의 수가 제한됩니다. 숫자가 낮을수록 비동기 작업이 완료되는 속도가 빨라지고 숫자가 높을수록 한 번에 여러 Substance를 일괄 렌더링하고 처리하는 업데이트 속도가 높아집니다. 값이 높을수록 업데이트 사이의 시간이 길어져 텍스처 업데이트가 고르지 않게 됩니다.

## 비동기/동기화 렌더링

동기화 렌더링은 차단 렌더링 호출입니다. 이렇게 하면 Substance Graph 인스턴스가 다시 계산되는 Substance 엔진에 전달되지만 Substance 엔진이 Substance 처리를 마칠 때까지 실행이 중지된 후 추가 코드 실행이 계속됩니다. 프로세스가 완료되는 즉시 화면에 결과도 업데이트됩니다.

Async는 플러그인을 업데이트할 때 그래프를 대기열에 추가하고 Substance 설정 내에서 설정된 한 번에 여러 그래프를 Substance 엔진에 보냅니다. 동기화 렌더링과 달리 프로그램은 전송 즉시 Substance 엔진이 완료될 때까지 대기하지 않고 평소처럼 계속 실행됩니다. Substance Engine에서 일괄 처리를 완료하면 결과가 다시 전송되어 출력물에 적용되고 다른 일괄 처리를 시작합니다.
