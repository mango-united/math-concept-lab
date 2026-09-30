# 수학 개념 연계 노트

교과 개념과 그 너머의 아이디어를 이어 보는 인터랙티브 수학 노트 모음입니다. GitHub Pages로 공개됩니다.

## 구조

```
index.html            목차 페이지 (노트 목록)
inversion/index.html  반전 기하 실험실
CLAUDE.md             Claude Code가 작업 시작 때 읽는 안내
docs/HANDOFF.md       작업 인계 노트 (현재 상태, 열린 요청, 작업 기록)
docs/CONTENT.md       수학 내용의 기준 (범위, 검산된 값, 후보 노트)
.nojekyll             GitHub Pages가 파일을 그대로 올리도록 하는 표시
```

## 함께 작업하는 방법

수학 내용은 Claude(claude.ai 대화), 코드와 백엔드는 Claude Code가 맡습니다. 둘은 직접 대화할 수 없으므로 `docs/HANDOFF.md`에 부탁할 일과 한 일을 적어 주고받습니다. 자세한 규칙은 `CLAUDE.md`에 있습니다.

노트 하나가 폴더 하나입니다. 각 페이지는 HTML 파일 하나에 스타일과 스크립트가 모두 들어 있어서, 별도의 빌드 과정이 없습니다.

## 새 노트 추가하기

1. 새 폴더를 만들고 그 안에 `index.html`을 넣습니다. 예: `lagrange/index.html`
2. 페이지 상단에 목차로 돌아가는 링크 `<a class="back" href="../">← 수학 개념 연계 노트</a>`를 둡니다.
3. 루트 `index.html`의 `<ol class="notes">` 안에 기존 항목을 복사해 새 노트의 제목, 범위, 설명, 연결된 개념을 적습니다.

## GitHub Pages 켜기

저장소의 **Settings → Pages**에서 Source를 **Deploy from a branch**, Branch를 **main / (root)**로 저장합니다. 1~2분 뒤 `https://<계정>.github.io/<저장소>/`에서 열립니다.

## 내 컴퓨터에서 미리 보기

```
python3 -m http.server 8000
```

실행 후 브라우저에서 `http://localhost:8000`을 엽니다.
