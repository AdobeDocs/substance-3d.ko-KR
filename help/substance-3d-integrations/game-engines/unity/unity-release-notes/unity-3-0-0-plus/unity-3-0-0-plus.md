---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-3-0-0-plus.html"
breadcrumb-title: ''
description: Unity 플러그인 버전 3.0.0 이상의 릴리스 노트를 검토하여 새로운 기능 및 개선 사항에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 유니티 .
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---


# Unity 3.0.0+

## 유니티 .

<b>추가/업데이트:</b>

* Unity에서 Substance 3D 커넥터 지원, Substance 3D Sampler과 Unity 간에 에셋을 전송하기 위한 SendTo 기능 활성화
* 업데이트된 그래프를 Unity 플러그인으로 다시 가져올 때 Designer에서 변경된 사항이 유지되도록 Designer에서 Unity로 .sbsar 그래프의 이름을 바꾸고 다시 게시할 수 있습니다.
* Unity 프로젝트 간에 .sbsar 파일을 공유하는 방법에 대한 설명서입니다.
* Unity 플러그인 설명서 커뮤니티 기여도 페이지: https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/community-contributions.html.

<b>고정:</b>

* .sbsar 파일을 다시 게시하고 현재 파일 대신 이전 재질을 표시한 후 Unity 프로젝트 에셋 폴더의 재질 미니어처가 업데이트되지 않는 문제가 있습니다.

## 유니티 .

<b>추가/업데이트:</b>

* 1000개 이상의 Substance 그래프로 프로젝트의 성능을 개선하여 Assets 폴더에서 sbsar 파일을 검사할 때 UI 응답 시간을 크게 줄였습니다.
* sbsar 파일을 원래 상태로 되돌리는 재설정 버튼을 추가하여 워크플로 효율성을 향상했습니다.
* [Substance 3D Integrations in Unity - Upgrading Projects &amp; Known Issues](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md)에서 사용할 수 있는 &quot;이미지 입력이 8비트로 잠겨 있습니다&quot; 문제에 대한 해결 방법이 포함된 문서가 업데이트되었습니다.
* Unity에서 패널 폴더를 탐색할 때 발생하는 &quot;식에서 어설션 실패&quot; 오류를 해결하기 위해 설명서가 업데이트되었습니다. [Unity의 Substance 3D 통합 - 프로젝트 및 알려진 문제 업그레이드](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md).

<b>고정:</b>

* Linux 플랫폼에서 플러그인이 중단되는 문제를 해결했습니다.
* 버전 2023의 Unity 플러그인에서 발생하는 호환성 문제가 해결되었습니다.

## 유니티 .

<b>고정:</b>

* Unity용 Substance 3D 플러그인의 sbsario.dll 문제로 인해 Substance 엔진을 로드하지 못했던 문제를 수정했습니다.

## 유니티 .

<b>추가/업데이트:</b>

* 플러그인의 RenderInstanceAsync API에 대한 주석 섹션을 업데이트했습니다.

<b>고정:</b>

* 플러그인의 C++ 코드에서 메모리 누수 문제를 해결하여 개체를 폐기할 때 완벽한 메모리 복구를 보장합니다.
* Linux에서 Unity 플러그인 패키지를 가져올 때 &#39;SubstanceException: API에 잘못된 인수가 제공됨&#39; 오류가 발생하는 문제를 수정하여 이제 SBSAR 파일을 성공적으로 가져올 수 있습니다.
* Unity에서 사용자 정의 편집기 창 스크립트를 사용하여 사전 설정을 로드할 때 SubstanceGraphSO.CurrentStatePreset이 올바르게 작동하지 않던 문제가 해결되었습니다. 이제 Substance 설명서(HelpX) 페이지에서 수정 스크립트를 사용할 수 있습니다. https://experienceleague.adobe.com/en/docs/substance-3d/ecosystem/game-engines/unity/substance-3d-for-unity-scripting/substance-3d-for-unity-scripting
* 유니티 편집기에서 다시 선택할 때 그래프 속성이 사라지는 버그가 수정되었습니다.
* Unity 플러그인에서 SubstanceGraphSO와 관련된 &#39;알 수 없는 관리 유형 참조&#39; 문제를 해결하여 특히 Unity 2022.1 및 모든 Unity 버전에서 Android 플랫폼의 호환성과 기능을 개선했습니다.
* DirectX 및 OpenGL 옵션이 있는 예상 드롭다운 목록이 아닌 TECHNICAL PARAMETERS 섹션의 &#39;NORMAL FORMAT&#39; 선택 항목이 숫자 입력 필드로 잘못 표시되는 문제를 수정했습니다.

