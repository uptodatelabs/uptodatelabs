# Hi there, I'm uptodatelabs 👋

**Solo founder building developer tools for the AI coding agent ecosystem.**
I believe small teams can make a big impact.

[![Sponsor](https://img.shields.io/badge/Sponsor-uptodatelabs-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/uptodatelabs)
[![Ko-fi](https://img.shields.io/badge/Ko--fi-Buy_me_a_coffee-FF5E5B?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/uptodatelabs)
[![Website](https://img.shields.io/badge/Website-uptodatelabs.vercel.app-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://uptodatelabs.vercel.app/)
[![Blog](https://img.shields.io/badge/Blog-25_guides_·_EN_%2B_KO-1f6feb?style=for-the-badge&logo=markdown&logoColor=white)](https://uptodatelabs.vercel.app/blog)

---

## 🧭 What I do

I build **the plumbing that makes Claude Code, Cursor, Copilot and friends actually usable in
real projects** — context, configuration, sessions, cost.

Everything here is **local-first**, open source, and shipped as a real artifact
(npm / PyPI / Windows installer) rather than a demo.

- **10 public tools**, MIT-licensed (one exception noted below)
- **25 long-form guides**, each published in **English and Korean**
- Built and maintained by one person, in public

---

## ⭐ Flagship: CodeNexus

> A local-first context engine for AI coding agents.

CodeNexus builds a dependency graph of your repository into SQLite and hands the agent **only the
files that matter** — instead of the whole repo. On a 211-file project this measured
**951K → ~4.3K prompt tokens** (about 99% fewer; your mileage will vary by project shape).

It speaks **MCP over stdio**, so it drops into Claude Code, Cursor and Zed as a context server,
and it indexes 7 languages.

📦 `pip install codenexus-ai` · 🔗 [CodeNexus](https://github.com/uptodatelabs/CodeNexus)

---

## 🛠 Toolbox

### AI agent tooling

| Project | Stack | What it does | Install |
|---|---|---|---|
| [**CodeNexus**](https://github.com/uptodatelabs/CodeNexus) | Python · MCP · SQLite | Context engine — serves only the relevant code, up to ~99% fewer context tokens | `pip install codenexus-ai` |
| [**agent-wizard**](https://github.com/uptodatelabs/agent-wizard) | TypeScript | One CLI that configures Claude Code, Cursor, Copilot, Aider, OpenClaw and Hermes — detects your stack, keeps each setup as a named profile, syncs across machines | `npm i -g agent-wizard` |
| [**claude-api-manager**](https://github.com/uptodatelabs/claude-api-manager) | JavaScript · Ink | Unlimited named API profiles (Anthropic, Bedrock, Vertex, Foundry, proxies) with a diff preview, then one-keystroke swap of the whole `env` block (`cam`) | `npm i -g claude-api-manager` |
| [**claude-session-hub**](https://github.com/uptodatelabs/claude-session-hub) | TypeScript · Ink | The missing file manager for Claude Code conversations — list, search, resume, trash, back up and restore sessions, plus per-session token accounting (`cshub`) | `git clone` + `npm link` |
| [**apiprobe**](https://github.com/uptodatelabs/api_tester) | Python · Textual | TUI that fingerprints OpenAI/Anthropic-compatible endpoints, infers context and max-token limits, and measures real connection latency | `pip install apiprobe` |
| [**ssh-file-explorer**](https://github.com/uptodatelabs/ssh-file-explorer) | Python (stdlib only) | Browse, edit, upload and download files on a remote box from your local browser — one file, token auth on by default, binds to 127.0.0.1 | `pip install ssh-file-explorer` |

### Desktop & local utilities

| Project | Stack | What it does |
|---|---|---|
| [**WallMagic**](https://github.com/uptodatelabs/WallMagic) | Rust · Tauri v2 · React 19 | Windows wallpaper studio — search, generate, apply and restore. Native per-monitor COM apply, snapshot restore so a failure never leaves a black desktop, 5 BYOK image providers |
| [**Game Recorder**](https://github.com/uptodatelabs/screen-recorder) | Python · dxcam | Buffer-based recorder — keeps the last N seconds in memory and a hotkey saves only the highlight. DXGI Desktop Duplication at refresh rate |
| [**Eye Care**](https://github.com/uptodatelabs/eye-care) | Electron · JavaScript · SVG | Overlays **guided** eye exercises (AAO/AOA-derived, animated SVG) instead of nagging you to take a break. Explicitly not a medical device |
| [**GPT Image Maker**](https://github.com/uptodatelabs/gpt-image-maker) | HTML + JavaScript · Puter.js | Zero-dependency local image workbench — text-to-image, image-to-image with up to 10 references, test mode that spends no credits |

<sub>License: MIT across the board. Exception — **apiprobe** ships no declared license file yet, so treat it as "all rights reserved" until that is fixed. `Game Recorder` is published from the `screen-recorder` repo.</sub>

---

## ✍️ Writing — 25 guides, English + Korean

Long-form, hands-on comparisons rather than press-release summaries. Everything below is live at
[**uptodatelabs.vercel.app/blog**](https://uptodatelabs.vercel.app/blog); every guide has a Korean
counterpart at `/blog/ko/<slug>`. Thirteen of the twenty-five are highlighted below — the full
index (pricing, comparisons, tutorials, trends) is on the hub page.

**Pricing & value**
- [AI Coding Tool Price Comparison 2026 — Cursor, Claude, Copilot, Codex](https://uptodatelabs.vercel.app/blog/ai-coding-tools-price-comparison-2026)
- [Claude Code Pricing Explained + Practical Token-Saving Tips](https://uptodatelabs.vercel.app/blog/claude-code-pricing-guide)
- [ChatGPT Plus vs Claude Pro vs Gemini Advanced](https://uptodatelabs.vercel.app/blog/chatgpt-plus-vs-claude-pro-vs-gemini-advanced)
- [12 Ways to Cut Your AI API Costs (Caching, Routing, and More)](https://uptodatelabs.vercel.app/blog/reduce-ai-api-costs)

**Agent comparison & reviews**
- [Claude Code vs OpenCode: 2026 Hands-On Comparison](https://uptodatelabs.vercel.app/blog/claude-code-vs-opencode)
- [Claude Code vs Cursor: Terminal-First or Editor-First](https://uptodatelabs.vercel.app/blog/claude-code-vs-cursor)
- [Best AI Coding Agents 2026: Recommendations by Use Case](https://uptodatelabs.vercel.app/blog/best-ai-coding-agents-2026)
- [Free AI Coding Agents: 7 Open-Source Tools We Tested](https://uptodatelabs.vercel.app/blog/free-ai-coding-agents)

**Build & operate agents**
- [Build an MCP Server — From Concept to First Server Code](https://uptodatelabs.vercel.app/blog/mcp-server-tutorial)
- [Build a RAG Agent — Hands-on Document Q&A](https://uptodatelabs.vercel.app/blog/rag-agent-tutorial)
- [AI Agent Framework Comparison — LangChain vs LlamaIndex vs AutoGen](https://uptodatelabs.vercel.app/blog/langchain-vs-llamaindex-vs-autogen)

**Trends**
- [2026 AI Coding Agent Trends — What Actually Changed](https://uptodatelabs.vercel.app/blog/ai-coding-agent-trends-2026)
- [AI Agent Market Outlook & Real Adoption Cases](https://uptodatelabs.vercel.app/blog/ai-agent-market-outlook)

---

## 🔐 Also shipping (commercial)

[**Memora**](https://uptodatelabs.vercel.app/memora) — an encrypted memory aid and credential vault
for Windows. Zero-knowledge by design: AES-256-GCM with Argon2id key derivation, TOTP two-factor
unlock, and encrypted-blob sync over GitHub / Drive / OneDrive. Nothing is readable server-side —
including by me. Closed source, paid, not part of the MIT set above.

---

## 💖 Sponsorship

If any of these tools saved you time or tokens, sponsoring helps me keep them maintained and free.

**Where sponsorship money actually goes:**
- ⏱ Maintenance time — issue triage, releases, cross-platform testing
- 🧪 New experiments in agent tooling (context, sessions, cost control)
- 📚 Documentation in **English and Korean**
- 🖥 Infrastructure (CI/CD, domains, hosting)

Sponsors are listed in `SPONSORS.md` in this repo — unless you prefer to stay anonymous, just say so.

---

## 📬 Reach me

- 🌐 [uptodatelabs.vercel.app](https://uptodatelabs.vercel.app/)
- ✍️ [Blog — /blog](https://uptodatelabs.vercel.app/blog)
- 💬 Open an issue on the repo you use — that is the fastest way to reach me

---

<details>
<summary>🇰🇷 한국어</summary>

안녕하세요, **uptodatelabs**입니다. 혼자서 개발자 도구를 만드는 솔로 파운더입니다.
작은 팀도 큰 영향을 만들 수 있다고 믿습니다.

주력 분야는 **AI 코딩 에이전트 생태계의 기반 도구**입니다. Claude Code, Cursor, Copilot 같은
도구가 실제 프로젝트에서 쓸모 있게 동작하도록 — 컨텍스트, 설정, 세션, 비용 — 을 다룹니다.
여기의 모든 프로젝트는 **로컬 우선(local-first)** 이며, 데모가 아니라 npm / PyPI / Windows
설치 파일로 실제 배포되는 산출물입니다.

**공개 도구 10개**(전부 MIT, 예외는 아래 표기)와 **영/한 병행 롱폼 가이드 25편**을 운영하고
있습니다. 한 사람이 공개적으로 유지보수합니다.

**플래그십은 CodeNexus**입니다. 코드베이스의 의존성 그래프를 SQLite에 만들어 에이전트에
**필요한 파일만** 전달합니다. 211개 파일 프로젝트에서 프롬프트 토큰이 **951K → 약 4.3K**로
측정되었습니다(약 99% 감소, 프로젝트 구조에 따라 달라질 수 있습니다). MCP stdio로
Claude Code·Cursor·Zed에 컨텍스트 서버로 붙고, 7개 언어를 인덱싱합니다.

**AI 에이전트 도구**: CodeNexus(컨텍스트 엔진) · agent-wizard(여러 도구 설정을 이름 있는
프로필로 관리·동기화) · claude-api-manager(API 프로필 무제한 저장 + diff 미리보기 후 한 번에
전환) · claude-session-hub(세션 목록·검색·재개·휴지통·백업 + 세션별 토큰 집계) ·
apiprobe(LLM 엔드포인트 판별·한도 추론·지연 측정) · ssh-file-explorer(파이썬 표준 라이브러리만
쓰는 단일 파일 웹 파일 탐색기).

**데스크톱·로컬 유틸**: WallMagic(윈도우 배경화면 스튜디오 — 모니터별 적용, 실패 시 원복,
BYOK 이미지 제공자 5종) · Game Recorder(마지막 N초를 메모리에 두고 핫키로 하이라이트만 저장) ·
Eye Care(안구 운동을 애니메이션으로 안내하는 오버레이, 의료기기 아님) · GPT Image Maker
(의존성 없는 로컬 이미지 생성 워크벤치).

**글쓰기**: [uptodatelabs.vercel.app/blog](https://uptodatelabs.vercel.app/blog) 에 25편의
가이드를 영/한으로 발행합니다. 가격 비교, 에이전트 비교·리뷰, MCP·RAG·프레임워크 구축 실습,
그리고 트렌드 정리입니다. 한국어판은 같은 슬러그의 `/blog/ko/<slug>` 경로에 있습니다.

**상용 제품**: [Memora](https://uptodatelabs.vercel.app/memora) — 윈도우용 암호화 메모리·자격
증명 보관함. AES-256-GCM + Argon2id, TOTP 2단계, GitHub/Drive/OneDrive로 암호화 블롭 동기화.
서버에서는(운영자조차) 내용을 읽을 수 없는 zero-knowledge 설계입니다. 클로즈드 소스 유료입니다.

이 도구들이 시간이나 토큰을 절약해줬다면, 후원은 유지보수·새 실험·영/한 문서 작성에 그대로
쓰입니다. [github.com/sponsors/uptodatelabs](https://github.com/sponsors/uptodatelabs) 또는
[ko-fi.com/uptodatelabs](https://ko-fi.com/uptodatelabs) 에서 가능합니다.

</details>

---

<sub>⭐ Star a repo if it helped — it's free and it genuinely helps a solo maintainer get discovered.</sub>
