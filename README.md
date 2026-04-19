# 🎯 RIASEC 직업 카드 메이커

> **진로 표준 RIASEC 흥미 검사로 나에게 맞는 직업 3장 카드 생성!**
> 18문항 검사 → 상위 2개 흥미 유형 → 매칭 직업 3개 → Gemini로 일러스트 카드 생성 → 인쇄

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Try%20Now-black?logo=vercel)](https://riasec-career-cards.vercel.app/)
[![Gemini](https://img.shields.io/badge/Gemini-2.5%20Flash%20Image-blue)](https://ai.google.dev/gemini-api/docs/image-generation)
[![RIASEC](https://img.shields.io/badge/Career%20Test-RIASEC%20%C2%A9%20Holland-purple)](https://en.wikipedia.org/wiki/Holland_Codes)
[![Print Ready](https://img.shields.io/badge/Print-13%3A10%20Card-emerald)](#)

---

## 🎯 기획 의도

진로 부스의 핵심은 단순히 "재미있는 사진"을 넘어 **"나에게 맞는 길"**을 발견하게 하는 것입니다. 본 앱은 진로교육의 표준 모델인 **RIASEC(홀랜드 직업흥미 모델)**을 기반으로:

1. 18문항 간이 검사 (3분)
2. 상위 2개 흥미 유형 자동 산출
3. 그 조합에 가장 잘 맞는 **직업 3개** 매칭
4. Gemini가 직업별 일러스트 카드 생성
5. 13:10 인쇄용 카드 다운로드

진로 담당 선생님·학교 진로 부스에 가장 적합한 형식입니다.

---

## ✨ 주요 기능

| 기능 | 설명 |
|------|------|
| 📋 **18문항 표준 검사** | 6유형 × 3문항, 1~5점 슬라이더로 답변 |
| 📊 **6유형 점수 시각화** | 결과 화면에 모든 유형 점수 막대로 표시 |
| 🎴 **직업 3장 매칭** | 상위 2개 유형 조합으로 최적 직업 추천 |
| 🖼️ **AI 일러스트 카드** | Gemini가 한국 학생 친화 일러스트로 생성 |
| 📐 **13:10 인쇄 비율** | 직업카드·포토프린터 출력 최적 |
| 💾 **개별/전체 다운로드** | 한 장씩 또는 ZIP 일괄 |
| 🔐 **BYOK 방식** | 사용자 본인의 Gemini API 키, 외부 저장 없음 |

---

## 🚀 바로 사용하기

👉 **[https://riasec-career-cards.vercel.app/](https://riasec-career-cards.vercel.app/)**

### 사용 단계

1. **「🚀 검사 시작」** 클릭
2. **18문항 답변** (각 1~5점, 약 3분)
3. **결과 화면**에서 6유형 점수 확인 + 상위 2개 조합 확인
4. **API 키 입력** ([Google AI Studio](https://aistudio.google.com/apikey)에서 무료 발급)
5. **「🎴 직업 카드 3장 생성」** 클릭 → AI 일러스트 자동 생성
6. **카드 다운로드** → 포토프린터 인쇄

---

## 🧬 RIASEC 6가지 흥미 유형

| 코드 | 유형 | 핵심 특성 |
|------|------|-----------|
| **R** | 🔧 실재형 (Realistic) | 도구·기계·자연을 다루는 활동을 좋아하는 실용주의자 |
| **I** | 🔬 탐구형 (Investigative) | 관찰·분석·논리적 사고로 문제를 풀어내는 학자형 |
| **A** | 🎨 예술형 (Artistic) | 창의·표현·자유로운 상상을 즐기는 예술가형 |
| **S** | 🤝 사회형 (Social) | 사람을 돕고 가르치고 협력하는 따뜻한 협력자 |
| **E** | 📈 진취형 (Enterprising) | 리더십·설득·도전으로 목표를 이뤄내는 추진자 |
| **C** | 📋 관습형 (Conventional) | 꼼꼼함·정확성·체계적 정리에 강한 신뢰의 관리자 |

> 💡 **John Holland**(미국 심리학자)의 직업선택이론 기반. 학교 진로교육에서 가장 널리 쓰이는 표준 모델.

---

## 🎴 직업 매칭 매트릭스

상위 2개 유형 조합(15개)별로 사전 정의된 직업 3개씩 매칭:

| 조합 | 추천 직업 |
|------|-----------|
| **RI** | 기계공학자 · 수의사 · 응급의료기사 |
| **RA** | 건축가 · 산업디자이너 · 항공정비사 |
| **RS** | 체육교사 · 물리치료사 · 농업지도사 |
| **RE** | 군 장교 · 건설현장 매니저 · 농장 경영자 |
| **RC** | 측량기사 · 품질검사원 · 기계제도사 |
| **IA** | 과학자 · 약사 · AI 연구원 |
| **IS** | 임상심리사 · 의사 · 사회복지 연구원 |
| **IE** | 변호사 · 경영 컨설턴트 · 시장 분석가 |
| **IC** | 회계사 · 데이터 분석가 · 통계학자 |
| **AS** | 국어교사 · 음악치료사 · 방송작가 |
| **AE** | 광고 기획자 · 영화 감독 · 공연 기획자 |
| **AC** | 그래픽 디자이너 · 도서관 사서 · 편집 디자이너 |
| **SE** | 기업 강사 · HR 매니저 · 사회운동가 |
| **SC** | 간호사 · 사회복지사 · 행정 공무원 |
| **EC** | 프로젝트 매니저 · 은행 지점장 · 스타트업 창업가 |

---

## 🛠️ 기술 스택

| 분류 | 기술 |
|------|------|
| **검사 로직** | Vanilla JavaScript (점수 합산 + TOP-2 매칭) |
| **AI 모델** | Google **Gemini 2.5 Flash Image** (`gemini-2.5-flash-image`) |
| **프론트엔드** | 단일 `index.html` 파일 |
| **스타일링** | Tailwind CSS (CDN) + 글래스/오로라 디자인 |
| **압축 다운로드** | [JSZip](https://stuk.github.io/jszip/) |
| **타이포그래피** | Pretendard |
| **호스팅** | Vercel (정적, GitHub 연동 자동 배포) |

---

## 📦 로컬 실행

```bash
git clone https://github.com/tigerjk9/riasec-career-cards.git
cd riasec-career-cards
python -m http.server 8000
# 브라우저에서 http://localhost:8000 접속
```

---

## 🔑 API 키 발급 가이드

1. [Google AI Studio](https://aistudio.google.com/apikey) 접속
2. Google 계정 로그인
3. **"Create API Key"** 클릭 → 키 복사
4. 검사 결과 화면에서 입력란에 붙여넣기

> 🔒 **보안:** API 키는 사용자 브라우저 내에서만 사용됩니다.

---

## 📁 저장소 구성

```
riasec-career-cards/
├── README.md       # 본 문서
├── index.html      # 단일 파일 웹앱 (검사 + 결과 + 카드 생성)
└── .gitignore
```

---

## 🎯 활용 사례

- 🎓 **학교 진로교육** - 표준 RIASEC 검사 + 시각화
- 🏫 **진로 동아리** - 친구들과 결과 비교 워크숍
- 📚 **진로 상담실** - 학생 자기 이해 도구
- 🧑‍🏫 **자유학기제 활동** - 진로 탐색 모듈

---

## 🐛 알려진 제약

- 18문항 간이 검사로, 정밀한 진단은 학교·전문 검사 보완 필요
- Gemini API 응답 시간: 카드 3장 생성 약 5~15초
- 모바일도 지원하지만 PC 권장

---

## 📝 변경 이력

| 날짜 | 내용 |
|------|------|
| 2026-04-19 | 🌟 **실시간 6각형 레이더 차트** 추가 — 검사 화면 우측에서 답변할 때마다 SVG 폴리곤이 채워지는 시각화 (검사 완주율 ↑) |
| 2026-04-19 | 🎴 **포스터형 직업카드 디자인** 적용 — 헤더(유형 색)·이름·학교·일러스트·PERSONALITY STATS 별점·CAREER MATCH·HALL OF FAME(한국 명사)·푸터 |
| 2026-04-19 | 💸 **예산 절감 모드** — 직업 카드 3장 → 매칭 직업 3개 중 1개 선택 → 카드 1장만 생성 |
| 2026-04-19 | ✏️ 검사 결과 화면에 **이름·학교명 입력 필드** 추가 (카드 헤더/푸터 자동 반영) |
| 2026-04-19 | 🎨 글래스모피즘 + 오로라 디자인 (부스 메인과 통일) |
| 2026-04-19 | 초기 출시 (RIASEC 18문항 검사 + Gemini 직업 일러스트) |

---

## 🌟 향후 개선 아이디어

- [ ] 검사 결과 PDF 리포트 다운로드
- [ ] 36문항 정밀 모드 (선택)
- [ ] 같은 유형 학생끼리 매칭 (학급 활동 연계)
- [ ] 직업별 상세 정보(평균 연봉·전공·자격증) 추가

---

## 🔗 관련 프로젝트 (진로 시리즈)

| 프로젝트 | 설명 | 라이브 |
|---------|------|--------|
| **Career Photo Studio** | 사진 → 8가지 직업 변신 | [link](https://career-photo-studio.vercel.app/) |
| **RIASEC Career Cards** *(본 프로젝트)* | 흥미 검사 → 매칭 직업 3장 카드 | [link](https://riasec-career-cards.vercel.app/) |
| **Future Business Card** | 10년 후 나의 명함 + 자서전 | [link](https://future-business-card.vercel.app/) |

본 프로젝트는 [AI Hands-On 부스](https://ai-hands-on-booth-v2.vercel.app/)에 등록되어 있습니다.

---

## 🙏 크레딧

- **John Holland** — RIASEC 직업선택이론 (1959)
- **Google Gemini 2.5 Flash Image** — 직업 일러스트 생성
- **Tailwind CSS** · **Pretendard** · **JSZip**

---

## 📝 라이선스

MIT License (코드) · RIASEC 모델은 ⓒ John Holland

---

## 👤 제작자

**김진관 (닷커넥터)**
- GitHub: [@tigerjk9](https://github.com/tigerjk9)
- Linktree: [litt.ly/dot_connector](https://litt.ly/dot_connector)

---

> 🎯 **지금 바로 [RIASEC 직업 카드](https://riasec-career-cards.vercel.app/)에서 나만의 흥미 유형과 맞춤 직업을 발견하세요!**
