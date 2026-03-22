<div align="center">

<img src="https://raw.githubusercontent.com/openprx/site/main/public/brand-assets/icon-48.svg" width="64" height="64" alt="OpenPRX" />

# OpenPRX

**Open-source pipeline for AI-autonomous software engineering.**

AI agents plan work, write code, distribute builds, and defend production — governed, auditable, and fully open source.

[Website](https://openprx.dev) · [Docs](https://docs.openprx.dev) · [Community](https://community.openprx.dev) · [GitHub](https://github.com/openprx)

---

</div>

## The Pipeline

### 1. Plan — [OpenPR](https://github.com/openprx/openpr)
AI-native project management. Issues, boards, sprints, governance, and a 34-tool MCP server that lets AI agents create tasks, vote on proposals, and manage projects.
**Tech:** Rust (Axum) · SvelteKit · PostgreSQL
**Key numbers:** 38 database tables · 34 MCP tools · 3 transports (HTTP, stdio, SSE) · 30 webhook event types

### 2. Think — [PRX](https://github.com/openprx/prx)
The AI brain. Routes conversations across 19 messaging channels and 14 LLM providers. Self-evolving architecture that improves its own behavior through governed feedback loops.
**Tech:** Rust
**Key numbers:** 19 channels · 14 providers ·  5-layer security pipeline

### 3. Build — [prx-memory](https://github.com/openprx/prx-memory) · [openpr-webhook](https://github.com/openprx/openpr-webhook)
Code generation agents with persistent memory. The webhook dispatcher turns OpenPR events into coding tasks; prx-memory gives agents a local-first MCP memory layer with hybrid retrieval.
**Tech:** Rust
**Key numbers (prx-memory):** 14 MCP tools · lexical + vector + rerank retrieval · MSES evolution scoring

### 4. Ship — [Fenfa](https://github.com/openprx/fenfa)
Self-hosted app distribution. Upload builds, get install pages with QR codes, manage releases across 5 platforms.
**Tech:** Go · SQLite · Vue
**Key numbers:** iOS/Android/macOS/Windows/Linux · Apple Developer API integration · S3/R2 storage

### 5. Protect — [PRX-WAF](https://github.com/openprx/prx-waf) · [PRX-SD](https://github.com/openprx/prx-sd)
Production defense. PRX-WAF is a 17-phase web application firewall built on Pingora. PRX-SD is an antivirus engine with hash matching, YARA rules, and heuristic analysis.
**Tech:** Rust
**Key numbers (WAF):** 17 processing phases · 644+ built-in rules · OWASP CRS · GeoIP · bot detection
**Key numbers (SD):** 5 threat intel sources · 64 built-in YARA rules · PE/ELF/MachO heuristics

---

<div align="center">

```
Plan            Think           Build           Ship            Protect
 │               │               │               │               │
 ▼               ▼               ▼               ▼               ▼
┌──────┐  MCP  ┌──────┐ events ┌──────────┐    ┌──────┐    ┌─────────┐
│OpenPR│◄─────►│ PRX  │───────►│ Webhook  │    │Fenfa │    │ PRX-WAF │
│      │       │      │       │ Dispatch │    │      │    │ PRX-SD  │
└──────┘       └──────┘       └────┬─────┘    └──────┘    └─────────┘
                                   │
                              ┌────▼─────┐
                              │prx-memory│
                              └──────────┘
```

</div>

## Supporting Repos

| Repo | Description |
|------|-------------|
| [prx-sd-signatures](https://github.com/openprx/prx-sd-signatures) | Threat intelligence database for PRX-SD (hash signatures + YARA rules) |
| [prx_email](https://github.com/openprx/prx_email) | Email plugin for PRX (IMAP/SMTP) |
| [voice_talk_realtime](https://github.com/openprx/voice_talk_realtime) | Browser-side real-time voice conversation via WebAssembly |
| [wacli](https://github.com/openprx/wacli) | WhatsApp CLI — fork with added JSON-RPC and webhook features |
| [homebrew-tap](https://github.com/openprx/homebrew-tap) | Homebrew tap for macOS/Linux |
| [scoop-bucket](https://github.com/openprx/scoop-bucket) | Scoop bucket for Windows |
| [site](https://github.com/openprx/site) | openprx.dev website source |

<div align="center">

MIT OR Apache-2.0 Licensed · [openprx.dev](https://openprx.dev) · [Docs](https://docs.openprx.dev) · [Community](https://community.openprx.dev)

</div>
