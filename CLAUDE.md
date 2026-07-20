# skylife-addons 프로젝트 규칙

공통 규칙은 상위 디렉토리 `/Users/jaypark/workspace/CLAUDE.md` 참고.

## 이 페이지 정보
- **용도**: 스카이라이프 모바일 부가서비스 전체 목록 + 검색/필터
- **파일**: `index.html` (단일 파일)
- **GitHub Pages URL**: https://pjungjin85-sketch.github.io/skylife-addons/

## 기능 구조
- 검색창 + 카테고리 필터 + 리셋 버튼
- 카드 클릭 시 모달로 상세 정보 표시
- `applyFilters()` 함수가 핵심 필터링 로직

## 수정 시 주의사항
- 부가서비스 데이터는 `const ADDONS = [...]` 배열에 있음
- 카테고리 목록이 바뀌면 필터 버튼도 같이 업데이트할 것
- 모달 구조 (`#modalOverlay`, `#modalBody`) 건드리지 말 것 — 의존성 있음
