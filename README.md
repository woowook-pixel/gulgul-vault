# gulgul-vault

굴굴 보관함 페이지입니다. 비공개 저장소 `gulgul-assets`의 파일을 보기 편하게 보여 줍니다.

- 이 저장소에는 페이지 파일만 있고 굴굴 파일은 없습니다. 파일은 `gulgul-assets`(private)에 있습니다.
- 처음 열면 GitHub 토큰(Fine-grained token, `gulgul-assets`만 선택, Contents: Read and write)을 한 번 입력합니다. 보기만 할 때는 Read-only도 되지만 올리기에는 쓰기 권한이 필요합니다. 토큰은 그 기기의 브라우저에만 저장됩니다.
- 파일: `index.html`, `manifest.webmanifest`, `icons/`
- 배포: GitHub Pages (Settings > Pages > Branch: main, / (root))
- 올리기: 상단 '올리기' 버튼으로 zip(폴더 경로 그대로) 또는 개별 파일(폴더와 파일 이름 선택)을 `gulgul-assets` main에 커밋 하나로 올립니다. 파일 하나는 25MB까지입니다. zip 해제에는 JSZip(cdnjs)을 씁니다.
- 목록 복사: 오른쪽 위 더보기(점 세 개) 메뉴의 '목록 복사'로 전체 파일을 `경로, 크기(KB), 마지막 수정일` 한 줄씩 클립보드에 복사합니다. 수정일은 main 커밋 이력에서 찾으며, 처음 한 번만 오래 걸리고 결과는 이 기기에 저장됩니다.
- 삭제: 더보기 메뉴의 '파일 선택 · 삭제'로 여러 파일을 고르거나, 미리보기와 읽기 화면 위쪽의 휴지통 버튼으로 한 파일을 삭제합니다. 확인 후 커밋 하나(`보관함 삭제: 파일 n개`)로 main에서 지우며, GitHub 커밋 기록에서 되돌릴 수 있습니다. 쓰기 권한 토큰이 필요합니다.
- 로고 탭: `gulgul-assets`의 `brand/`와 `logo/`(01_mark, 02_wordmark, 03_lockup, 04_app_icon, 05_favicon, 06_social, 07_guidelines)를 한 탭에서 하위 폴더별로 묶어 보여 줍니다. SVG, PNG, ICO 미리보기와 md 읽기를 지원합니다. 그 밖의 확장자(html, pdf 등)는 저장소에는 있어도 보관함에 표시하지 않습니다.
