# 📚 Awesome-AI-Agents 저장소 분석 & 활용 정리

> 작성일: **2026-09-18**
> 대상 저장소: **https://github.com/bmshin94/Awesome-AI-Agents**
> 원본(포크 출처): **https://github.com/ChatTeach/Awesome-AI-Agents**
> 정리: Claude Code (페르소나 "카리나")

---

## 📑 목차

1. [저장소 정체 분석](#1-저장소-정체-분석)
2. [쉬운 버전 설명](#2-쉬운-버전-설명)
3. [핵심 Q&A 7선](#3-핵심-qa-7선)
4. [수익화 아이디어 7가지](#4-수익화-아이디어-7가지)
5. [수록 프로젝트 전체 링크](#5-수록-프로젝트-전체-링크)

---

## 1. 저장소 정체 분석

### 1-1. 한 줄 요약

실행 코드가 **0줄**인 **`awesome-list` 계열 큐레이션 문서 저장소**.
AI 에이전트 오픈소스 프로젝트 **65개**를 이름·설명·GitHub 링크 형태로 모아둔 목록이다.

### 1-2. 파일 구조 (전수조사)

| 파일 | 크기 | 역할 |
|---|---|---|
| `README.md` | 2.1KB | 소개 + 뉴스레터 구독 유도 (구독 링크 5회 등장) |
| `AGENTS.md` | 19.7KB | **핵심 콘텐츠.** 프로젝트 65개 목록 |
| `CONTRIBUTING.md` | 2.5KB | 기여 가이드 (fork → branch → commit → PR) |
| `manuagi.PNG` | 48KB | 뉴스레터 배너 이미지 |
| `CLAUDE.md` | 1.4KB | Claude Code 프로젝트 메모리 (카리나 페르소나 설정) |

- `package.json` / `requirements.txt` / `src/` / `.github/` — **모두 없음**
- 총 파일 5개, 총 커밋 40개

### 1-3. AGENTS.md 수록 항목 카테고리 분류

| 카테고리 | 대표 프로젝트 |
|---|---|
| 범용 에이전트 프레임워크 | AutoGPT, MetaGPT, Agno, Agent Zero, AutoAgent |
| 메모리 / 기억 레이어 | Mem0, Letta(구 MemGPT), Supermemory |
| MCP 생태계 | FastMCP, MCP-Go, MCP-Agent, Playwright MCP |
| 브라우저 / 컴퓨터 조작 | Browser-use, Steel, Open Interface, Agent.exe |
| 코딩 에이전트 | OpenHands, GPT Pilot, PR-Agent, CopilotKit |
| 로컬 / 프라이버시 | Local Deep Researcher, Sidekick, TinyAgent |
| 산업 특화 | FinRobot(금융), HuatuoGPT-o1(의료), LeRobot(로봇), AI Scientist(연구) |
| 운영 / 평가 | AgentOps, TheAgentCompany, Agenta |
| 실시간 / 음성 | LiveKit Agents, Realtime API Agents, CSM |

### 1-4. 언제 쓰나

1. **기술 선정** — "메모리 붙이려면?" → Mem0 vs Letta 후보 즉시 확보
2. **트렌드 파악** — 2025년 4월 시점 판도 스냅샷
3. **아이디어 수집** — 에이전트로 가능한 영역 탐색
4. **오픈소스 기여 연습** — 구조가 단순해 첫 PR 대상으로 적합

### 1-5. ⚠️ 비판적 검토 (반드시 인지할 것)

| 문제 | 상세 |
|---|---|
| 🎣 **마케팅 깔때기 성격** | README에 뉴스레터(`manuagi.beehiiv.com`) 구독 링크 5회 삽입. 무료 가치 제공 → 구독자 확보 구조 |
| 📅 **콘텐츠 노후화** | 마지막 콘텐츠 갱신 `2025-04-08`. 기준일(2026-09-18) 대비 **약 17개월 정체**. README는 "weekly 업데이트"라고 명시 |
| 🐛 **오분류** | `Luna Executor`는 AI 에이전트가 아닌 **로블록스 스크립트 실행기** |
| 🐛 **출처 오류** | `Codename Goose`를 `deepseek-ai/codename-goose`로 기재. 실제는 Block사의 `block/goose` |
| 🐛 **중복 등재** | `GenAI Agents`, `AppAgent` 각 2회 중복 |
| 🐛 **문서 불일치** | README의 폴더 구조에 `images/` 명시되어 있으나 실제 디렉터리 없음 |
| 🔀 **포크본** | 원본은 `ChatTeach/Awesome-AI-Agents` |

> **결론:** "검증된 정답지"가 아니라 **"출발점 지도"**. 여기서 후보를 건지고, 각 프로젝트 원본 저장소에서 최신 상태를 반드시 재확인할 것.

---

## 2. 쉬운 버전 설명

### 비유

> **이 저장소 = "AI 에이전트 맛집 리스트 노트"**

강남에 식당이 수백 개일 때, 친구가 건네준 손글씨 추천 노트와 같다.
노트가 밥을 해주지는 않지만, **"어디 갈지 정하는 시간"** 을 극적으로 줄여준다.

- AI 에이전트 = 식당들 (65개)
- `AGENTS.md` = 손글씨 노트
- GitHub Link = 식당 주소

### 챗봇 vs AI 에이전트

| 구분 | 챗봇 (ChatGPT) | AI 에이전트 |
|---|---|---|
| "맛집 예약해줘" | **말로** 알려줌 | **실제로 예약 실행** |
| 능력 | 대화 | 대화 + 도구 사용 + 다단계 반복 + 기억 |
| 비유 | 입만 있음 | 입 + 손 + 발 + 기억력 |

핵심 차이는 **도구(Tool) 사용**과 **자율적 반복(loop)**.

### 사용 시나리오 비교

```
[리스트 없을 때] 구글 검색 → 블로그 20개 → 광고글 반 → 3시간 소모 → 포기
[리스트 있을 때] AGENTS.md 3분 훑기 → Agno + Mem0 + browser-use 조합 발견 → 즉시 착수
```

### 기억할 3가지

1. 코드가 아니라 **목록**이다 → 설치할 것이 없다
2. 읽고 → 고르고 → 그 링크로 이동해서 → 거기서 실제 작업
3. 17개월 정체 상태 → **참고용**으로만, 최신 여부는 별도 확인

---

## 3. 핵심 Q&A 7선

### Q1. 설치 및 사용법

**설치 개념 자체가 없다.** 마크다운 문서이므로 읽는 것이 곧 사용이다.

```bash
# 방법 1: 웹에서 바로 읽기 (권장)
# https://github.com/bmshin94/Awesome-AI-Agents/blob/main/AGENTS.md

# 방법 2: 클론해서 검색 활용
git clone https://github.com/bmshin94/Awesome-AI-Agents.git
cd Awesome-AI-Agents
cat AGENTS.md
grep -i "memory" AGENTS.md      # 메모리 관련 항목만 추출
grep -c '^### ' AGENTS.md       # 총 65개 확인

# 방법 3: 개인 큐레이션으로 개조 (가장 실용적)
git checkout -b my-curation
# AGENTS.md에 "⭐ 검증 완료", "🔖 나중에 볼 것" 섹션 추가
```

수록된 프로젝트를 실제로 구동하려면 각 프로젝트 저장소의 설치 절차를 따라야 한다.

```bash
pip install agno                 # 프로젝트마다 상이
export ANTHROPIC_API_KEY=...     # LLM 키 필요
python my_agent.py
```

---

### Q2. 플러그인인가? 스킬인가? MCP인가?

**셋 다 아니다. 순수 문서(Documentation)다.**

| 구분 | 정체 | 비유 | 형태 | 실행 주체 |
|---|---|---|---|---|
| 🔌 **MCP** | AI ↔ 외부 도구 **연결 표준 프로토콜** | USB-C 단자 | 별도 서버 프로세스 | 서버 |
| 🧠 **Skill** | AI에게 주는 **작업 설명서** | 레시피 카드 | 마크다운 폴더 | AI가 읽고 수행 |
| 🧩 **Plugin** | 스킬+명령어+MCP설정 **묶음 패키지** | 밀키트 세트 | 배포 가능한 번들 | 툴이 로드 |
| 📄 **이 저장소** | 사람이 읽는 **글** | 요리책 | `.md` 파일 | 사람 |

확인 결과: `mcp.json` 없음 / `.claude/skills/` 없음 / `.claude-plugin/` 없음.
이 저장소는 MCP를 **소개**만 할 뿐(FastMCP, MCP-Go 등), 본인이 MCP인 것은 아니다.

**단, `CLAUDE.md`는 예외** — 이는 Claude Code가 세션 시작 시 자동으로 읽는 **프로젝트 메모리(Project Memory)** 파일이다. 플러그인도 스킬도 아니지만 AI의 동작에 직접 영향을 준다.

> 💡 **개선 제안:** `AGENTS.md`를 Claude Skill로 변환하면 "메모리 라이브러리 추천해줘" 질문 시 AI가 이 65개 목록을 자동 참조하게 만들 수 있다.

---

### Q3. API 토큰이 필요한가?

| 상황 | 토큰 필요 | 비용 |
|---|---|---|
| `AGENTS.md` 읽기 | ❌ | 무료 |
| `git clone` (public) | ❌ | 무료 |
| PR 제출 | ⚠️ GitHub 계정 | 무료 |
| **수록 프로젝트 실행** | ✅ 거의 전부 | 💰 |

실제 비용 발생 지점:

```bash
ANTHROPIC_API_KEY=sk-ant-...   # Claude
OPENAI_API_KEY=sk-...          # GPT
TAVILY_API_KEY=...             # 웹 검색
PINECONE_API_KEY=...           # 벡터 DB
```

**중요:** 에이전트는 한 작업에 LLM을 **수십 번** 호출한다.

```
사용자 요청 1회
 → 계획 수립(1) → 도구 선택(2) → 결과 판단(3) → 재시도(4) → … → 최종 답변(15)
```

#### 비용 절감 4대 원칙

1. **모델 계층 분리** — 분류/라우팅은 Haiku, 복잡 추론만 Opus → 최대 70% 절감
2. **프롬프트 캐싱** — 반복되는 시스템 프롬프트 캐싱 → 최대 90% 절감
3. **완전 로컬 옵션** — Ollama + Local Deep Researcher → API 비용 0원 (GPU 필요)
4. **지출 한도 설정** — 무한 루프 1회로 요금 폭탄. spend limit 필수

---

### Q4. 왜 GitHub에서 유명한가?

**전제:** 이 포크(`bmshin94/Awesome-AI-Agents`) 자체가 유명한 것이 아니라, **`awesome-list`라는 장르**가 유명하다.

#### 흥행 요인 5가지

1. **정보 과부하 해소** — 2023~2025년 에이전트 프로젝트 수천 개 폭증 → 큐레이션 수요 폭발
2. **진입장벽 0** — 마크다운만 쓰면 기여 가능 → 컨트리뷰터 증가 → 스타 증가 (선순환)
3. **GitHub SEO** — `awesome` 키워드 + `ai-agents` 토픽 = 검색 상위 고정
4. **"북마크 대신 스타" 심리** — 스타는 "읽었다"가 아니라 "나중에 볼게"의 의미. 큐레이션 레포가 스타를 얻기 쉬운 구조
5. **뉴스레터 성장 엔진** ← 이 저장소의 실제 전략

```
Awesome 레포 (무료 가치)
  → GitHub 검색 유입 (무료 트래픽)
    → README 내 구독 링크 (전환)
      → 뉴스레터 구독자 (자산)
        → 광고 / 스폰서 수익
```

#### 그림자

- 업데이트 중단 시 가치 급락 (본 저장소가 그 사례)
- 무검증 수록으로 인한 오류 (Luna Executor 사례)
- 스타 수 ≠ 품질 지표

---

### Q5. 로컬 에이전트 구축에 도움이 되는가?

**"부품 카탈로그"로는 유용, "조립 설명서"로는 부족.**
튜토리얼·코드 예제·벤치마크 비교·아키텍처 가이드는 전무하다.

#### 로컬 에이전트 5계층 아키텍처

```
┌─────────────────────────────────────┐
│  🖥️  UI 레이어          │ React / Next.js / Gradio
├─────────────────────────────────────┤
│  🧠  에이전트 코어      │ Agno / LangGraph / Agent Zero
├─────────────────────────────────────┤
│  💾  메모리 레이어      │ Mem0 / Letta
├─────────────────────────────────────┤
│  🔧  도구 레이어        │ MCP 서버 / browser-use
├─────────────────────────────────────┤
│  ⚡  LLM 레이어         │ Claude API 또는 Ollama(로컬)
└─────────────────────────────────────┘
```

#### 추천 조합

| 코스 | 구성 | 기간 |
|---|---|---|
| 🥇 입문 | Agno + Claude API(Haiku) + FastMCP | 1주 |
| 🥈 실전 | Agno + Mem0 + browser-use + AgentOps | 2~3주 |
| 🥉 완전 로컬 | Ollama + Local Deep Researcher + Sidekick | 2주 |

#### 리스트가 알려주지 않는 현실 문제 5가지

1. **무한 루프** — 실패→재시도 반복. `max_iterations` 필수
2. **컨텍스트 폭발** — 대화 누적 시 토큰 한도 초과. 요약/압축 전략 필수
3. **비용 폭탄** — 작업 1회 $2 × 하루 100회 = $200. spend limit 필수
4. **관측 불가** — 판단 근거 추적 불가. AgentOps 등 초기부터 도입
5. **안정성 벽** — 데모 성공률 100%, 실사용 60%. 나머지 40%가 진짜 작업량

> **핵심 조언:** 만능 에이전트가 아니라 **"업무 하나를 확실히 처리하는 작은 에이전트"** 부터 시작할 것.
> 예: "매일 아침 GitHub 이슈 요약 → Slack 전송"

---

### Q6. 수익화 아이디어가 있는가?

| 방향 | 난이도 | 수익 규모 |
|---|---|---|
| 큐레이션 · 뉴스레터 | ⭐ | 💵 |
| 리스트 → SaaS 디렉토리 | ⭐⭐⭐ | 💵💵💵 |
| 에이전트 조립 서비스 | ⭐⭐⭐⭐ | 💵💵💵💵 |
| 업종 특화 에이전트 | ⭐⭐⭐⭐⭐ | 💵💵💵💵💵 |

→ 상세는 [4장](#4-수익화-아이디어-7가지) 참조.

---

### Q7. React나 PHP로 만들 수 있는가?

**가능하다. 다만 "무엇을 만드는가"에 따라 적합도가 갈린다.**

#### 케이스 A. 이 리스트를 웹사이트로 → **React/Next.js 최적**

```
Next.js 15 (App Router)
  ├─ AGENTS.md 파싱 → JSON 변환 (빌드 타임)
  ├─ 검색: Fuse.js (퍼지 검색)
  ├─ UI: Tailwind + shadcn/ui
  ├─ GitHub API로 실시간 스타 수 표시 ← 원본에 없는 차별화 기능
  └─ 배포: Vercel
```

```tsx
// app/page.tsx — 서버 컴포넌트에서 빌드 타임 파싱
import { parseAgents } from '@/lib/parse-agents'

export default async function Home() {
  const agents = await parseAgents()          // AGENTS.md → Agent[]
  const enriched = await Promise.all(
    agents.map(async (a) => ({
      ...a,
      stars: await fetchStars(a.repo),        // 실시간 스타
      lastPush: await fetchLastPush(a.repo),  // 휴면 프로젝트 판별
    }))
  )
  return <AgentGrid agents={enriched} />
}
```

```tsx
// components/AgentGrid.tsx — 클라이언트 필터링
'use client'
export function AgentGrid({ agents }: { agents: Agent[] }) {
  const [q, setQ] = useState('')
  const [cat, setCat] = useState<Category | 'all'>('all')

  const filtered = useMemo(() =>
    agents
      .filter(a => cat === 'all' || a.category === cat)
      .filter(a => a.name.toLowerCase().includes(q.toLowerCase())),
    [agents, q, cat]
  )
  return <>{/* 검색바 + 카드 그리드 */}</>
}
```

#### 케이스 B. 에이전트 엔진 자체를 구현

| 언어 | 적합도 | 사유 |
|---|---|---|
| Python | ⭐⭐⭐⭐⭐ | 생태계 압도적 (LangGraph, Agno 등 대부분 파이썬) |
| TypeScript | ⭐⭐⭐⭐ | Vercel AI SDK, LangChain.js 등 충분히 성숙 |
| PHP | ⭐⭐ | 전용 라이브러리 희소. HTTP 직접 호출 필요 |

**권장 하이브리드 아키텍처**

```
[React/Next.js 프론트]  ←→  [PHP or Node 백엔드]  ←→  [Python 에이전트 엔진]
     화면                     인증 / 결제 / DB            추론 (FastAPI)
```

**PHP로도 충분히 가능한 범위**

```php
// Laravel + Anthropic API 직접 호출
$response = Http::withHeaders([
    'x-api-key'         => env('ANTHROPIC_API_KEY'),
    'anthropic-version' => '2023-06-01',
])->post('https://api.anthropic.com/v1/messages', [
    'model'      => 'claude-sonnet-5',
    'max_tokens' => 4096,
    'tools'      => $tools,
    'messages'   => $messages,
]);
// 도구 호출 루프는 Laravel Queue로 비동기 처리
```

PHP의 강점은 **기존 WordPress/Laravel 자산에 AI 기능을 얹고, 결제·회원 시스템과 통합**하는 지점이다.

---

## 4. 수익화 아이디어 7가지

### 💡 1. "살아있는" AI 에이전트 디렉토리
**난이도 ⭐⭐ | 기간 2~4주 | 예상 월 30~300만원**

현 저장소의 치명적 약점(17개월 정체, 깨진 링크, 중복, 오분류)을 자동화로 해결한 버전.

| 차별화 기능 | 설명 |
|---|---|
| ⭐ 실시간 스타 수 | GitHub API 일일 갱신 |
| 💀 활성도 배지 | 마지막 커밋 3개월 초과 시 "휴면" 표시 |
| 🔍 퍼지 검색 + 태그 필터 | "메모리 + 로컬실행 + MIT" 조합 검색 |
| ⚖️ 비교 테이블 | Mem0 vs Letta 병렬 비교 |
| 📊 주간 트렌드 차트 | 스타 증가율 랭킹 |
| 🔔 알림 | 관심 카테고리 신규 프로젝트 알림 |

**수익 구조 (4중 스택)**
1. 뉴스레터 스폰서 — 구독 5,000명 기준 1회 $300~800
2. 유료 등재 — "Featured" 배지 월 $50~200
3. 제휴 링크 — 클라우드/벡터DB 레퍼럴
4. 프로 구독 — API 접근 + 데이터 export, 월 $9

**로드맵**
```
Week 1: AGENTS.md → JSON 파서 + GitHub API 크롤러
Week 2: Next.js 프론트 (검색/필터/카드)
Week 3: GitHub Actions 일일 자동 갱신
Week 4: 배포 + Product Hunt 런칭
```

---

### 💡 2. 에이전트 "레시피" 유료 템플릿
**난이도 ⭐⭐⭐ | 기간 1~2개월 | 건당 $29~99**

사람들이 원하는 것은 "프로젝트 목록"이 아니라 **"바로 돌아가는 완성품"**.

| 템플릿 | 가격 | 구성 |
|---|---|---|
| 📧 이메일 분류 비서 | $39 | Agno + Gmail MCP + 분류 로직 |
| 🔍 리서치 봇 | $49 | 검색 + 요약 + Notion 저장 |
| 💬 고객문의 자동응답 | $79 | RAG + 상담 이력 메모리 |
| 🐘 Laravel용 AI 모듈 | $99 | PHP 통합 + 결제 연동 |

**필수 구성 요소**
- 완성 소스코드 (Docker 포함)
- 5분 셋업 가이드
- 환경변수 템플릿
- 비용 추정 계산기
- **실패 케이스 대응 가이드** ← 실질 가치의 핵심

판매: Gumroad / Lemon Squeezy. 무료 버전을 GitHub에 공개해 유입 확보.

---

### 💡 3. 업종 특화 에이전트 SaaS
**난이도 ⭐⭐⭐⭐⭐ | 기간 3~6개월 | 예상 월 500만~수천만원**

> 범용 에이전트는 빅테크가 이기지만, **특정 업종의 깊은 문제**는 빅테크가 건드리지 않는다.

FinRobot(금융), HuatuoGPT-o1(의료)이 이미 이 방향을 증명.

| 타겟 | 에이전트 | 가격 |
|---|---|---|
| 🏥 병의원 | 보험청구 서류 자동 검토 | 월 30만원 |
| ⚖️ 법무법인 | 계약서 리스크 자동 스캔 | 월 50만원 |
| 🛒 이커머스 | 리뷰 분석 + CS 자동응답 | 월 20만원 |
| 🏗️ 건설 | 입찰 공고 모니터링 + 요약 | 월 40만원 |
| 🏫 학원 | 학생 상담기록 분석 리포트 | 월 15만원 |

```
B2C: 월 $9 × 1,000명  = 900만원  (고객 1,000명 확보 = 매우 어려움)
B2B: 월 30만 × 20곳   = 600만원  (고객 20곳 = 현실적)
```

⚠️ 의료·법률은 규제 영역. **"AI가 판단"이 아니라 "AI가 초안, 사람이 최종 확인"** 구조 필수.

---

### 💡 4. 에이전트 비용 최적화 툴
**난이도 ⭐⭐⭐ | 예상 월 100~500만원**

에이전트의 토큰 소모량 폭증이 기업의 실질 고통 포인트.

**기능**
- 실시간 토큰 사용량 대시보드
- 에이전트별/기능별 비용 분해
- 이상 급증 알림 (무한 루프 탐지)
- "이 호출은 Haiku로 전환 시 68% 절감" 자동 제안
- 중복 호출 캐싱 추천

**강점**
- ROI 증명이 쉬움 — "월 $3,000 → $900" 숫자로 제시
- **절감액의 20% 과금** 모델 가능 → 고객 거절 사유가 없음
- AgentOps는 관측 중심, "비용 절감 제안"은 약함 → 틈새 존재

---

### 💡 5. 뉴스레터 + 콘텐츠 미디어
**난이도 ⭐ | 즉시 시작 가능 | 예상 월 50~500만원**

현 저장소가 이미 실행 중인 전략(`manuagi.beehiiv.com`).

| 구독자 | 주 수익원 | 월 예상 |
|---|---|---|
| 1,000명 | 제휴 링크 | 30만원 |
| 5,000명 | 스폰서 1회 $500 | 200만원 |
| 20,000명 | 스폰서 + 유료 티어 | 800만원+ |

**한국형 차별화**
- **한국어 큐레이션** — 영어권은 포화, 한국어는 미개척
- "한국 서비스 적용 관점" (카카오/네이버 연동, 국내 규제)
- 비용을 **원화 기준**으로 환산 제시

---

### 💡 6. 교육 / 부트캠프
**난이도 ⭐⭐ | 예상 월 100~1,000만원**

```
온라인 강의 (인프런/유데미)  : 8~15만원 × 수백명
라이브 워크샵 (4주)         : 50만원 × 20명 = 1,000만원
기업 출강                   : 일 200~500만원
전자책 + 코드                : 3~5만원
```

**커리큘럼 (본 리스트 기반)**
```
1주차: 에이전트 vs 챗봇, 5계층 아키텍처
2주차: Agno로 첫 에이전트 (도구 호출)
3주차: Mem0로 기억 붙이기
4주차: MCP 서버 직접 구현
5주차: browser-use로 웹 자동화
6주차: 비용 최적화 + 배포 + 모니터링
```

차별화 포인트: **"데모가 아니라 실패 대응까지 가르치는 강의"**

---

### 💡 7. 에이전트 구축 에이전시
**난이도 ⭐⭐⭐⭐ | 프로젝트당 500~5,000만원**

| 단계 | 내용 | 가격 |
|---|---|---|
| 🔍 진단 | 업무 분석 + 자동화 후보 도출 | 300만원 |
| 🛠️ PoC | 2주 프로토타입 | 1,000만원 |
| 🚀 구축 | 실제 배포 + 시스템 통합 | 3,000만원~ |
| 🔧 운영 | 유지보수 + 튜닝 (리테이너) | 월 200만원 |

핵심은 **운영 리테이너 계약** — 1회 구축 후 매월 안정 수익 확보.

---

### 🏆 권장 실행 로드맵

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
STEP 1 (1개월) — 아이디어 1 + 5
  "살아있는 디렉토리" 웹사이트 + 한국어 뉴스레터
  → 리스크 최소, React 역량으로 즉시 착수 가능
  → 확보한 트래픽/구독자가 이후 모든 단계의 연료
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
STEP 2 (2~3개월) — 아이디어 2 + 6
  템플릿 판매 + 강의
  → STEP 1의 트래픽을 직접 현금화
  → "고객이 실제로 원하는 것" 데이터 확보
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
STEP 3 (6개월~) — 아이디어 3 또는 7
  업종 특화 SaaS 또는 에이전시
  → STEP 2에서 발견한 "진짜 아픈 문제"로 직행
  → 최대 수익, 최대 진입장벽(해자)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### 💎 핵심 원칙

> **"AI 에이전트"를 팔지 말고 "해결된 문제"를 팔 것.**
>
> ❌ "최신 멀티에이전트 오케스트레이션을 제공합니다"
> ✅ "매일 2시간 걸리던 견적서 작성이 5분이 됩니다"
>
> 고객은 기술이 아니라 **되찾은 시간**에 비용을 지불한다.

---

## 5. 수록 프로젝트 전체 링크

> 출처: `AGENTS.md` (2025-04-08 기준, 총 65개 항목 / 중복 포함)

### 🤖 범용 에이전트 프레임워크
- [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT)
- [MetaGPT](https://github.com/geekan/MetaGPT)
- [Agno](https://github.com/agno-agi/agno)
- [Agent Zero](https://github.com/frdel/agent-zero)
- [AutoAgent](https://github.com/HKUDS/AutoAgent)
- [Archon](https://github.com/coleam00/Archon)
- [LangManus](https://github.com/langmanus/langmanus)
- [TEN Agent](https://github.com/TEN-framework/TEN-Agent)
- [Qwen-Agent](https://github.com/QwenLM/Qwen-Agent)
- [ZerePy](https://github.com/blorm-network/ZerePy)
- [Multi-Agent Orchestrator](https://github.com/awslabs/multi-agent-orchestrator)
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python)
- [GenAI Agents](https://github.com/NirDiamant/GenAI_Agents) *(중복 등재)*

### 🧠 메모리 / 기억 레이어
- [Mem0](https://github.com/mem0ai/mem0)
- [Letta (구 MemGPT)](https://github.com/letta-ai/letta)
- [Supermemory](https://github.com/supermemoryai/supermemory)
- [KBLaM](https://github.com/microsoft/KBLaM)

### 🔌 MCP 생태계
- [FastMCP](https://github.com/jlowin/fastmcp)
- [MCP-Go](https://github.com/mark3labs/mcp-go)
- [MCP-Agent](https://github.com/lastmile-ai/mcp-agent)
- [Playwright MCP Server](https://github.com/executeautomation/mcp-playwright)

### 🌐 브라우저 / 컴퓨터 조작
- [Browser-use](https://github.com/browser-use/browser-use)
- [Browser-use WebUI](https://github.com/browser-use/web-ui)
- [Steel Browser](https://github.com/steel-dev/steel-browser)
- [Open Interface](https://github.com/AmberSahdev/Open-Interface)
- [Agent.exe](https://github.com/corbt/agent.exe)
- [AutoMate](https://github.com/yuruotong1/autoMate)
- [Page Assist](https://github.com/n4ze3m/page-assist)
- [AppAgent (mnotgod96)](https://github.com/mnotgod96/AppAgent)
- [AppAgent (FigmaAI)](https://github.com/FigmaAI/AppAgent) *(중복 등재)*

### 👨‍💻 코딩 / 개발 자동화
- [OpenHands](https://github.com/All-Hands-AI/OpenHands)
- [GPT Pilot](https://github.com/Pythagora-io/gpt-pilot)
- [PR-Agent](https://github.com/Codium-ai/pr-agent)
- [CopilotKit](https://github.com/CopilotKit/CopilotKit)
- [Codename Goose](https://github.com/deepseek-ai/codename-goose) *(⚠️ 출처 오류 — 실제는 `block/goose`)*
- [Integuru](https://github.com/Integuru-AI/Integuru)
- [Prompt-To-Agent (potpie)](https://github.com/potpie-ai/potpie)
- [VisionAgent](https://github.com/landing-ai/vision-agent)
- [RDAgent](https://github.com/microsoft/RD-Agent)

### 🔒 로컬 / 프라이버시
- [Local Deep Researcher](https://github.com/langchain-ai/local-deep-researcher)
- [Sidekick](https://github.com/johnbean393/Sidekick)
- [TinyAgent](https://github.com/SqueezeAILab/TinyAgent)
- [Terminal GPT](https://github.com/Simatwa/python-tgpt)

### 🏢 산업 특화
- [FinRobot](https://github.com/AI4Finance-Foundation/FinRobot) — 금융
- [HuatuoGPT-o1](https://github.com/FreedomIntelligence/HuatuoGPT-o1) — 의료
- [LeRobot](https://github.com/huggingface/lerobot) — 로보틱스
- [The AI Scientist](https://github.com/SakanaAI/AI-Scientist) — 연구 자동화
- [Executive AI Assistant](https://github.com/langchain-ai/executive-ai-assistant) — 비서 업무

### 📊 운영 / 평가 / 관측
- [AgentOps](https://github.com/AgentOps-AI/agentops)
- [Agenta](https://github.com/agenta-ai/agenta)
- [TheAgentCompany](https://github.com/TheAgentCompany/TheAgentCompany)
- [LARS](https://github.com/abgulati/LARS)

### 🎙️ 실시간 / 음성 / 멀티모달
- [LiveKit Agents](https://github.com/livekit/agents)
- [Realtime API Agents](https://github.com/openai/openai-realtime-agents)
- [CSM](https://github.com/SesameAILabs/csm)

### 💬 UI / 챗 인터페이스
- [Agent Chat UI](https://github.com/langchain-ai/agent-chat-ui)
- [Chat Nio](https://github.com/zmh-program/chatnio)
- [AstrBot](https://github.com/Soulter/AstrBot)
- [DuckDuckGPT](https://github.com/KudoAI/duckduckgpt)
- [Giselle](https://github.com/giselles-ai/giselle)

### 📚 학습 / 템플릿
- [AI Agents for Beginners](https://github.com/microsoft/ai-agents-for-beginners)
- [LangGraph Retrieval Agent Template](https://github.com/langchain-ai/retrieval-agent-template-js)

### 🌐 기타 / 분류 주의
- [Farcaster Agent](https://github.com/0xKoda/fagent) — 탈중앙 소셜
- [Luna Executor](https://github.com/secondlathloothy/Luna-Executor) — ⚠️ **AI 에이전트 아님. 로블록스 스크립트 실행기**

---

## 📎 참고 링크

| 항목 | URL |
|---|---|
| 본 저장소 | https://github.com/bmshin94/Awesome-AI-Agents |
| 원본(포크 출처) | https://github.com/ChatTeach/Awesome-AI-Agents |
| 프로젝트 목록 | https://github.com/bmshin94/Awesome-AI-Agents/blob/main/AGENTS.md |
| 기여 가이드 | https://github.com/bmshin94/Awesome-AI-Agents/blob/main/CONTRIBUTING.md |
| 뉴스레터 | https://manuagi.beehiiv.com/subscribe |
| Model Context Protocol | https://modelcontextprotocol.io |

---

*본 문서는 2026-09-18 기준 저장소 상태를 분석한 결과다. `AGENTS.md`의 콘텐츠는 2025-04-08 이후 갱신되지 않았으므로, 각 프로젝트의 현재 상태는 원본 저장소에서 별도 확인이 필요하다.*
