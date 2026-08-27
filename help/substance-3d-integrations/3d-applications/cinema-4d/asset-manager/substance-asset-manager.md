---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/substance-asset-manager.html"
breadcrumb-title: ''
description: Cinema 4D에서 Substance 에셋 관리자를 사용하여 장면에 Substance 재질을 추가, 제거 및 구성할 수 있습니다.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Substance Asset Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 에셋 관리자
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---


# Substance 에셋 관리자

[Substance 에셋 관리자] 창에는 장면에 로드된 모든 Substance이 나열됩니다. 여기에서 Substance을 추가, 제거 및 재구성할 수 있습니다.

Substance 에셋 관리자 내에서 Substance을 선택(왼쪽 클릭)하면 Cinema 4D의 속성 관리자에서 Substance이 열립니다. 이 경우 Cinema 4D의 다른 매개 변수처럼 매개 변수와 키프레임 Substance 입력을 변경할 수 있습니다.

>[!NOTE]
>
> 속성 관리자에는 특별한 Substance 에셋 모드가 있어 Cinema 4D 레이아웃에 Substance 전용 속성 관리자를 보유한 경우 편리합니다.

![](../../../assets/cinema-4d-4.png){width="500px"}

## 파일 메뉴

## 에셋 로드...

장면에 새 Substance을 로드합니다([플러그인] 메뉴에서와 동일함).

닫기

Substance Asset Manager를 닫습니다. 로드된 Substance은 당연히 장면에 남아 있습니다.

## 편집 메뉴

## 모든 Substance 선택

Asset Manager에 나열된 모든 Substance을 선택합니다. Ctrl+a를 눌러도 마우스가 Asset Manager 위에 놓일 수 있습니다.

## 모든 Substance 선택 해제

Asset Manager에 나열된 모든 Substance을 선택 취소합니다. Shift+Ctrl+a를 눌러도 마우스가 Asset Manager 위에 놓일 때 동일한 작업을 수행할 수 있습니다.

## 선택한 재질에서 선택

현재 *선택한* 자료에서 참조하는 모든 Substance을 선택합니다.

## 표시된 재질에서 선택

현재 *표시* 자료에서 참조하는 모든 Substance을 선택합니다. Cinema 4D에서 이 재질을 사용한 개체나 태그가 선택되면 해당 재질이 표시됩니다.

## 재질 선택

현재 선택한 Substance을 참조하는 모든 재질을 선택합니다.

## 액션 메뉴

## 재질 만들기

현재 선택한 Substance에서 새 Cinema 4D 재질을 만듭니다. 재료 채널들은 Substance의 각각의 출력 채널을 참조하는 Substance 셰이더들로 자동으로 초기화될 것이다.

## Substance 복제

현재 선택한 Substance을 복제합니다. 이는 여러 재질에 서로 다른 파라미터 세트를 가진 동일한 Substance을 사용하는 데 유용할 수 있다.

## Substance 다시 가져오기

이 함수는 Substance의 기본값으로 돌아가거나 (예를 들어, Substance Designer의) 외부 변경들을 통합하는 데 사용될 수 있다.\
참고: Substance 입력에 대한 **모든** 매개 변수 변경 내용이 손실됩니다!

## Substance 제거

장면에서 현재 선택된 Substance을 제거합니다. Asset Manager 위에 마우스를 올려놓은 상태에서 Delete 키를 눌러도 동일한 결과를 얻을 수 있습니다.

## 사용하지 않는 Substance 삭제

현재 어떠한 재질에서도 참조되지 않는 모든 Substance을 제거합니다.

## Substance 엔진 메뉴

이 메뉴의 내용은 Cinema 4D이 실행 중인 운영 체제에 따라 다릅니다. Substance 엔진 변경은 Cinema 4D을 다시 시작한 후에만 적용됩니다.

## 컨텍스트 메뉴

선택한 Substance을 마우스 오른쪽 버튼으로 클릭하면 컨텍스트 메뉴가 표시됩니다. 이 기능은 앞서 설명한 메뉴에서 이름이 같은 함수와 동일합니다.

* 제거
* 재질 만들기
* Substance 복제
* Substance 다시 가져오기
* 모든 Substance 선택
* 모든 Substance 선택 해제
* 재질 선택

## 드래그 앤 드롭

드래그 앤 드롭을 통해 Substance Asset Manager와 상호 작용할 수 있습니다. 다음과 같은 몇 가지 옵션을 사용할 수 있습니다.

* 탐색기 또는 Finder에서 Substance을 Substance Asset Manager에 놓아 드래그하여 놓아 장면에 콘텐츠를 불러옵니다.
* 셰이더와 Substance 에셋을 연결하기 위해 Substance 셰이더의 Substance 필드로 링크를 끌 수 있습니다.
* 정렬되지 않음 모드(아래 참조)인 경우 Asset Manager에서 Substance을 새 위치로 드래그하여 다시 정렬할 수 있습니다.


## Substance 에셋 관리자에서 정렬

## 정렬되지 않은 모드

## Substance 자산 관리자가 기본적으로 **정렬되지 않은 모드**&#x200B;에 있습니다. 이름 열의 머리글 셀에 오른쪽에 화살표가 표시되지 않습니다. 드래그 앤 드롭을 사용하여 물질을 원하는 대로 다시 정렬할 수 있습니다.

![](../../../assets/cinema-4d-3.png){width="500px"}

![](../../../assets/cinema-4d-5.png){width="500px"}

## Substance 에셋 관리자의 미리 보기

## Substance 에셋 관리자에 각 Substance에서 사용할 수 있는 채널의 미리 보기가 있는 작은 아이콘이 표시됩니다.

## 미리 보기는 Substance에서 출력 채널 순서로 표시됩니다. 미리 보기가 표시되는 열에는 의미가 없습니다.
