---
helpx_url: 'https://helpx.adobe.com/substance-3d-general/ecosystem/general-system-requirements.html'
breadcrumb-title: ''
description: Substance 3D 애플리케이션의 시스템 요구 사항을 확인하여 하드웨어가 최소, 권장 또는 최적의 사양을 충족하는지 확인하십시오.
helpx_creative_field: ''
helpx_description: General Knowledge > Ecosystem > General system requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 일반 시스템 요구 사항
user-guide-description: ''
user-guide-title: ''
source-git-commit: eef3d78f33034f2c24f4c4471d9ccac805184525
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 2%
---

# 일반 시스템 요구 사항

## 하드웨어 요구 사항

+++Windows

|  | 최소 | 권장 | 최적 |
| --- | --- | --- | --- |
| **OS** | Windows 11 64비트 버전 23H2 | Windows 11 64비트 버전 24H1 | Windows 11 64비트 버전 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8GB | 16GB | 24GB |
| **RAM** | 16GB | 32GB | 64GB |
| **저장소** | 30GB의 사용 가능한 공간이 있는 SSD | 50GB의 사용 가능한 공간이 있는 SSD | 70GB의 사용 가능한 공간이 있는 SSD |

+++

+++macOS

|  | 최소 | 권장 | 최적 |
| --- | --- | --- | --- |
| **OS** | macOS 세쿼이아 | macOS 골든 게이트 | macOS 골든 게이트 |
| **CPU** | Apple | Apple | Apple M4 Pro |
| **GPU** | Apple | Apple | Apple M4 Pro |
| **RAM** | 16GB | 32GB | 64GB |
| **저장소** | 30GB의 사용 가능한 공간이 있는 SSD | 50GB의 사용 가능한 공간이 있는 SSD | 70GB의 사용 가능한 공간이 있는 SSD |

>[!WARNING]
>
> [VFX 참조 플랫폼](https://vfxplatform.com/)을(를) 염두에 두고 빌드된 파이프라인의 경우 Substance 3D 응용 프로그램은 macOS 14 Sonoma에 계속 설치할 수 있습니다. 그러나 최소 시스템 요구 사항 미만의 OS 버전에서는 Substance 앱을 더 이상 테스트하지 않으므로 안정성이 보장되지 않습니다. 최신 OS 버전으로 업데이트하는 것이 좋습니다.

+++

+++리눅스

|  | 최소 | 권장 | 최적 |
| --- | --- | --- | --- |
| **OS** | **기업 ETLA** RHEL 8.6 이상 또는 RHEL 9.2 이상 **Steam** Ubuntu 22.04.1 LTS | **기업 ETLA** RHEL 8.6 이상 또는 RHEL 9.4 이상 **Steam** Ubuntu 22.04.1 LTS 이상 | **기업 ETLA** RHEL 8.6 이상 또는 RHEL 9.4 이상 **Steam** Ubuntu 22.04.1 LTS 이상 |

**RHEL(Red Hat Enterprise Linux) 9.x**: 애플리케이션에 필요한 xcb-util-cursor 패키지가 2024년 5월 10일에 EPEL 9 저장소에서 제거되었습니다. 이 날짜부터 패키지는 RHEL 9.4 릴리스와 함께 기본 RHEL 9 저장소에서 지원됩니다. 9.4 이전 버전의 RHEL을 사용하는 고객은 2024년 5월 10일 이후에는 더 이상 EPEL 9 저장소에서 xcb-util-cursor 패키지를 소싱할 수 없습니다.

기본 RHEL 9 리포지토리에서 이 패키지의 가용성에 대한 자세한 내용은 [Red Hat Enterprise Linux 9 - 패키지 매니페스트 - AppStream 리포지토리](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/9/html-single/package_manifest/index#AppStream-repository)를 참조하십시오.

이 변경에 대한 자세한 내용은 다음을 참조하십시오. [Red Hat Bugzilla - Bug 2238273](https://bugzilla.redhat.com/show_bug.cgi?id=2238273) , [Red Hat Bugzilla - Bug 2212302](https://bugzilla.redhat.com/show_bug.cgi?id=2212302)

+++

+++VR

| 브랜드 | 모델 |
| --- | --- |
| 메타 | Rift, Rift S, Quest, Quest 2 (Link 포함), Quest Pro |

+++

자세한 내용은 각 애플리케이션의 요구 사항을 살펴보십시오.

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/sa-appicon-noshadow-256.png" alt="Substance 3D Sampler 아이콘" width="64px"/><br><a href="https://experienceleague.adobe.com/en/docs/substance-3d-sampler/using/getting-started/system-requirements">Substance 3D Sampler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/ds-appicon-noshadow-256.png" alt="Substance 3D Designer 아이콘" width="64px"/><br><a href="https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/getting-started/system-requirements">Substance 3D</a> <a href="https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/getting-started/system-requirements">Designer</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/pt-appicon-noshadow-256.png" alt="Substance 3D Painter 아이콘" width="64px"/><br><a href="https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/system-requirements">Substance 3D Painter</a></td>
  </tr>
</table>

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/md-appicon-noshadow-256.png" alt="Substance 3D Modeler 아이콘" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-modeler/getting-started/system-requirements.html">Substance 3D Modeler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/sg-appicon-noshadow-256.png" alt="Substance 3D Stager 아이콘" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-stager/getting-started/system-requirements.html">Substance 3D Stager</a></td>
    <td style="border: 0;" valign="top"></td>
  </tr>
</table>

## 추가 정보

### 지원되지 않는 구성

* eGPU 및 사용자가 설치한 GPU가 있는 Apple 컴퓨터 구성은 지원되지 않습니다.
* Windows 가상 컴퓨터는 지원되지 않습니다.
* Windows Server 운영 체제가 지원되지 않습니다.
