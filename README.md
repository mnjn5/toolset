# 작업 도구함

GitHub와 Vercel에 바로 올릴 수 있도록 구성한 정적 웹 도구 모음입니다.

## 구조

```text
.
├── index.html                              # 도구 허브 메인 페이지
├── tools/
│   └── screen-spec-ppt-converter/
│       └── index.html                      # 화면설계서 PPT 변환기
└── assets/                                 # 공통 이미지·폰트 등 정적 자산
```

## 배포

1. 이 폴더를 GitHub 저장소에 푸시합니다.
2. Vercel에서 해당 GitHub 저장소를 Import합니다.
3. Framework Preset은 `Other`, Build Command는 비워 두고 배포합니다.

빌드 과정이 필요 없는 순수 정적 HTML 사이트입니다. 새 도구는 `tools/<도구-이름>/index.html` 형태로 추가한 뒤, 루트 `index.html`의 도구 카드만 추가하면 됩니다.
