# CLAUDE.md — RIASEC 직업 카드

## 한 줄 정의
진로 표준 RIASEC 18문항 검사 → 매칭 직업 1개 선택 → 포스터형 직업카드 PNG.

## 라이브 / 저장소
- 🌐 https://riasec-career-cards.vercel.app/
- 🐙 https://github.com/tigerjk9/riasec-career-cards

## 기술 스택
- 단일 `index.html` (Vanilla JS)
- Tailwind CSS CDN + Pretendard + html2canvas 1.4.1
- Gemini 2.5 Flash Image (일러스트 1장)
- Gemini 2.5 Flash Text JSON (Hall of Fame 명사 정보)

## 핵심 데이터 구조
- `TYPES{}`: R/I/A/S/E/C 6개 (`{name, emoji, color, grad, desc, stat}`)
- `QUESTIONS[]`: 18문항 (각 유형 3문항)
- `CAREER_MAP{}`: 15개 조합(RI~EC) + 6개 단일 fallback → 직업 3개씩
- `COMBO_DESC{}`: 15개 조합 한 줄 설명

## 핵심 결정
- **3장 → 1장** (예산 절감): 매칭 3개 중 1개 선택 후 카드 1장만 생성
- **포스터형 카드 디자인** (참고: 카카오톡 ESTJ 카드)
  - 헤더(유형 색) + 이름·학교
  - RIASEC 코드 배지 3곳 (헤더/이미지/푸터)
  - **풀 한글 라벨 동반** (`🤝 사회형(S) × 📋 관습형(C)`) — 영문 약자만으론 의미 X
  - PERSONALITY STATS = 사용자 RIASEC TOP 4 점수 → 별점
  - HALL OF FAME = AI가 생성한 한국 명사 2~3명
- **실시간 6각형 레이더 차트** (검사 화면 우측, SVG, 답변마다 폴리곤 갱신)

## 자주 마주치는 이슈
- **별점 깨짐:** `★`은 폰트 의존이라 캡처 시 정렬 어긋남 → `font-family: Arial, sans-serif` + `letter-spacing: 1px`
- **PNG 텍스트 깨짐:** `await document.fonts.ready` + onclone에서 `font-family` fallback 명시
- **Hall of Fame 부정확:** Gemini Text가 가짜 인물 만들 수 있음 → 프롬프트에 "실존만, 불확실 시 직무 가치로 대체"

## 변경 핵심 이력
- 2026-04-19: 초기 3장 → 1장 + 포스터 카드 + 이름/학교 입력 + 레이더 차트 + RIASEC 코드 풀 라벨

## 관련 문서
- [PRD.md](./PRD.md)