## 유니티 .

<b>추가/업데이트:</b>

* 이제 Sbsar 파일을 프로젝트로 드래그하여 놓을 수 있습니다. .sbsar 개체는 Unity 2022.3에서 예상대로 메시에 적용할 수 있습니다.
* 플러그인에 대한 향상된 설명서.

<b>고정:</b>

* Android에서 Unity 플러그인이 작동하지 않던 문제가
* Unity 플러그인의 이름 지정 제약 조건을 해결했습니다. 파일 이름에 &quot;.&quot;가 포함된 경우 플러그인이 파일을 올바르게 로드하지 않았습니다.
* &quot;모든 출력 생성&quot;을 선택 취소해도 추가 텍스처가 자동으로 삭제되지 않는 문제를 해결했습니다.
* Unity 2021.3 표준 프로젝트에서 SBSAR 재질을 잘못 가져온 문제를 수정했습니다. 이제 표준 템플릿 프로젝트에서 SBSAR 재질을 에셋 폴더로 가져와 오류 없이 3D 메시에 적용할 수 있습니다.
* Unity 2021/2022 HDRP 프로젝트에서 SBSAR 재질을 잘못 가져온 문제를 수정했습니다. 이제 HDRP 템플릿 프로젝트에서 SBSAR 재질을 에셋 폴더로 가져와 오류 없이 3D 메시에 적용할 수 있습니다.
* APK를 생성하기 위해 Android 빌드를 생성할 때 컴파일 오류가 발생하는 문제를 수정했습니다. &quot;컴파일에 실패했습니다. 자세한 내용은 컴파일러 오류 출력을 참조하십시오.&quot;
* Windows에서 빌드 프로젝트 프로세스가 실패하고 오류가 발생하는 문제를 해결했습니다.
* Android:UnityEditor.BuildPlayerWindow+BuildMethodException에서 빌드 프로젝트 프로세스가 오류와 함께 실패하는 문제를 해결했습니다.
* 런타임에 SubstanceGraph 입력을 변경할 때 발생하는 UnityException을 해결했습니다. 이전에는 SubstanceRuntimeGraph.SetTexturesResolution 및 SubstanceRuntimeGraph.Render()를 호출하여 SubstanceGraph가 잘못된 결과를 렌더링하도록 했습니다.
* SubstanceEditorTools.cs의 입력 오류를 수정했습니다.

## 유니티 .

<b>추가/업데이트:</b>

* 조건부 가시성(Visible If 기능)이 있는 매개 변수에 대한 지원이 도입되었습니다.
* Substance 엔진을 버전 9로 업그레이드했습니다.
* 사용자 지정 편집기 창 스크립트에서 NativeGraph.InRenderWork가 작동하지 않는 문제를 해결하기 위해 문서가 업데이트되었습니다. 자세한 내용은 여기에서 확인할 수 있습니다. [Unity 스크립팅용 Substance 3D - 클래스 문서](../../../../game-engines/unity/3d-for-unity-scripting/class-documentation/substanceruntime-class/substanceruntime-class.md)

<b>고정:</b>

* Android 프로젝트의 노멀 맵에 영향을 주는 문제를 해결했습니다.
* sbsar 개체를 장면 보기로 드래그하면 실수로 모든 마우스 오버 개체의 재질이 sbsar 개체 재질에 의해 재정의되게 되는 버그가 해결되었습니다.
* [런타임] 모드에서 [런타임만]으로 표시된 재질을 검사하고 [출력 텍스처 매핑]을 열 때 오류가 발생하는 버그를 해결했습니다.

## 유니티 .

<b>추가/업데이트:</b>

* 포함 및 외부 사전 설정 지원
* Unity 2022.2와 호환

<b>고정:</b>

* 그래프 복사 버튼을 사용하여 sbsar 파일에 대한 새 그래프를 생성하는 동안 오류가 발생했습니다. &quot;스크립팅된 클래스의 예기치 않은 재귀 전송&quot;
* 프로젝트를 다시 연 후 Mac에서 추가 재질 폴더 생성
* 그래프 인스턴스를 생성/삭제할 때 SubstanceFileSO 배열이 업데이트되지 않음
* Substance 복제 시 잘못된 입력 옵션이 표시됨
* .sbsprs 파일 내보내기의 빈 레이블 필드
* 편집기에서 사전 설정 내보내기/가져오기 중 오류 발생: EndLayoutGroup: BeginLayoutGroup을 먼저 호출해야 합니다.

<b>제거됨:</b>

