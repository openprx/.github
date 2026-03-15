<div align="center">

<img src="https://raw.githubusercontent.com/openprx/site/main/public/brand-assets/icon-48.svg" width="64" height="64" alt="OpenPRX" />

# OpenPRX

**AI-native development infrastructure. Open source. Built with Rust & Go.**

[Website](https://openprx.dev) · [GitHub](https://github.com/openprx)

---

</div>

## Projects

### 🔧 [OpenPR](https://github.com/openprx/openpr)
Open-source project management platform with built-in governance, AI agent integration, and MCP support.  
**Tech:** Rust (Axum + SeaORM) · SvelteKit · PostgreSQL  
**Highlights:** Issues & Kanban · Sprint planning · Governance center (proposals, voting, trust scores) · MCP server with 34 tools across 3 protocols (HTTP, stdio, SSE) · Bot token auth · File attachments

### 🤖 [PRX](https://github.com/openprx/prx)
Self-evolving AI assistant framework with multi-provider inference and governed sub-agents.  
**Tech:** Rust  
**Highlights:** 14 AI providers · 19 messaging channels · Self-evolution system (~9,500 lines) · OAuth auto-refresh · Governed sub-agents · Production-hardened security

### 🧠 [prx-memory](https://github.com/openprx/prx-memory)
Local-first MCP memory component for coding agents. Store, recall, evolve.  
**Tech:** Rust  
**Highlights:** stdio + HTTP transport · Full toolchain (store, recall, update, forget, evolve) · Governance controls · Hybrid retrieval (lexical + vector + rerank) · Works with Codex, Claude Code, OpenClaw

### 📦 [Fenfa](https://github.com/openprx/fenfa)
Self-hosted app distribution platform. Upload builds, get install pages with QR codes, manage releases.  
**Tech:** Go · SQLite · Embedded frontend  
**Highlights:** Multi-platform (iOS/Android/macOS/Windows/Linux) · iOS UDID binding · Apple Developer API integration · S3/R2 storage · Single binary deployment · i18n (EN/ZH)

### 💬 [wacli](https://github.com/openprx/wacli)
WhatsApp JSON-RPC daemon for programmatic messaging.  
**Tech:** Go  
**Highlights:** JSON-RPC API · Multi-session · Webhook integration · Lightweight daemon

---

<div align="center">

**Manage → Operate → Remember → Distribute → Connect**

```
┌─────────────┐     MCP      ┌─────────────┐
│   OpenPR    │◄────────────►│     PRX     │
│  (Manage)   │              │  (Operate)  │
└──────┬──────┘              └──────┬──────┘
       │                            │
       └──────────┬─────────────────┘
                  │
     ┌────────────┼────────────┐
     ▼            ▼            ▼
┌──────────┐ ┌──────────┐ ┌──────────┐
│prx-memory│ │  Fenfa   │ │  wacli   │
│(Remember)│ │(Distrib.)│ │(Connect) │
└──────────┘ └──────────┘ └──────────┘
```

MIT OR Apache-2.0 Licensed · [openprx.dev](https://openprx.dev)

</div>
