# Awesome DeepSeek Harness Plugins [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated collection of plugins, tools, and integrations for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) (`dsh`) — the open-source agent harness by DeepSeek AI where **everything is a plugin**.

DeepSeek Harness is built on an architecture where every capability — tools, UI, memory, orchestration — is a [Cordis](https://github.com/cordiverse/cordis) plugin. This list tracks the best community plugins and ecosystem projects.

**Find more:** add the [`dsh-plugin`](https://github.com/topics/dsh-plugin) topic to your repo for discoverability.

**Website:** browse the searchable catalog at **[awesome-deepseek-harness-plugins.pages.dev](https://awesome-deepseek-harness-plugins.pages.dev/)** (source in [`website/`](website/), built with Astro + Bun, hosted on Cloudflare Pages — redeploy with `cd website && bun run deploy`).

## Contents

- [Official](#official)
- [Tool Plugins](#tool-plugins)
  - [Search & Web](#search--web)
  - [Vision](#vision)
  - [Browser & Computer Use](#browser--computer-use)
  - [Files & Editing](#files--editing)
- [Memory & Context](#memory--context)
- [Orchestration & Agents](#orchestration--agents)
- [UI & Interfaces](#ui--interfaces)
  - [Terminal UIs](#terminal-uis)
  - [Web UI Enhancements](#web-ui-enhancements)
  - [Desktop Clients & Distros](#desktop-clients--distros)
  - [Skins & Fun](#skins--fun)
- [Observability & Cost](#observability--cost)
- [Integrations & Apps](#integrations--apps)
- [Plugin Development & Utilities](#plugin-development--utilities)
- [Learning Resources](#learning-resources)
- [Related Lists](#related-lists)

## Official

- [deepseek-harness](https://github.com/deepseek-ai/deepseek-harness) - The official DeepSeek Harness runtime. Run it with `npx @deepseek-ai/dsh web`.

## Tool Plugins

### Search & Web

- [modsearch](https://github.com/liustack/modsearch) - Web plugin for DeepSeek Harness: ask the web or X, get structured results.
- [argo](https://github.com/taxueseek/argo) - Multilingual search built for agents, covering CN/EN, academic, code, shopping, finance, and news.

- [anysearch-dsh](https://github.com/anysearch-team/anysearch-dsh) - AnySearch web-search provider and advanced search tools for DeepSeek Harness.
- [anime-find](https://github.com/cocofhu/anime-find) - An anime search plugin for DeepSeek Harness: multi-source within-conversation search with card display (Bangumi/Mikan).
- [dsh-free-search](https://github.com/DDDMUC/dsh-free-search) - A free web-search provider for DeepSeek Harness — DuckDuckGo backend, no API key needed.
- [dsh-web-search-pro](https://github.com/anweat/dsh-web-search-pro) - An enhanced, persistent multi-engine web search plugin for DeepSeek Harness.
- [SpecFusion](https://github.com/wxkingstar/SpecFusion) - Search Chinese API docs and build specifications directly inside DeepSeek Harness, Claude Code, Cursor, Codex, and Gemini CLI.
- [dsh-scholar](https://github.com/lzszq/dsh-scholar) - A scholarly search plugin for DeepSeek Harness.

### Vision

- [modlens](https://github.com/liustack/modlens) - The first vision plugin for DeepSeek Harness — paste an image, get analysis; a vision bridge for text-only coding agents.
- [dsh-vision-toolkit](https://github.com/Anionex/dsh-vision-toolkit) - Vision toolkit for text-only models: intent-aware image Q&A, long-screenshot OCR, and UI restoration.
- [dsh-vision](https://github.com/william-jin-cmu/dsh-vision) - `view_image` tool bridging any OpenAI-compatible VLM (works with free tiers).
- [dsh-vision-router](https://github.com/ysr666/dsh-vision-router) - Built-in keyless vision chain plus pixel-level tools (Q&A, grounding) for text-only agents.
- [dsh-draw](https://github.com/PerryLink/dsh-draw) - Unified static-image generation routing for DeepSeek Harness: one image_generate tool across OpenAI Images, Zhipu CogView, and compatible endpoints, with health-aware fallback and durable results.

- [dsh-image-gen](https://github.com/shanliuling/dsh-image-gen) - Generate images directly in DeepSeek Harness chats (Gemini, OpenAI, Seedream).
- [dsh-plugin-mineru](https://github.com/HuanLinOTO/dsh-plugin-mineru) - Exposes MinerU document-parsing tools to the model — converts PDF/images/DOCX/PPTX/XLSX to structured output.
- [dsh-imagegen](https://github.com/dickpy/dsh-imagegen) - Text-to-image and image-to-image generation directly in the DSH web GUI.
- [picturereader](https://github.com/jing-hy/picturereader) - A DSH plugin that reads images as pixel-to-text for text-only models — image_scan/image_ocr.

### Browser & Computer Use

- [dsh-browser](https://github.com/Lum1104/dsh-browser) - Chrome sidebar extension that lets DSH operate your browser directly — no vision capabilities required.
- [browser-bridge](https://github.com/hanelalo/browser-bridge) - Let your agent drive your real browser window, just like you would.
- [dsh-computer-use](https://github.com/Anionex/dsh-computer-use) - Accessibility-first macOS computer-use plugin with scoped permissions and safe input.
- [open-record-replay](https://github.com/humblebanana/open-record-replay) - macOS record-and-replay workflow recorder for computer-use agents: captures mouse, keyboard, and UI events.
- [dsh-click](https://github.com/PerryLink/dsh-click) - Cross-platform native desktop control for DeepSeek Harness (Windows first): screen_shot, screen_read, click, type, scroll, and key actions with approval gating and process identity verification.

- [mirage](https://github.com/strukto-ai/mirage) - A virtual terminal for AI agents that fuses a VFS sandbox inside a real terminal, DSH-aware.
- [BrowserSkill](https://github.com/Tencent/BrowserSkill) - Let AI agents use your real, logged-in browser without interrupting your work — a CLI plus browser extension for any shell-capable agent.
- [dsh-ios](https://github.com/ZSeven-W/dsh-ios) - A live iOS Simulator — and a USB-connected iPhone — plugin for DeepSeek Harness for UI automation and mobile testing.
- [dsh-tabbit](https://github.com/Tabbit-Browser/dsh-tabbit) - Tabbit Browser plugins for DeepSeek Harness — browser automation that drives a real browser via Playwright.
- [dsh-computer-use (ZRui-C)](https://github.com/ZRui-C/dsh-computer-use) - Text-first browser and background macOS control for DeepSeek Harness — accessibility-first automation.

### Files & Editing

- [dsh-at-file](https://github.com/omdsh-dev/dsh-at-file) - Codex-style `@file` mentions: search workspace files in the composer and attach them to prompts.
- [dsh-toolkit](https://github.com/omdsh-dev/dsh-toolkit) - Zero-dependency toolkit: time, encoding, JSON, calculator, CSV, regex, Markdown, diff, stat, and schema tools.
- [dsh-custom-tool](https://github.com/omdsh-dev/dsh-custom-tool) - Create and manage sandboxed JavaScript tools with a Monaco editor and model-driven tool lifecycle.
- [dsh-plugin (PicGo)](https://github.com/PicGo/dsh-plugin) - Upload images and files to your image host from DeepSeek Harness, powered by PicGo.
- [dsh-lsp-actions](https://github.com/PerryLink/dsh-lsp-actions) - LSP action surface for DSH: diagnostics, formatting, completion, code actions, symbols, signature help, inlay hints and rename, all backed by real language servers.

- [dsh-at-file (FSMargoo)](https://github.com/FSMargoo/dsh-at-file) - Codex-style @file mentions for DeepSeek Harness: search workspace files in the composer and attach their paths to prompts.
- [dsh-wsl-workspace](https://github.com/6Mikao9/dsh-wsl-workspace) - Seamless WSL workspace support for DeepSeek Harness — add a WSL workspace from the GUI without installing dsh inside WSL.
- [dsh-files](https://github.com/taxueseek/dsh-files) - Dual-face file-upload plugin with colorful file previews and document reading in DSH.

### Misc Tools

- [leantoken](https://github.com/morluto/leantoken) - Code intelligence for agents: find the code that matters and keep your context window lean.
- [jacobian](https://github.com/morluto/jacobian) - Pure mathematics for agents: search examples/counterexamples, compute exactly, independently check reasoning.
- [rea](https://github.com/morluto/rea) - Reverse engineer anything with agents, from app behavior down to native binaries.
- [flameox](https://github.com/morluto/flameox) - Runtime evidence for agents: trace, profile, and burn down hotspots in application, native, and GPU code.
- [mcp-for-stata](https://github.com/SepineTam/mcp-for-stata) - MCP server integrating Stata into your agent workflow.
- [dsh-auto-review](https://github.com/PerryLink/dsh-auto-review) - Read-only second-model reviewer for DSH approval requests: structured allow/deny verdicts with reasons, fail-closed by default.
- [dsh-claude-move](https://github.com/PerryLink/dsh-claude-move) - Four-source migration wizard: move Claude Code, Codex, OpenCode and Hermes sessions, memories, skills, instructions and slash commands into DSH (/move wizard with approval gate and idempotent move.json, resumable sessions).
- [dsh-data-quality](https://github.com/PerryLink/dsh-data-quality) - Data quality checking for DeepSeek Harness — profiling, cleaning, and verification pipelines with structured reports.
- [dsh-defend](https://github.com/PerryLink/dsh-defend) - Detects prompt-injection, jailbreak, and secret-leak patterns on the agent/pre-step, tools/pre-execute, and tools/post-execute seams with allow/ask/block tiers, sanitized defend/detection audit events, a defend_report tool, and a destructive-delete command guard.
- [dsh-doublecheck](https://github.com/PerryLink/dsh-doublecheck) - Engineering-discipline guard: requirements grill before the first edit, red/green test-evidence gates, forked adversary review, and a delivery report with a per-dimension verification workflow.
- [dsh-fund-research](https://github.com/PerryLink/dsh-fund-research) - Deterministic research reports for Chinese public mutual funds built from public-source data (Tiantian Fund and Eastmoney), pure-function metrics (performance decomposition, holdings penetration, style attribution, manager profile), and versioned reports with a per-number snapshot traceability appendix.
- [dsh-github](https://github.com/PerryLink/dsh-github) - Official-grade GitHub CI integration: a composite action.yml, a polling PR review bot with idempotent inline comments and a status-check gate, plus PR/issues tools with every write gated by human approval.
- [dsh-industry-research](https://github.com/PerryLink/dsh-industry-research) - Deterministic industry research reports for DeepSeek Harness — company and industry research flows produce structured, verifiable reports from staged evidence.
- [dsh-local-ai](https://github.com/PerryLink/dsh-local-ai) - Ollama provider for DeepSeek Harness with model management, health checks, rule-based local routing, and cloud fallback.
- [dsh-mask](https://github.com/PerryLink/dsh-mask) - PII masking for DeepSeek Harness — anonymizes names, phones, emails, ids, and keys before requests and restores them at the display layer, keeping plaintext out of session logs.
- [dsh-mcp-panel](https://github.com/PerryLink/dsh-mcp-panel) - MCP management console for the official DSH MCP client: server CRUD, health diagnostics, and trial calls from a settings tab.
- [dsh-permission-rules](https://github.com/PerryLink/dsh-permission-rules) - Declarative Claude Code-style permission rules for DSH: ordered allow/deny/ask matching on tools, paths, and network targets.
- [dsh-research-report](https://github.com/PerryLink/dsh-research-report) - Verifiable research-report engine for DeepSeek Harness with a content-addressed evidence ledger, versioned sealed reports where every claim carries a verification verdict and the manifest hash seals the directory, and retrieval orchestration that reuses the ctx.web and ctx.jobs seams.
- [dsh-session-sync](https://github.com/PerryLink/dsh-session-sync) - Cross-device session sync for DeepSeek Harness: a dedicated git mirror of the session store with append-only keep-both conflict resolution that never loses a turn.
- [dsh-skill-pack-security](https://github.com/PerryLink/dsh-skill-pack-security) - Security-audit methodology skill pack plus the plugin_vet supply-chain gate: eight agent skills (secret scan, dependency audit, supply-chain review, prompt-injection review, audit orchestration, threat modeling, vuln intel, incident response) in Chinese and English editions, with an npm provider bundle that mounts the skills and registers the automated plugin_vet pre-install scanner.
- [dsh-translate](https://github.com/PerryLink/dsh-translate) - Tool-output repair layer for DeepSeek Harness — JSON schema enforcement, parameter mapping, and JSON repair for tool calls.

- [dsh-routing-suite](https://github.com/yjh051108/dsh-routing-suite) - Runtime injector plus a task-aware reasoning-mode router preset (measured P1–P23) for DeepSeek Harness.
- [api-relay-audit](https://github.com/toby-bridges/api-relay-audit) - Local security audit for AI API relays and LLM proxies: detects prompt injection, model substitution, tool-call rewriting, SSE anomalies, and error leakage.
- [dsh-pentest](https://github.com/howmp/dsh-pentest) - A penetration-testing mode for DeepSeek Harness (dsh), by @CloverSecLabs.
- [dsh-plugin-subscriptions](https://github.com/V1ki/dsh-plugin-subscriptions) - Use ChatGPT (Codex), Claude, and Grok (X Premium) subscriptions as DeepSeek Harness LLM providers via OAuth.
- [pi2dsh](https://github.com/weijiafu14/pi2dsh) - Bridge Pi and DeepSeek Harness ecosystems: one Pi Host ABI runs unmodified Pi plugins inside DSH.
- [dsh-commandcode-provider](https://github.com/Mars-Sea/dsh-commandcode-provider) - An unofficial DeepSeek Harness LLM provider plugin for Command Code with live model catalog.
- [dsh-reverse-skill](https://github.com/dhicoc/dsh-reverse-skill) - A complete reverse-skill (87 SKILL.md) as a DeepSeek Harness Cordis plugin for CTF and penetration testing.
- [dsh-network-settings](https://github.com/kanneiren/dsh-network-settings) - DeepSeek Harness network diagnostics, proxy detection, and network troubleshooting across macOS/Windows/WSL.
- [dsh-codex-connect](https://github.com/franksong2702/dsh-codex-connect) - Use OpenAI Codex models and image generation via ChatGPT OAuth for DeepSeek Harness.
- [rapid-mlx-dsh-provider](https://github.com/raullenchai/rapid-mlx-dsh-provider) - A native Rapid-MLX provider for DeepSeek Harness — DSH reads model facts from Rapid-MLX for local Apple Silicon inference.
- [opencues](https://github.com/opencues/opencues) - Turns any text field into a two-way LLM channel: read what you write and fill in the context, across Claude Code, Gemini, OpenCode, and DSH.
- [dsh-codex-subscription](https://github.com/WSL043/dsh-codex-subscription) - Bring ChatGPT/Codex subscription into DeepSeek Harness: OAuth, models, quota monitoring, and image generation.
- [dsh-agy-link](https://github.com/amlyczz/dsh-agy-link) - Google Antigravity (agy CLI) models for DeepSeek Harness — streaming chat and thinking.
- [dsh-science](https://github.com/biociao/dsh-science) - A DeepSeek Harness plugin for scientific computing and research workflows.
- [dsh-win32](https://github.com/sjh9714/dsh-win32) - Fix and diagnose DeepSeek Harness on native Windows — official PowerShell and workspace-write support without WSL.
- [dsh-plugin-writing-guard](https://github.com/xmutfyh/dsh-plugin-writing-guard) - A scientific-writing and document-integrity guard for AI-assisted research — style and journal-fit checks.
- [deepseek-harness-acp](https://github.com/openma-ai/deepseek-harness-acp) - An ACP (Agent Client Protocol) server implementation for DeepSeek Harness — dsh-acp.

## Memory & Context

- [mnemon](https://github.com/mnemon-dev/mnemon) - LLM-supervised persistent memory for AI agents: graph-based recall, cross-session knowledge, single binary.
- [dsh-memory-evolve](https://github.com/csyangwen/dsh-memory-evolve) - Cross-session long-term memory plus background self-evolution: five-track memory, git-branch awareness, and skill evolution — pure plugin, no core changes.
- [billion-context-dsh](https://github.com/Tyan66666/billion-context-dsh) - Model-driven context compression (Active Context Pruning) — the model decides when and what to compress.
- [dsh-context-doctor](https://github.com/Zhenyu98/dsh-context-doctor) - Audit exactly what every request carries: token cost of the AGENTS.md chain, skill catalog, and tool schemas, with duplicate/conflict detection.
- [dsh-library](https://github.com/PerryLink/dsh-library) - Turns local markdown and text documents into a queryable knowledge base with hybrid semantic and keyword search, citation verification, and source injection.
- [dsh-memento](https://github.com/PerryLink/dsh-memento) - Bounded, layered, approval-gated cross-session memory for DSH, with a SQLite provider and frozen snapshot injection.

- [OpenViking](https://github.com/volcengine/OpenViking) - Self-evolving context database for AI agents: unify agent memory, knowledge RAG, and skills, with DeepSeek Harness support.
- [memsearch](https://github.com/zilliztech/memsearch) - A persistent, unified memory layer for all your AI agents (Claude Code, Codex, DSH), backed by Markdown and Milvus.
- [dsh-context](https://github.com/bowenliang123/dsh-context) - Context insight and management plugin for DeepSeek Harness — a context dashboard/browser and commands for composition, evolution, compression, and pruning.
- [MisakaNet](https://github.com/Ikalus1988/MisakaNet) - A zero-dependency, git-backed micro-lesson library for AI agents to asynchronously share and search verified knowledge.
- [dsh-mnemon (omdsh-dev)](https://github.com/omdsh-dev/dsh-mnemon) - A composable three-tier memory control plane for DeepSeek Harness: persistent runtime context, searchable project memory, and shared agent memory.
- [dsh-noema](https://github.com/ZSeven-W/dsh-noema) - Noema long-term memory for DSH: durable, inspectable agent memory with recall.
- [dsh-memory (FuRongJun)](https://github.com/FuRongJun-1999/dsh-memory) - A white-box AGI memory exploration: metacognition, continuous learning, and a spatiotemporal knowledge graph for DSH.
- [dsh-meow-memory](https://github.com/Phant0Meow/dsh-meow-memory) - Cross-session memory for DeepSeek Harness — a seven-layer SQLite store for project and soul memory.
- [dsh-mneme](https://github.com/modusensus/dsh-mneme) - The memory that dreams — a self-evolving memory for DeepSeek Harness with heat-memory consolidation and semantic search.
- [dsh-deepread](https://github.com/xiehuan123/dsh-deepread) - Evidence-first reading for AI agents — turns articles, books, and PDFs into traceable knowledge maps.
- [dsh-memoir](https://github.com/Qinling-Melon-Farmers/dsh-memoir) - Local-first cross-session project memory for DeepSeek Harness with cache-aware BM25 hot-memory retrieval.

## Orchestration & Agents

- [dsh-agent-teams](https://github.com/NanmiCoder/dsh-agent-teams) - AgentTeams plugin for DeepSeek Harness.
- [dsh_workflow](https://github.com/icetomoyo/dsh_workflow) - Brings Claude Code's UltraCode mode to DSH: one-off multi-agent scheduling upgraded into a generatable, saveable, governable, observable, resumable workflow layer.
- [allinluna](https://github.com/zenx0x/allinluna) - Resource-aware multi-agent orchestration for Codex and DeepSeek Harness.
- [dsh-automation](https://github.com/titanwings/dsh-automation) - Run coding tasks on a schedule in fresh agent sessions, with user- or agent-managed cron tasks.
- [mstar-harness](https://github.com/btspoony/mstar-harness) - Skill-driven harness/loop-engineering workflow agent plugin.
- [dsh-interconnect](https://github.com/Chinesezjc/dsh-interconnect) - Cross-instance message and event handoff between DSH instances.
- [Vibe-Skills](https://github.com/foryourhealth111-pixel/Vibe-Skills) - General-purpose skill that automatically routes local skills and orchestrates harness workflows.
- [helloagents](https://github.com/hellowind777/helloagents) - An autonomous agent companion that keeps working until the implementation is done and verified.
- [oh-my-dsh](https://github.com/LaplaceYoung/oh-my-dsh) - A 700+ plugin ecosystem for DSH, registered purely through extension seams without touching the agent loop.
- [deepseek-harness-action](https://github.com/Lixiaoyiao/deepseek-harness-action) - GitHub Action that runs DeepSeek Harness for PR review, CI diagnosis, trusted fixes, and issue-to-PR implementation.
- [dsh-background-agents](https://github.com/PerryLink/dsh-background-agents) - Durable background child agents on the official subagent seam: start from any session, watch progress in the Web UI sidebar, message and interrupt any time, with per-child tool scoping, persona and delegation-depth caps.
- [dsh-checkpoint-rewind](https://github.com/PerryLink/dsh-checkpoint-rewind) - Claude Code /rewind for DeepSeek Harness: git-first workspace snapshots before every mutating tool execution, turn-boundary session forks, and a one-shot /rewind command that restores files and forks the session back to a checkpoint.

- [ouroboros](https://github.com/Q00/ouroboros) - Agent OS that makes the agent smarter on its own: interview-gated staged evaluation and a budgeted evolution loop across 13 runtimes including Claude Code and Codex.
- [Aegis](https://github.com/GanyuanRan/Aegis) - Makes AI coding agents architecture-aware: baseline-first, evidence-verified, drift-checked, and safe across long tasks.
- [DSH-taskboard](https://github.com/shengsheng90/DSH-taskboard) - A native local taskboard plugin for DeepSeek Harness with SQLite-backed projects and agent task tracking.
- [dsh-plugin-bridge](https://github.com/Totoro-qaq/dsh-plugin-bridge) - Previewable cross-preset session migration for DeepSeek Harness
- [dsh-agent-team-gui](https://github.com/toolclub/dsh-agent-team-gui) - Persistent multi-model workflow teams for DeepSeek Harness — dynamic lead planning, DAG orchestration, and token usage.
- [dsh-crew](https://github.com/ZSeven-W/dsh-crew) - Dispatch work to DSH agents from Claude Code / Codex — a subagent orchestration bridge.
- [odai](https://github.com/orziz/odai) - A general task-governance framework for AI agents: align goals with facts, and plan and schedule capabilities.
- [sofagent](https://github.com/KongFangXun/sofagent) - An audit-first governance harness for AI coding agents — 24 rules, HMAC chains, and prompt-injection guards.
- [dsh-taskboard (cloader)](https://github.com/cloader/dsh-taskboard) - A kanban task-board plugin for DeepSeek Harness.
- [Vibe-Mathematics](https://github.com/ChongCyrus/Vibe-Mathematics) - A multi-agent mathematics problem-solving and formal-verification framework.

## UI & Interfaces

### Terminal UIs

- [dsh-TUI](https://github.com/ccch1mneyyy/dsh-TUI) - Claude Code-style fullscreen terminal UI: pixel-whale header, live status line, streaming thinking, double-Esc rollback, context progress bar + TPS gauge. `npm` one-line install.
- [dsh-tianshu-tui](https://github.com/huiliyi37/dsh-tianshu-tui) - Interactive terminal UI plugin with a self-developed harness workflow rendering core.

- [Martty](https://github.com/openma-ai/Martty) - A self-improvement TUI plugin for DeepSeek Harness (dsh-tui), built in Rust for terminal UI polish.

### Web UI Enhancements

- [dsh-web-ui](https://github.com/zhu1090093659/dsh-web-ui) - Plugin and skin collection for the DSH Web UI: task board, git graph, right-side panel, and remote mobile UI.
- [DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) - A complete sidebar workbench: file rendering/editing, terminal, Git, subagents — with third-party tab registration.
- [dsh-side-panel](https://github.com/ccq1/dsh-side-panel) - Side panel integrating a file browser, terminal, and Git review.
- [dsh-genui](https://github.com/omdsh-dev/dsh-genui) - GenUI for DSH: interactive UI components rendered inline in assistant replies.
- [dsh-visualize](https://github.com/Nagi-ovo/dsh-visualize) - Generative UI plugin: the model draws interactive HTML cards directly into the conversation, with streaming preview.
- [dsh-notification](https://github.com/omdsh-dev/dsh-notification) - Desktop notifications for turn completions, with per-outcome controls and keyword rules.
- [dsh-open-in-vscode](https://github.com/omdsh-dev/dsh-open-in-vscode) - Open DSH workspace directories in VS Code directly from the web GUI.
- [dsh-annotation](https://github.com/omdsh-dev/dsh-annotation) - Select text in the web UI to annotate it; annotations ship with your next message.
- [dsh-message-edit](https://github.com/Moeblack/dsh-message-edit) - Branch-based message editing, reroll, retry, and a version timeline.
- [dsh-turn-rewind](https://github.com/Anionex/dsh-turn-rewind) - Rewind conversation and workspace state, powered by a persistent change ledger.
- [dsh-share](https://github.com/hellodigua/dsh-share) - One-click conversation sharing.
- [dsh-chat-import](https://github.com/Nwflower/dsh-chat-import) - Import history from Claude Code, Codex, and other agent tools, and continue the conversation in DSH.
- [dsh-openpencil](https://github.com/ZSeven-W/dsh-openpencil) - OpenPencil design preview and editing inside DSH.
- [dsh4vscode](https://github.com/DoggyHU/dsh4vscode) - DSH chat windows inside VS Code with OpenCode-style independent sessions and model auto-routing.
- [dsh-composer-history](https://github.com/PerryLink/dsh-composer-history) - Terminal-style input history for the web composer: edge-first arrow-key recall with exact draft/caret restore, browser-local persisted history, Ctrl+R reverse search, and sliding-context awareness; 0.5.0 adds a smart input layer — cross-session snippets (/save, /load), prompt templates with variables, reuse insights, and compaction-summary highlighting.
- [dsh-message-navigator](https://github.com/miaomiao636/dsh-message-navigator) - Codex-style message navigator for the DSH Web UI: a tick per user message along the conversation edge, hover/click to preview and smooth-jump, with full history auto-loading.
- [dsh-output-styles](https://github.com/PerryLink/dsh-output-styles) - Runtime-switchable model output styles with Claude Code outputStyles parity, plus the output.render.* presentation protocol: a /style command, per-session persistence, systemPrompt injection, six built-in styles, a web picker, and a renderer registry with per-session/per-tool rules and /export.
- [dsh-pr-checks](https://github.com/pauloapoloni/dsh-pr-checks) - GitHub Actions check status and progress for your open PRs, grouped by workspace/project, in the sidebar footer.
- [dsh-session-pin](https://github.com/PerryLink/dsh-session-pin) - Pin sessions and workspaces to the top of the Web sidebar with per-pin row colors, a header toggle and a pinned panel; 0.4.0 adds a navigation organizer — pin groups (boards), tags and saved filter views, session health summaries, and /goto.

- [working-activity](https://github.com/ccch1mneyyy/working-activity) - A lively working-line statusbar extension for the pi CLI and DSH.
- [dsh-synapse](https://github.com/liangmianya/dsh-synapse) - A visual, non-linear conversation workspace plugin for DeepSeek Harness — a canvas-style agent workflow.
- [DSH-EasyRewrite](https://github.com/Renzic-Stone/DSH-EasyRewrite) - A seamless message recall/rewrite plugin for the DSH web UI with undo, rollback, and i18n.
- [dsh-smooth-stream](https://github.com/Laplace-bit/dsh-smooth-stream) - A DeepSeek Harness web UI plugin for fluid streaming rendering and silky scrolling.
- [dsh-navbar](https://github.com/vlln/dsh-navbar) - A DSH dialogue-node navigation bar — quick-jump along a node chain of user messages.
- [dsh-session-manager](https://github.com/dream12347/dsh-session-manager) - DSH session management: delete (trash-restore/purge), statistics, and continuation.
- [dsh-auto-continue](https://github.com/HsiangNianian/dsh-auto-continue) - DSH web UI plugin that auto-sends "continue" after non-human interruptions, with smart sleep modes.
- [dsh-auto-collapse](https://github.com/a179-sanae/dsh-auto-collapse) - Auto-collapses tool outputs in the DSH web UI to keep long agent runs readable.
- [dsh-meow-smooth](https://github.com/Phant0Meow/dsh-meow-smooth) - Mobile notifications for dsh with a polished PWA/UX — a notification layer usable from your phone.
- [dsh-rewind](https://github.com/SiriLee/dsh-rewind) - Seamless in-window conversation rewind for DSH without creating new branches — snapshot, undo, recover.
- [dsh-filesnap](https://github.com/extracurricular-ai/dsh-filesnap) - Roll the conversation and the files it changed back to a previous turn — snapshot/undo for DSH.
- [dsh-recall-plugin](https://github.com/limbo947/dsh-recall-plugin) - A DSH message-withdraw plugin — return to the state when a message was sent, with rollback.
- [dsh-skill-picker](https://github.com/a735624258/dsh-skill-picker) - A WorkBuddy-style skill picker for DeepSeek Harness — pick a skill in the composer and insert the /skill gesture.
- [dsh-milestone](https://github.com/SnowCrescenter-tech/dsh-milestone) - A git-style milestone timeline for DeepSeek Harness — hover for metadata, click to navigate.
- [dsh-vscode](https://github.com/Lixxx1/dsh-vscode) - Use DeepSeek Harness inside VS Code via a VS Code extension.
- [dsh-focus-chat](https://github.com/dingyi222666/dsh-focus-chat) - A new "focused session" streamlined conversation view for dsh.

### Desktop Clients & Distros

- [deeptide](https://github.com/paean-ai/deeptide) - Built by DeepSeek, for DeepSeek — a Swift-native macOS coding agent.
- [oh-dsh](https://github.com/hust-open-atom-club/oh-dsh) - One-stop community distribution: unified TUI, desktop, and Web UI experiences with layered installation.
- [Deepseek-Harness-Desktop](https://github.com/ChisaAlter/Deepseek-Harness-Desktop) - Electron desktop shell for the DSH web UI with themes and background customization.
- [DeepSeekHarnessDesktop](https://github.com/wess09/DeepSeekHarnessDesktop) - Desktop packaging of DeepSeek Harness.
- [dsh-desktop](https://github.com/iuikj/dsh-desktop) - A polished DeepSeek Harness desktop client.
- [DSH-Desktop](https://github.com/JustGenius-s/DSH-Desktop) - Another desktop build of DSH.
- [dsh-launcher](https://github.com/Ruler4396/dsh-launcher) - Lightweight Windows launcher: silent autostart at logon plus a minimal WebView2 window.

- [dsh-desktop (anywhere-labs)](https://github.com/anywhere-labs/dsh-desktop) - A modern desktop client for the DSH plugin ecosystem — the desktop itself ships as a plugin, in the "everything is a plugin" spirit.
- [desktop-cc-gui](https://github.com/zhukunpenglinyutong/desktop-cc-gui) - Multi-engine AI coding desktop client (Tauri) for Claude Code, Codex, Gemini, OpenCode, and DeepSeek Harness.
- [DSHDesktop](https://github.com/dataelement/dsh-desktop) - A DeepSeek Harness desktop build with bundled plugins for a one-click local experience.
- [dsh-desktop (bruc3van)](https://github.com/bruc3van/dsh-desktop) - An open-source DeepSeek Harness desktop client focused on security and developer respect.
- [dsh-desktop-hub](https://github.com/FlashingChen/dsh-desktop-hub) - A desktop management console (Electron + TypeScript) for DeepSeek Harness.

### Skins & Fun

- [dsh-deep-whale](https://github.com/Small-tailqwq/dsh-deep-whale) - Whale-girl skin series for DSH Web (deep-sea maid atelier).
- [whale-girl](https://github.com/vlln/whale-girl) - Desktop-pet whale plugin (QQ-pet style): floating, draggable, feedable companion.
- [dsh-ui-whale](https://github.com/lhh010/dsh-ui-whale) - Hand-drawn pixel whale that lives in the session title bar, animates while thinking, and spouts water on completion.
- [ui-status-label](https://github.com/alingalingling/ui-status-label) - Customize the whale's "deep diving" thinking status label to anything you like.
- [dsh-ads](https://github.com/Nagi-ovo/dsh-ads) - Parody plugin: 2005-era Chinese-site-style sidebar ads, in-feed ads, and corner pop-ups (all fictional).

- [DeepSeek-Balance-Whale-Widget](https://github.com/MeteorNOX/DeepSeek-Balance-Whale-Widget) - A floating whale-girl widget that watches your DeepSeek account balance from the corner of the DSH UI, with drag-and-drop snapping.
- [dsh-pet](https://github.com/PC2005-cloud/dsh-pet) - A transparent animated desktop pet for DSH — one-command install, multi-instance, size and position configurable, with a DIY material chain.
- [DSH-Transparent-UI-Plugin](https://github.com/WYH66666666/DSH-Transparent-UI-Plugin) - A high-degree-of-freedom glass-style theme layered over the DeepSeek Harness web UI.
- [dsh-wallpaper-engine](https://github.com/elysia395/dsh-wallpaper-engine) - Turn your local Wallpaper Engine video backgrounds into the DSH web UI background.
- [open-sea-skin](https://github.com/d-dev0101/open-sea-skin) - A WebGPU ocean skin for DeepSeek Harness — a Harness-only Chrome/Edge theme.
- [dsh-dream-skin](https://github.com/RevolutionLA/dsh-dream-skin) - DeepSeek Harness skin/wallpaper/theme pack plugin — eight mirage-style themes.
- [dsh-status-rotator](https://github.com/01Virex/dsh-status-rotator) - Rotate the "Deep diving…" status label with typewriter-animated rainbow phrases, live status pills, tab titles, and danmaku behind the UI.
- [dsh-whale-musume](https://github.com/Sutera-Diffusus/dsh-whale-musume) - An energetic whale-girl desktop pet for DeepSeek Harness, local-first with no telemetry.
- [dsh-emoji](https://github.com/hellodigua/dsh-emoji) - Add custom emoji to AI replies, sourced from Bilibili, Xiaohongshu, Tieba, and Zhihu.
- [dsh-qq2006](https://github.com/LaplaceYoung/dsh-qq2006) - A QQ2006 retro skin plugin for DeepSeek Harness that mirrors the classic chat UI.
- [dsh-minigames](https://github.com/lhh010/dsh-minigames) - An 18-game offline mini-game panel in the DSH web UI right sidebar.
- [dsh-stickers](https://github.com/william-jin-cmu/dsh-stickers) - A DSH web UI sticker plugin for bidirectional user and agent reactions.
- [dsh-any-background](https://github.com/Tkingxiao/dsh-any-background) - A custom theme plugin for DeepSeek Harness supporting any image/video wallpaper background.

## Observability & Cost

- [tokenbank](https://github.com/wink-run/tokenbank) - Local LLM gateway between your agents and every provider: know where tokens go, spend less.
- [forkprobe](https://github.com/Jayden-X-L/forkprobe) - Compare multiple skills on the same task and pick the winner.
- [dsh-budget](https://github.com/PerryLink/dsh-budget) - Cost governance for DeepSeek Harness: budgets, carbon, and latency in one panel, with per-model, per-session, and per-day token metering, threshold alerts, and over-limit policies.
- [dsh-fast](https://github.com/PerryLink/dsh-fast) - Read-only performance diagnostics for DeepSeek Harness: reports session load and restore timing, context-injection volume, and LLM cache hit rate, off the model hot path.
- [dsh-observe](https://github.com/PerryLink/dsh-observe) - Exports the session event stream to OpenTelemetry OTLP and Langfuse as sanitized, buffered traces and metrics, off by default.

- [TokenTracker](https://github.com/xiufengsun/TokenTracker) - Local-first AI token and cost tracker for 31 coding tools including Claude Code, Codex, Cursor, Gemini, and DeepSeek Harness.
- [dsh-cost-meter](https://github.com/Han-1413141/dsh-cost-meter) - DeepSeek Harness session cost meter: session/daily cost, budgets, history, and threshold alerts.
- [TokenLedger](https://github.com/zh667/TokenLedger) - Relay-site-attributed token usage for DeepSeek Harness — zero config and no credentials.
- [dsh-usage-stats](https://github.com/Ychris12138/dsh-usage-stats) - Provider balances, subscription quotas, and token-usage analytics for DeepSeek Harness.
- [deepseek-harness-control-center](https://github.com/feibi-mochi/deepseek-harness-control-center) - A DeepSeek Harness control center for balance, usage, peak/off-peak pricing, encrypted keys, and session management.
- [dsh-maze](https://github.com/lamost423/dsh-maze) - An execution maze for DeepSeek Harness — visualize how the agent really works through trace playback.
- [dsh-save-money](https://github.com/zhu168/dsh-save-money) - A save-money plugin for DSH — define your own pause/resume triggers to control spend.
- [dsh-whale-report](https://github.com/SenmuuuuW/dsh-whale-report) - DeepTrace — a DSH plugin that turns session event logs into an agent report in numbers.
- [dsh-plugin (loongsuite)](https://github.com/loongsuite/dsh-plugin) - OpenTelemetry tracing for DeepSeek Harness: turns each agent turn into a GFM-tracked trace.
- [dsh-peak-pricing-warning](https://github.com/Imnotndesh/dsh-peak-pricing-warning) - Inline readout beside the model selector showing DeepSeek peak/off-peak pricing status, a countdown to the next rate change, and the estimated session cost at published list rates.

## Integrations & Apps

- [open-design](https://github.com/nexu-io/open-design) - Open-source, local-first design app that turns your coding agent into a design engine: prototypes, landing pages, slides, images, and video.
- [iPolloWork](https://github.com/Devin-AXIS/iPolloWork) - AI workspace with a self-evolving agent runtime that integrates DeepSeek Harness for subagent delegation.
- [OpenBiliClaw](https://github.com/whiteguo233/OpenBiliClaw) - Local-first, self-evolving cross-platform AI content discovery agent ([DSH plugin](https://github.com/whiteguo233/dsh-openbiliclaw) with a dedicated fourth-column UI and 22 agent tools).
- [dsh-work](https://github.com/vibeinging/dsh-work) - Local-first AI workbench combining agent sessions, project files, data analysis, web research, and MCP.
- [MuseAI](https://github.com/yejiming/MuseAI) - Create AI characters and enter story worlds — chat, adventure, and roleplay (ships as a DSH plugin).
- [notes](https://github.com/zhaoolee/notes) - Open-source Smartisan-style notes: self-hostable, skill- and DSH-plugin-enabled, with one-click image export.
- [coding-tools-mcp](https://github.com/xyTom/coding-tools-mcp) - Give any AI agent the ability to code (MCP).
- [sandbase-harness](https://github.com/sandbaseai/sandbase-harness) - Open-source CMA-compatible agent runtime with MCP tools, sandboxed sessions, audit, and replay.

- [dsh-im](https://github.com/xmanrui/dsh-im) - Connect IM bots to DeepSeek Harness via QR code or credentials — supports Feishu, WeChat, DingTalk, WeCom, QQ, Slack, Telegram, Discord, WhatsApp, and more.
- [dsh-pocket](https://github.com/shaobeichen/dsh-pocket) - Put DeepSeek Harness in your pocket: run dsh web on your computer and access it synchronously by scanning a QR code from your phone (LAN + public network, mirrored screen).
- [deepseek-design](https://github.com/Devin-AXIS/deepseek-design) - An editable design system for DeepSeek Harness: AI generation, visual editing, a template market, and PPT workflows.
- [Invoice-Downloader](https://github.com/EthanYoQ/Invoice-Downloader) - An e-invoice collection and reimbursement tool: batch-collect PDF/OFD/XML invoices from email, then OCR, classify, and prepare expense reports.
- [dsh-univer-office](https://github.com/dream-num/dsh-univer-office) - Give DeepSeek Harness a real office environment — widgets for spreadsheets, slides, and documents via Univer Office.
- [dsh-data-agent](https://github.com/omdsh-dev/dsh-data-agent) - Connect DSH to your database for conversational data analysis and actionable business insights.
- [dsh-mobile](https://github.com/saya-ch/dsh-mobile) - A DeepSeek Harness Android app and secure remote-access plugin over LAN or via tailscale/cpolar tunnels.
- [dsh-qqbot](https://github.com/tencent-connect/dsh-qqbot) - The official Tencent plugin to connect a QQ bot to DeepSeek Harness (dsh).
- [dsh-notifier](https://github.com/THEWOLFWALKER/dsh-notifier) - A unified notification and remote-control plugin for DeepSeek Harness: one app across Telegram, Feishu, DingTalk, WeChat, and QQ.
- [dsh-remote (xgone)](https://github.com/xgone/dsh-remote) - Remote access for DeepSeek Harness with account/password auth plus MFA (TOTP) login gating.
- [dsh-remote (flymysql)](https://github.com/flymysql/dsh-remote) - A remote-work assistant for DeepSeek Harness: connect SSH (key or password), SFTP, and tunnels.
- [dsh-lark](https://github.com/omdsh-dev/dsh-lark) - The Lark/Feishu IM bot channel plugin for DeepSeek Harness.
- [dsh-openmaic](https://github.com/THU-MAIC/dsh-openmaic) - OpenMAIC for DeepSeek Harness: classrooms, slides, interactive widgets, and Socratic teaching elements.
- [dsh-passwords](https://github.com/slywalker2006/dsh-passwords) - A server-grade gateway that turns DeepSeek Harness into a multi-tenant platform with per-user auth.
- [dsh-lark-bot](https://github.com/PlutoKeating/dsh-lark-bot) - Connect DeepSeek Harness to a Lark/Feishu bot with QR-code auth, streaming cards, and self-healing.
- [dsh-lark-link](https://github.com/amlyczz/dsh-lark-link) - A high-reliability Feishu/Lark bridge for DeepSeek Harness with QR-code one-click auth.
- [dsh-Remote](https://github.com/Blank-not-black/dsh-Remote) - A pocket DSH console — sessions, approvals, questions, and file transfer from your phone.
- [dsh-full-remote](https://github.com/JUANWANG-BUAA/dsh-full-remote) - An auditable, token-gated DeepSeek Harness remote gateway: mobile QR access and per-device auth.
- [dsh-quant](https://github.com/pengpengyi92/dsh-quant) - An everything-plugin AI-native quantitative OS for DeepSeek Harness — backtesting, risk management, and factor investing.
- [dsh-web-lan-access](https://github.com/AcidGr/dsh-web-lan-access) - A DeepSeek Harness web plugin for accessing dsh web over the local network.
- [dsh-feishu](https://github.com/PGZXB/dsh-feishu) - A panel-driven Feishu control console for DeepSeek Harness — every slash command as interactive cards.
- [dsh-trading](https://github.com/maddogfinance/dsh-trading) - A trading-research workbench for DeepSeek Harness: typed market-data seam and technical analysis.

## Plugin Development & Utilities

- [plugin-registry](https://github.com/vlln/plugin-registry) - Plugin ecosystem infrastructure: a thin browser console for managing official repository plugins, plus a `make-dsh-plugin` skill for guided plugin development.
- [dsh-find-plugins](https://github.com/Nagi-ovo/dsh-find-plugins) - Discover and install plugins from within DSH itself.
- [dsh-plugin-guide](https://github.com/PerryLink/dsh-plugin-guide) - The DSH plugin-development knowledge base as an on-demand agent skill: official constraints, task workflows, API reference and community gotchas, installed with the bundle so the agent can look things up while building a plugin.
- [dsh-score](https://github.com/PerryLink/dsh-score) - Multi-dimensional quality scoring for DeepSeek Harness plugins that scores a repo or npm package across install success, maintenance activity, documentation completeness, security scan, and protocol compliance using real CLI evidence, and produces a JSON or Markdown leaderboard report.
- [dsh-test-drive](https://github.com/PerryLink/dsh-test-drive) - Runs isolated install-and-smoke test drives for DSH plugins in throwaway profiles, returning structured pass/fail records and batch matrices without touching your real profile.

- [dsh-plugin-hub](https://github.com/Noob-stupid/dsh-plugin-hub) - A DSH plugin-management panel: one-click enable/disable plugins plus a GitHub-install flow.
- [dsh-web-plugin-manager](https://github.com/LX2000WASD/dsh-web-plugin-manager) - Manage DeepSeek Harness plugins from the web UI — view, and start/stop them in real time.
- [dsh-config-manager](https://github.com/xiajiajun516/dsh-config-manager) - DeepSeek Harness backup and restore plugin — export, import, migrate, and sync config/skills over WebDAV.
- [dsh-plugin-check](https://github.com/omdsh-dev/dsh-plugin-check) - A DSH plugin health-check tool that scans plugin repos for manifest/protocol and patch-format issues.

## Learning Resources

- [dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) - DeepSeek Harness from 0 to 1: installation, plugin development, performance tuning, and real multi-agent case studies (CN + EN PDF).
- [hello-dsh](https://github.com/pingfanfan/hello-dsh) - Zero-to-plugin tutorial for understanding the "everything is a plugin" architecture, with 22 skill examples.

- [deepseek-harness-handbook](https://github.com/sandbaseai/deepseek-harness-handbook) - An agent-first DeepSeek Harness handbook with 173 source-backed runtime, plugin, MCP, and sandbox references.
- [superpowers-dsh](https://github.com/LayneChai/superpowers-dsh) - Superpowers skills for DeepSeek Harness: TDD, debugging, planning, and collaborative workflows.
- [sandbase-skills](https://github.com/sandbaseai/sandbase-skills) - 88 installable open-source Agent Skills for research, social intelligence, and marketing, usable across DSH.

## Related Lists

- [awesome-dsh-plugins](https://github.com/AdamPlatin123/awesome-dsh-plugins) - Radar-style index that automatically scans for new dsh plugin candidates.
- [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) - Curated list of DSH plugins (CN/EN).
- [awesome-deepseek-harness (0xsline)](https://github.com/0xsline/awesome-deepseek-harness) - Curated plugins, tools, and infrastructure from dsh-external/hub and the public topic.
- [awesome-dsh-plugin (bruc3van)](https://github.com/bruc3van/awesome-dsh-plugin) - Find the right DSH plugin in 30 seconds — organized by problem, not just repo.
- [awesome-DSH-plugin (Alex-Yanggg)](https://github.com/Alex-Yanggg/awesome-DSH-plugin) - Plugins, extensions, tools, and development resources for DSH.
- [awesome-deepseek-harness (libukai)](https://github.com/libukai/awesome-deepseek-harness) - The ultimate guide: quickstart, resources, and selected plugins.
- [awesome-deepseek-harness (Dominic789654)](https://github.com/Dominic789654/awesome-deepseek-harness) - Plugins, skills, MCP servers, orchestrators, and UIs for DSH.

- [dsh-web](https://github.com/zhu1090093659/dsh-web) - Web plugin aggregation ecosystem for DeepSeek Harness, distributed through the Creative Workshop.
- [dsh-market](https://github.com/dsh-market/dsh-market) - The plugin marketplace inside DeepSeek Harness — browse, search, and one-click install plugins.
- [dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) - Open-source DSH plugin-ecosystem radar that auto-discovers 15,900+ candidates and produces a plugin catalog artifact.
- [awesome-dsh-plugin (Anil-matcha)](https://github.com/Anil-matcha/awesome-dsh-plugin) - A curated list of plugins for DeepSeek Harness (dsh) — the plugin ecosystem.
- [Awesome-DeepSeek-Harness-Plugins (Zhiyuan-Fan)](https://github.com/Zhiyuan-Fan/Awesome-DeepSeek-Harness-Plugins) - Curated DeepSeek Harness (DSH) plugins, extensions, tools, skills, clients, runtimes, and verified references — English and Chinese.
- [DSH-Plugins-Marketplace](https://github.com/bradeGithub/DSH-Plugins-Marketplace) - A plugin marketplace that lets you browse and one-click install plugins inside the DeepSeek Harness web GUI.
- [dsh-skin-market](https://github.com/kingOfSoySauce/dsh-skin-market) - A DeepSeek Harness skin market with 200+ skins and a community rating system.
- [dsh-suite](https://github.com/whyihaveyou/dsh-suite) - A living DeepSeek Harness plugin directory — refreshed hourly and compatibility-tested.
- [dsh-plugin-workshop](https://github.com/yyyyukari/dsh-plugin-workshop) - A Steam Workshop-style plugin browser for the DSH web UI.

## Contributing

Contributions are welcome! Please open a pull request adding your plugin under the appropriate category, in this format:

```markdown
- [Plugin Name](https://github.com/user/repo) - One-line description of what it does.
```

Guidelines:

- One plugin per pull request.
- Keep descriptions short and factual.
- The plugin should work with DeepSeek Harness (`dsh`); add the [`dsh-plugin`](https://github.com/topics/dsh-plugin) topic to your repo.

## License

[CC0 1.0 Universal](LICENSE) — public domain dedication.
