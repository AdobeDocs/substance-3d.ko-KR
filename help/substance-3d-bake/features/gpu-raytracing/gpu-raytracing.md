---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/gpu-raytracing.html"
breadcrumb-title: ''
description: 하드웨어 가속 GPU 광선 추적을 활성화하여 더 빠른 워크플로우를 위해 베이킹 계산 속도를 25배 이상 높입니다.
helpx_creative_field: ""
helpx_description: bakers > Features > GPU Raytracing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU 광선 추적
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 18%

---


# GPU 광선 추적

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

일부 베이커는 GPU에서 광선 추적의 하드웨어 가속을 지원하는데, 이는 일반적으로 25배 이상의 계산 속도를 증가시킵니다.

## 하드웨어 요구 사항

시스템이 다음 요구 사항을 충족하면 광선 추적이 자동으로 활성화됩니다.

* 호환 가능한 GPU가 설치됩니다.\* (RTX 시리즈, Titan V 또는 GeForce 10xx)
* GPU 드라이버가 최신 상태입니다.
* Windows 10 &#39;Fall Creator&#39; / 10월 업데이트(버전 1809) 이상이 설치되었습니다.\*\*

</td>
<td style="border: 0;" valign="top">

![GPU 광선 추적 켜기/끄기 비교](../../assets/rtx-ao-demo.gif "GPU 광선 추적 켜기/끄기 비교"){zoomable="yes"}

</td>
</tr>
</table>

\*: 호환되는 NVIDIA GPU에는 Pascal 아키텍처 이상의 최신 버전을 사용하는 모든 GPU가 포함됩니다. 즉, GTX 10 시리즈, Titan V 시리즈, RTX 20 시리즈 또는 그 이상의 최근.

\*\*: Windows 버전을 확인하려면 [시작] 메뉴를 클릭하고 &#39;winver&#39;를 입력한 다음 Enter 키를 누릅니다.\
Microsoft 지원 웹 사이트의 [전용 페이지](https://support.microsoft.com/en-us/help/4028685/windows-10-get-the-update)를 통해 업데이트를 받을 수 있습니다.

>[!TIP]
>
> 문제가 발생하는 경우 애플리케이션 환경 설정에서 GPU 광선 추적을 비활성화할 수 있습니다.

## 지원되는 제빵사

Substance 3D 제빵사 버전에 따라, 아래 표에는 모든 제빵사에 대한 GPU 광선 추적 지원이 나열되어 있습니다.

+++버전 3 이상

| 베이커 | GPU 광선 추적 지원 |
| --- | --- |
| 주변 폐색 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 노멀 구부리기 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 색상 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 곡선 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 높이 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 표준 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 노멀 월드 공간 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |



| 베이커 | GPU 광선 추적 지원 |
| --- | --- |
| 불투명 마스크 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 위치 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 낮은 위치 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 두께 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 전송된 텍스처 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 월드에서 탄젠트로 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |


+++

+++버전 2

| 베이커 | GPU 광선 추적 지원 |
| --- | --- |
| 주변 폐색 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 메시 기준 앰비언트 오클루전 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 메시 기준 벤트 노멀 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 메시 기준 색상 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| UV를 SVG로 전환 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 메시 기준 곡률 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 메시 기준 높이 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 메시 기준 노멀 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |



| 베이커 | GPU 광선 추적 지원 |
| --- | --- |
| 메쉬의 불투명 마스크 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 메시 기준 위치 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 위치 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 메시 기준 두께 | <div><img alt="(틱)" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 메시에서 전달된 텍스처 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 세계 우주 방향 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 세계 우주 표준 | <div><img alt="(오류)" data-preserve-html="true" src="../../assets/error.svg"/></div> |


\*: GPU 광선 추적 속도가 훨씬 느린 CPU 광선 추적을 지원합니다.

+++
