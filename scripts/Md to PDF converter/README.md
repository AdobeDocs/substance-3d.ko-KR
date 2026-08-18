---
source-git-commit: a517442244806bc6aef0f5bfb165c5d4f67341be
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---
# PDF 변환기로 마크다운

이 폴더에는 이 저장소에서 문서 페이지의 PDF 버전을 생성하기 위한 전처리 및 변환 스크립트가 포함되어 있습니다.

## 이 항목이 있는 이유

설명서 소스 파일은 표준 마크다운 도구가 인식하지 못하는 Adobe 플랫폼별 마크다운 구문(아코디언 블록, 경고 콜아웃 및 이미지 특성 확장)을 사용합니다. 이 스크립트는 구문을 정규화하고 [md-to-pdf](https://github.com/simonhaenisch/md-to-pdf)을(를) 사용하여 파일을 PDF으로 변환하는 동시에 이미지를 압축하여 출력 파일 크기를 관리 가능하게 유지합니다.

## 사전 요구 사항

- [Node.js](https://nodejs.org/)&#x200B;(v18 이상)
- `node_modules/`에 종속성이 이미 설치되어 있습니다. 다시 설치해야 하는 경우 이 폴더에서 `npm ci`을(를) 실행하십시오.

## 사용

**리포지토리 루트**&#x200B;에서 스크립트를 실행하고 변환할 마크다운 파일의 경로를 전달합니다.

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" <path/to/file.md>
```

**예:**

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" help/substance-3d-general/openpbr/openpbr-overview.md
```

PDF이 **원본 파일과 같은 디렉터리**&#x200B;에 기록됩니다. 변환 중 생성된 임시 파일(`*.pdf-ready.md` 및 `_pdf-images/`)은 성공 시 자동으로 삭제됩니다. 변환이 실패하면 디버깅을 지원하기 위해 그대로 유지됩니다.

## 스크립트의 기능

| 소스 구문 | PDF 출력 |
|---|---|
| 아코디언 블록 `+++Title`/`+++`개 | 콘텐츠가 항상 표시되는 `#####` 제목 |
| 경고 콜아웃 `>[!NOTE]`개 | 굵은 **참고:** 접두사가 있는 표준 블록 따옴표 |
| `![](path){width="N"}` 이미지 특성 | 지정된 너비를 유지하는 `<img>` 태그 |
| `.pdf`개 파일에 대한 마크다운 이미지 링크 | 제거됨(웹 전용 자체 다운로드 참조) |
| `hold:` 프런트 마스트 키 | 제거됨(플랫폼 전용 메타데이터) |
| 모든 이미지 | 너비가 최대 1200px로 크기 조정되고 80% 품질로 JPEG으로 다시 인코딩됨 |
| 모든 테이블 | 삽입된 CSS를 통해 제거된 테두리 및 배경 |
