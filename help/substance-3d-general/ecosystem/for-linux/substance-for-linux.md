---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-general/ecosystem/substance-for-linux.html"
breadcrumb-title: ''
description: Adobe 다운로드 액세스 포털을 사용하여 Linux에서 Substance 3D 애플리케이션을 다운로드, 설치 및 활성화하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Substance 3D General
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Linux용 Substance 3D (ADA)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 081136918fdf7f431ecee47e5ce64d8b5235bb1b
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---


# 배포 안내서

Enterprise 계약을 통해 Linux®용 Substance 3D을 구입하면 해당 제품과 라이선스가 [Adobe 다운로드 액세스(ADA)](https://download-access.adobe.com/lws/downloads) 포털에 프로비저닝됩니다. 소프트웨어를 성공적으로 배포하려면 ADA에서 소프트웨어 빌드와 라이선스 키 파일을 모두 다운로드해야 합니다.

## 소프트웨어 빌드를 다운로드하고 키 파일에 라이선스 부여:

[다운로드 액세스 Adobe](https://download-access.adobe.com/lws/downloads)에 로그인합니다. 소프트웨어 빌드를 찾고 키 파일에 라이선스를 부여합니다.

1. 계정 드롭다운을 사용하여 Substance 3D Linux를 구매한 계정을 선택합니다.

   ![](../../assets/ADA1.png)
1. 페이지 헤더에 링크가 있는 다운로드로 이동합니다.

   ![](../../assets/ADA2.png)
1. 해당 제품에서 다운로드 보기 를 클릭합니다.

   ![](../../assets/ADA3.png)
1. ADA가 이 ID와 관련된 라이선스 정보를 로드하여 아래 표에 표시합니다.
1. &quot;디지털 인증서&quot; 줄에서 &quot;다운로드&quot;를 클릭하여 라이센스 키 파일이 포함된 zip 파일을 다운로드합니다.

   * zip 파일에는 제품당 하나의 라이센스 키가 들어 있습니다.
   * 라이선스 키는 라이선스가 부여된 각 컴퓨터에서 제품을 활성화합니다.

   ![](../../assets/ADA4.png)
1. &quot;Substance 3D&quot; Sampler, Painter 또는 Designer을 클릭하여 Substance 3D Painter, Substance 3D Designer 및 Substance 3D Sampler의 소프트웨어 빌드를 표시합니다.
1. 설치하고자 하는 제품의 설치 파일을 다운로드하려면 &quot;다운로드&quot;를 클릭하십시오.

   ![](../../assets/ADA5.png)
1. &quot;소프트웨어 다운로드&quot; 알림이 표시됩니다. &quot;수락&quot;을 클릭합니다.

   ![](../../assets/ADA6.png)

## 설치 및 활성화

소프트웨어를 설치하려면 다음을 수행하십시오.

1. 제품의 EXE 파일을 더블 클릭하여 설치 마법사를 시작합니다.
1. 설치 단계에 따라 설치를 완료합니다.

소프트웨어 활성화를 위해 로컬 활성화 또는 네트워크 활성화의 두 가지 옵션이 있습니다.

### 로컬 활성화

1. ADA에서 다운로드한 zip 폴더의 압축을 풉니다.
1. 활성화할 소프트웨어를 실행합니다.
1. 활성화 마법사에서 &quot;라이선스 키 파일을 사용하여 활성화&quot;를 선택합니다.

   ![](../../assets/LinuxActivation3.png)
1. &quot;찾아보기&quot;를 클릭하고 해당 라이센스 키 파일의 위치를 가리킵니다.
1. &quot;다음&quot;을 클릭하여 소프트웨어를 활성화합니다.

### 네트워크 활성화

1. ADA에서 다운로드한 zip 폴더의 압축을 풉니다.
1. 공유 마운트 네트워크에 압축 해제된 라이선스 키 파일을 배치합니다.
1. 사용자 컴퓨터에서 다음 페이지에 설명된 대로 라이선스 키 파일을 가리키는 환경 변수를 설정합니다.

   * Substance 3D Painter - <https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/pipeline-and-integration/configuration/environment-variables>
   * Substance 3D Designer - <https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/pipeline-and-project-configuration/environment-variables>
   * Substance 3D Sampler - <https://experienceleague.adobe.com/en/docs/substance-3d-sampler/using/pipeline-and-integrations/environment-variables>
