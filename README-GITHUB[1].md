# 오늘의 한 권 — GitHub Pages 배포용

이 폴더의 내용은 GitHub Pages에서 바로 배포할 수 있는 정적 사이트입니다. 별도의 빌드나 서버가 필요하지 않습니다.

## 업로드 구조

`index.html`이 저장소 최상위(root)에 오도록 이 폴더 안의 파일과 폴더를 업로드하세요. ZIP 파일 자체를 저장소에 올리는 것이 아닙니다.

```text
repository-root/
├── index.html
├── favicon.svg
├── .nojekyll
├── css/
│   └── style.css
└── js/
    ├── app.js
    └── books.js
```

## GitHub Pages 설정

1. GitHub 저장소의 **Settings → Pages**로 이동합니다.
2. **Build and deployment → Source**에서 `Deploy from a branch`를 선택합니다.
3. Branch는 `main`, Folder는 `/(root)`로 선택하고 **Save**를 누릅니다.
4. 배포가 완료되면 Pages 화면에 표시되는 사이트 주소로 접속합니다.

## 참고

- Framework preset이나 Build command는 필요하지 않습니다.
- Cloudflare 전용 `_headers` 파일은 포함하지 않았습니다.
- 프로젝트 저장소 주소가 `https://USERNAME.github.io/REPOSITORY/` 형태여도 CSS와 JavaScript는 상대경로로 연결됩니다.
- 브라우저 보안 정책상 배경음악은 사용자가 음악 버튼을 누른 뒤 재생될 수 있습니다.
