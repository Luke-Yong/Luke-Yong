# Harness

> A sovereign agentic IDE — DeepSeek-native, zero Western cloud dependencies.

## Why this exists

DeepSeek's models are state-of-the-art, but they lack a proper development environment.
Existing tools chain together SaaS wrappers and cloud APIs that are one sanction away from
disappearing. Harness is the opposite: a single desktop application where DeepSeek controls
a real IDE — files, terminals, browser, and diagnostics — with nothing between it and the machine.

**No wrappers. No third-party SaaS. 6 server-side runtime dependencies.** Every component
is built from the ground up: the agent loop, the tool registry, the LSP bridge, the terminal
manager, the browser sandbox.

## What it does

- **Agentic coding**: DeepSeek drives the entire IDE — reads files, writes code, runs builds,
  debugs errors, and iterates autonomously in a tool-calling loop with history compaction
- **Built-in browser**: The agent navigates web apps, inspects DOM elements, clicks, types,
  and reads console output — all through text-based DOM snapshots (no expensive visual screenshots)
- **Dynamic instruction retrieval**: 14 themed prompt chunks assembled per-turn based on
  conversation context, cutting system prompt tokens by up to **95%**
- **Real terminal**: PTY-backed shell sessions with automatic venv activation and
  localhost URL detection
- **LSP diagnostics**: 25+ language servers auto-detected and wired into Monaco Editor
- **Desktop-ready**: Electron shell with native file dialogs, geolocation, and tabbed browsing
- **Sub-agent delegation**: Spawn focused sub-agents with isolated context windows for
  parallel research tasks
- **Persistent memory**: SQLite-backed cross-session recall of project conventions,
  user preferences, and key decisions

---

**✅ MVP ready** — core loop is stable, tool-calling works end-to-end, and the agent can
autonomously complete real-world coding and browser automation tasks.

Built for [@deepseek-ai](https://github.com/deepseek-ai) — designed to showcase
what DeepSeek models can do when given a real, sovereign IDE environment.
