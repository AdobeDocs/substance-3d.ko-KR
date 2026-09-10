---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-integrations/3d-applications/blender/workflows.html"
breadcrumb-title: ''
description: 다양한 워크플로우에 대해 블렌더의 주기 및 이벤트 렌더러에서 Substance 재질을 사용하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 워크플로
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---


# 워크플로

## 사이클 작업

기본적으로, 주기 렌더링 보기에서 볼 때 매개 변수 변경 내용이 3D 뷰포트에서 자동으로 업데이트되지 않습니다. 주기 렌더링 보기에서 업데이트를 보려면 [환경 설정]에서 **주기 자동 업데이트 텍스처**&#x200B;을(를) 활성화하여 강제로 업데이트합니다.

## 멀티그래프 .sbsar 파일

추가 기능은 여러 Substance 그래프가 있는 .sbrar 파일을 지원합니다. 여러 그래프가 있는 파일을 로드하면 Substance 3D 패널에 새로운 그래프 드롭다운이 나타납니다. 다른 매개변수 변경과 달리 그래프를 전환하면 재료가 자동으로 업데이트되지 않습니다. 따라서 그래프를 변경한 후 재질을 다시 할당하려면 **적용** 단추를 사용해야 합니다.

>[!NOTE]
>
> 기본적으로 [적용] 단추는 이전 재료 지정을 무시하지 않고 새 슬롯에 재료를 추가합니다. 이전 재질을 제거하거나 재질 드롭다운을 사용하여 새로 적용된 재질을 다시 할당합니다.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/blender-workflows-multigraphs?$png$&jpegSize=100&wid=168)

## 이미지 입력 작업

사용자 정의 이미지 입력을 허용하는 Substance 재질을 사용하는 경우, 이미지 선택 매개 변수 Substance 3D 패널을 사용하여 이미지 파일 브라우저(폴더 아이콘)를 열거나 프로젝트에 있는 이미지(이미지 아이콘 드롭다운)에서 선택할 수 있습니다.

이미지 형식 내보내기 환경 설정을 사용하여 Blender 내에서 생성된 이미지 입력을 임시 폴더에 저장할 수 있습니다. 자세한 내용은 [환경 설정](../../../3d-applications/blender/preferences/preferences.md)페이지를 참조하세요.

![](../../../assets/blender-workflows-image-inputs-steps.png)

## 셰이더 네트워크 사전 설정.

Substance 3D 패널의 출력 섹션에 있는 드롭다운을 통해 셰이더 사전 설정을 빠르게 조정할 수 있습니다. 이러한 셰이더 사전 설정은 이미지 텍스처가 적용되는 방법을 조정합니다. Cycles/Evee Standard는 일반 UV 텍스처 좌표 매핑을 사용합니다. 다른 세 개의 주기/깊이 투영 사전 설정은 상자, 구 또는 원통 투영 방법에 대해 생성된 텍스처 좌표 매핑을 사용합니다.

재질에 사용되는 기본 셰이더 사전 설정은 추가 기능 [환경 설정](../../../3d-applications/blender/preferences/preferences.md)에서 선택할 수 있습니다.

![](../../../assets/2022-08-12-12-12-33-adobeexpress-1.gif)

## 출력 필터링 및 조정

Substance 3D 패널의 출력 섹션에도 출력을 필터링하는 옵션이 있습니다. 셰이더 사전 설정 드롭다운 옆에 있는 세 개의 버튼을 사용하여 활성화된 출력(체크 마크), 셰이더 출력(구) 및 사용 가능한 모든 출력(선)별로 필터링할 수 있습니다.

확인란에 따라 출력을 개별적으로 활성화할 수 있습니다. 출력이 활성화되면 텍스처 노드 그룹의 해당 출력이 생성됩니다. 해당 출력이 Principled BSDF 재질 노드에서 지원되면 자동으로 연결됩니다. Height이 변위 노드에 연결되고 앰비언트 오클루전이 MixRGB 노드의 기본 색상과 결합됩니다.\
확인 표시 옆의 파일 형식 드롭다운을 사용하여 출력 텍스처를 저장할 파일 형식을 설정할 수 있습니다.

또한 추가 기능 [환경 설정](../../../3d-applications/blender/preferences/preferences.md)에서 기본 파일 출력 환경 설정을 변경할 수 있습니다.

## 개체의 재질 교체

블렌더의 재질 속성 패널에서 구 아이콘을 클릭하여 블렌더의 재질 목록을 엽니다. 패널에서 만든 Substance 재질이 목록에도 표시됩니다. 이 목록에서 재료를 선택하면 해당 재료 슬롯의 활성 재료가 대체됩니다.

## 변위

[텍스처] 렌더러에서는 지원되지만 Evee에서는 지원되지 않는 시퀀스의 메시 변위. 변위를 보려면 Height 출력이 활성화되어 있는지 확인합니다. 추가 기능은 재질의 변위 설정을 **변위 및 범프**&#x200B;로 자동으로 설정합니다. 이제 오브젝트에서 재질을 보면 렌더링 보기에 변위가 표시됩니다. 변위 비율은 재질 패널 또는 변위 노드에서 조정할 수 있습니다.

최상의 결과를 얻으려면 복잡한 변위 세부 묘사가 있는 재질에 대해 더 높은 서브디비전 수준 또는 높은 폴리 메쉬를 사용합니다.
