# Hi there, I'm uptodatelabs 👋

**Solo founder building useful open source tools.**
I believe small teams can make a big impact.

[![Sponsor](https://img.shields.io/badge/Sponsor-uptodatelabs-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/uptodatelabs)
[![Ko-fi](https://img.shields.io/badge/Ko--fi-Buy_me_a_coffee-FF5E5B?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/uptodatelabs)
[![Website](https://img.shields.io/badge/Website-uptodatelabs.vercel.app-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://uptodatelabs.vercel.app/)

---

## 🧭 What I do

I build **developer tools for the AI coding agent ecosystem** — the plumbing that makes
Claude Code, Cursor, Copilot and friends actually usable in real projects.

Everything here is **local-first**, open source, and shipped as a real package
(npm / PyPI), not just a demo.

---

## ⭐ Flagship: CodeNexus

> A local-first context engine for AI coding agents.

CodeNexus builds a dependency graph of your codebase and feeds the agent **only the
context it needs** — instead of the whole repo. In my own benchmarks this cut prompt
tokens from ~951K to ~4.3K on a large project (your mileage will vary).

📦 `pip install codenexus-ai` · 🔗 [CodeNexus](https://github.com/uptodatelabs/CodeNexus)

---

## 🛠 Toolbox

### AI coding agent tools

| Project | Stack | What it does | Install |
|---|---|---|---|
| [**CodeNexus**](https://github.com/uptodatelabs/CodeNexus) | Python | Local-first context engine — token cost slashed by feeding only relevant code | `pip install codenexus-ai` |
| [**agent-wizard**](https://github.com/uptodatelabs/agent-wizard) | TypeScript | Setup wizard for AI coding assistant configs (Cursor, Claude Code, Copilot, aider…) | `npm i -g agent-wizard` |
| [**claude-api-manager**](https://github.com/uptodatelabs/claude-api-manager) | TypeScript | Switch Claude Code API profiles from a TUI dashboard (`cam`) | `npm i -g claude-api-manager` |
| [**claude-session-manager**](https://github.com/uptodatelabs/claude-session-manager) | TypeScript | Browse, search, resume, back up and restore Claude Code sessions (`csm`) | — |
| [**api_tester**](https://github.com/uptodatelabs/api_tester) | Python | TUI tester for OpenAI/Anthropic-compatible endpoints — auto-detect + latency | `pip install apiprobe` |

### Desktop utilities

| Project | Stack | What it does |
|---|---|---|
| [**screen-recorder**](https://github.com/uptodatelabs/screen-recorder) | Python | Buffer-based recorder — hotkey saves the last N seconds of gameplay to MP4 |
| [**eye-care**](https://github.com/uptodatelabs/eye-care) | Electron | Eye exercise reminders as an overlay (optometrist-recommended movements) |
| [**gpt-image-maker**](https://github.com/uptodatelabs/gpt-image-maker) | HTML | Zero-dependency GPT Image generator — runs entirely in the browser |

---

## 💖 Sponsorship

If any of these tools saved you time or tokens, sponsoring helps me keep them
maintained and free.

**Where sponsorship money goes:**
- ⏱ Actual maintenance time — issue triage, releases, cross-platform testing
- 🧪 New experiments in the AI agent tooling space
- 📚 Documentation in **English and Korean**
- 🖥 Infrastructure (CI/CD, domains, hosting)

Sponsors get listed in [SPONSORS.md](./SPONSORS.md) (unless you prefer to stay anonymous — just say so).

---

## 📬 Reach me

- 🌐 [uptodatelabs.vercel.app](https://uptodatelabs.vercel.app/)
- 💬 Open an issue on the repo you use — that's the fastest way to reach me

---

<details>
<summary>🇰🇷 한국어</summary>

안녕하세요, **uptodatelabs**입니다. 혼자서 유용한 오픈소스 도구를 만드는 솔로 파운더입니다.
작은 팀도 큰 영향을 만들 수 있다고 믿습니다.

주력 분야는 **AI 코딩 에이전트 개발자 도구**입니다. Claude Code, Cursor, Copilot 같은
도구가 실제 프로젝트에서 쓸모 있게 동작하도록 만드는 데 집중하고 있습니다.

여기의 모든 프로젝트는 **로컬 우선(local-first)** 설계이며, 데모가 아니라 npm / PyPI로
실제 배포되는 패키지입니다.

플래그십은 **CodeNexus**입니다. 코드베이스의 의존성 그래프를 만들어 에이전트에
**필요한 컨텍스트만** 전달합니다. 자체 벤치마크에서 대형 프로젝트 기준 프롬프트 토큰이
약 951K에서 4.3K로 줄었습니다 (환경에 따라 결과가 다를 수 있습니다).

이 도구들이 시간이나 토큰 비용을 절약해줬다면, 후원은 유지보수와 새로운 실험,
그리고 영/한 문서 작성에 그대로 쓰입니다. 후원은 [github.com/sponsors/uptodatelabs](https://github.com/sponsors/uptodatelabs) 또는 [ko-fi.com/uptodatelabs](https://ko-fi.com/uptodatelabs)에서 가능합니다.

</details>

---

<sub>⭐ Star a repo if it helped — it's free and it genuinely helps a solo maintainer get discovered.</sub>