* 사용자 값 부족으로 인한 Unity 플러그인의 채널 섹션

## 유니티 .

<b>추가/업데이트:</b>

* 개별 Int 4 값을 독립적으로 편집 가능하게 만드는 기능.

<b>고정:</b>

* 프로젝트를 다시 열 때 재질이 이전 상태로 되돌아가는 문제
* 재질 그래프를 수정하려고 할 때 &quot;그래프를 찾을 수 없습니다&quot;라는 메시지가 표시되는 오류
* 물리적 크기 기능의 [회전 오프셋] 매개 변수에 대한 입력 값이 변경되지 않는 문제
* 복제된 그래프 인스턴스에서 입력에 대한 GraphID 값이 잘못된 문제를 발견하였습니다.
* Substance 스크립트(사용자 정의 편집기 창)를 사용하여 그래프를 변경하는 동안 편집기 생성기가 제대로 초기화되지 않는 문제가 발생했습니다
* 사용자 정의 편집기 창 스크립트에서 SubstanceGraphSO.CurrentStatePreset을 내보낼 때 캐시된 버전의 그래프가 내보내지는 문제
* 검사기 창이 잠겨 있을 때 매개 변수 변경 내용이 저장되지 않는 문제
* [물리적 크기] 옵션의 [위치 오프셋] 섹션에 있는 수동 키보드 입력이 [편집기] 모드의 재질에 영향을 주지 않는 문제가
* SBSAR 개체에 매개 변수 값을 수동으로 입력할 때 오류가 발생했습니다.

## 유니티 .

<b>추가/업데이트:</b>

* 사용자가 출력 텍스처가 Unity 자료에 할당되는 방법을 변경할 수 있도록 지원합니다.
* 최신 Unity 2022.2 버전과의 플러그인 호환성

<b>고정:</b>

* 재질에 Int4 입력이 있는 경우 Null 참조 오류
* Int4 입력에 오류가 있습니다. W 값이 Data3 대신 Data2에 할당됩니다.
* 함수 이름 &quot;\_OcclusionStrength&quot;의 오타

## 유니티 .

<b>추가/업데이트:</b>

* 위치 오프셋 컨트롤을 사용하여 [텍스처] 패널에서 서피스를 기준으로 물리적 크기를 변환합니다
* 프로젝트 설정에서 Adobe Substance 3D Assets 및 Substance 커뮤니티 에셋 다운로드 링크

## 유니티 .

<b>추가/업데이트:</b>

* HDRP용 물리적 크기 기능으로 실제 크기에 맞게 재료를 적용하고 크기를 조정할 수 있습니다.
* 프로젝트 설정의 GPU 사용을 위한 UI

<b>제거됨:</b>

* 대부분의 API 호출의 graphID

## 유니티 3.2.1

<b>고정:</b>

* 플러그인을 3.0.0 및 3.1.0에서 최신 버전으로 업그레이드하는 데 문제가 있습니다.

## 유니티 .

<b>추가/업데이트:</b>

* 스크립트 다시 컴파일에 대한 성능 개선

<b>고정:</b>

* 사용자 정의 Sbsar 재질을 가져올 때 Unity 플러그인에서 에셋 가져오기가 실패했습니다.
* &quot;ArgumentException: 값이 예상 범위 내에 있지 않습니다.&quot; 오류
* &quot;ArgumentOutOfRangeException: 인덱스가 범위를 벗어났습니다&quot; 오류

## 유니티 .

<b>추가/업데이트:</b>

* Mac의 1.38배 성능 개선
* Mac의 GPU 엔진이 OpenGL 대신 Metal을 사용함

<b>고정:</b>

* 출력 텍스처의 R 및 B 채널이 뒤집어지는 Mac 문제

## 유니티 .

<b>추가/업데이트:</b>

* Apple Silicon 지원
* 플러그인 사용 방법에 대한 새로운 YouTube 튜토리얼
* 새로운 스크립팅 설명서

<b>고정:</b>

* [임의화] 버튼을 여러 번 누르면 검사기에 표시되는 버그
* Substance 업데이트를 중단하는 Null 텍스처 입력
* &quot;모든 출력 생성&quot;, &quot;Mip 맵 생성&quot; 및 &quot;런타임 전용&quot; 토글이 작동하지 않음
* 네임스페이스 문제
* 그래프 에셋이 선택된 상태에서 재생 모드로 들어갈 때 Null 참조 오류 발생
* 런타임 전용 재질을 사용할 때 최신 2021.3 LTS 버전의 Unity에 대한 HDRP 및 URP 문제
