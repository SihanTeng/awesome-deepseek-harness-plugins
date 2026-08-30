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

### Vision

- [modlens](https://github.com/liustack/modlens) - The first vision plugin for DeepSeek Harness — paste an image, get analysis; a vision bridge for text-only coding agents.
- [dsh-vision-toolkit](https://github.com/Anionex/dsh-vision-toolkit) - Vision toolkit for text-only models: intent-aware image Q&A, long-screenshot OCR, and UI restoration.
- [dsh-vision](https://github.com/william-jin-cmu/dsh-vision) - `view_image` tool bridging any OpenAI-compatible VLM (works with free tiers).
- [dsh-vision-router](https://github.com/ysr666/dsh-vision-router) - Built-in keyless vision chain plus pixel-level tools (Q&A, grounding) for text-only agents.

### Browser & Computer Use

- [dsh-browser](https://github.com/Lum1104/dsh-browser) - Chrome sidebar extension that lets DSH operate your browser directly — no vision capabilities required.
- [browser-bridge](https://github.com/hanelalo/browser-bridge) - Let your agent drive your real browser window, just like you would.
- [dsh-computer-use](https://github.com/Anionex/dsh-computer-use) - Accessibility-first macOS computer-use plugin with scoped permissions and safe input.
- [open-record-replay](https://github.com/humblebanana/open-record-replay) - macOS record-and-replay workflow recorder for computer-use agents: captures mouse, keyboard, and UI events.

### Files & Editing

- [dsh-at-file](https://github.com/omdsh-dev/dsh-at-file) - Codex-style `@file` mentions: search workspace files in the composer and attach them to prompts.
- [dsh-toolkit](https://github.com/omdsh-dev/dsh-toolkit) - Zero-dependency toolkit: time, encoding, JSON, calculator, CSV, regex, Markdown, diff, stat, and schema tools.
- [dsh-custom-tool](https://github.com/omdsh-dev/dsh-custom-tool) - Create and manage sandboxed JavaScript tools with a Monaco editor and model-driven tool lifecycle.
- [dsh-plugin (PicGo)](https://github.com/PicGo/dsh-plugin) - Upload images and files to your image host from DeepSeek Harness, powered by PicGo.

### Misc Tools

- [leantoken](https://github.com/morluto/leantoken) - Code intelligence for agents: find the code that matters and keep your context window lean.
- [jacobian](https://github.com/morluto/jacobian) - Pure mathematics for agents: search examples/counterexamples, compute exactly, independently check reasoning.
- [rea](https://github.com/morluto/rea) - Reverse engineer anything with agents, from app behavior down to native binaries.
- [flameox](https://github.com/morluto/flameox) - Runtime evidence for agents: trace, profile, and burn down hotspots in application, native, and GPU code.
- [mcp-for-stata](https://github.com/SepineTam/mcp-for-stata) - MCP server integrating Stata into your agent workflow.
- [dsh-translate](https://github.com/PerryLink/dsh-translate) - Tool-output repair layer for DeepSeek Harness — JSON schema enforcement, parameter mapping, and JSON repair for tool calls.

## Memory & Context

- [mnemon](https://github.com/mnemon-dev/mnemon) - LLM-supervised persistent memory for AI agents: graph-based recall, cross-session knowledge, single binary.
- [dsh-memory-evolve](https://github.com/csyangwen/dsh-memory-evolve) - Cross-session long-term memory plus background self-evolution: five-track memory, git-branch awareness, and skill evolution — pure plugin, no core changes.
- [billion-context-dsh](https://github.com/Tyan66666/billion-context-dsh) - Model-driven context compression (Active Context Pruning) — the model decides when and what to compress.
- [dsh-context-doctor](https://github.com/Zhenyu98/dsh-context-doctor) - Audit exactly what every request carries: token cost of the AGENTS.md chain, skill catalog, and tool schemas, with duplicate/conflict detection.

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

## UI & Interfaces

### Terminal UIs

- [dsh-TUI](https://github.com/ccch1mneyyy/dsh-TUI) - Claude Code-style fullscreen terminal UI: pixel-whale header, live status line, streaming thinking, double-Esc rollback, context progress bar + TPS gauge. `npm` one-line install.
- [dsh-tianshu-tui](https://github.com/huiliyi37/dsh-tianshu-tui) - Interactive terminal UI plugin with a self-developed harness workflow rendering core.

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

### Desktop Clients & Distros

- [deeptide](https://github.com/paean-ai/deeptide) - Built by DeepSeek, for DeepSeek — a Swift-native macOS coding agent.
- [oh-dsh](https://github.com/hust-open-atom-club/oh-dsh) - One-stop community distribution: unified TUI, desktop, and Web UI experiences with layered installation.
- [Deepseek-Harness-Desktop](https://github.com/ChisaAlter/Deepseek-Harness-Desktop) - Electron desktop shell for the DSH web UI with themes and background customization.
- [DeepSeekHarnessDesktop](https://github.com/wess09/DeepSeekHarnessDesktop) - Desktop packaging of DeepSeek Harness.
- [dsh-desktop](https://github.com/iuikj/dsh-desktop) - A polished DeepSeek Harness desktop client.
- [DSH-Desktop](https://github.com/JustGenius-s/DSH-Desktop) - Another desktop build of DSH.
- [dsh-launcher](https://github.com/Ruler4396/dsh-launcher) - Lightweight Windows launcher: silent autostart at logon plus a minimal WebView2 window.

### Skins & Fun

- [dsh-deep-whale](https://github.com/Small-tailqwq/dsh-deep-whale) - Whale-girl skin series for DSH Web (deep-sea maid atelier).
- [whale-girl](https://github.com/vlln/whale-girl) - Desktop-pet whale plugin (QQ-pet style): floating, draggable, feedable companion.
- [dsh-ui-whale](https://github.com/lhh010/dsh-ui-whale) - Hand-drawn pixel whale that lives in the session title bar, animates while thinking, and spouts water on completion.
- [ui-status-label](https://github.com/alingalingling/ui-status-label) - Customize the whale's "deep diving" thinking status label to anything you like.
- [dsh-ads](https://github.com/Nagi-ovo/dsh-ads) - Parody plugin: 2005-era Chinese-site-style sidebar ads, in-feed ads, and corner pop-ups (all fictional).

## Observability & Cost

- [tokenbank](https://github.com/wink-run/tokenbank) - Local LLM gateway between your agents and every provider: know where tokens go, spend less.
- [forkprobe](https://github.com/Jayden-X-L/forkprobe) - Compare multiple skills on the same task and pick the winner.

## Integrations & Apps

- [open-design](https://github.com/nexu-io/open-design) - Open-source, local-first design app that turns your coding agent into a design engine: prototypes, landing pages, slides, images, and video.
- [iPolloWork](https://github.com/Devin-AXIS/iPolloWork) - AI workspace with a self-evolving agent runtime that integrates DeepSeek Harness for subagent delegation.
- [OpenBiliClaw](https://github.com/whiteguo233/OpenBiliClaw) - Local-first, self-evolving cross-platform AI content discovery agent ([DSH plugin](https://github.com/whiteguo233/dsh-openbiliclaw) with a dedicated fourth-column UI and 22 agent tools).
- [dsh-work](https://github.com/vibeinging/dsh-work) - Local-first AI workbench combining agent sessions, project files, data analysis, web research, and MCP.
- [MuseAI](https://github.com/yejiming/MuseAI) - Create AI characters and enter story worlds — chat, adventure, and roleplay (ships as a DSH plugin).
- [notes](https://github.com/zhaoolee/notes) - Open-source Smartisan-style notes: self-hostable, skill- and DSH-plugin-enabled, with one-click image export.
- [coding-tools-mcp](https://github.com/xyTom/coding-tools-mcp) - Give any AI agent the ability to code (MCP).
- [sandbase-harness](https://github.com/sandbaseai/sandbase-harness) - Open-source CMA-compatible agent runtime with MCP tools, sandboxed sessions, audit, and replay.

## Plugin Development & Utilities

- [plugin-registry](https://github.com/vlln/plugin-registry) - Plugin ecosystem infrastructure: a thin browser console for managing official repository plugins, plus a `make-dsh-plugin` skill for guided plugin development.
- [dsh-find-plugins](https://github.com/Nagi-ovo/dsh-find-plugins) - Discover and install plugins from within DSH itself.

## Learning Resources

- [dsh-handbook](https://github.com/Electricitysheep/dsh-handbook) - DeepSeek Harness from 0 to 1: installation, plugin development, performance tuning, and real multi-agent case studies (CN + EN PDF).
- [hello-dsh](https://github.com/pingfanfan/hello-dsh) - Zero-to-plugin tutorial for understanding the "everything is a plugin" architecture, with 22 skill examples.

## Related Lists

- [awesome-dsh-plugins](https://github.com/AdamPlatin123/awesome-dsh-plugins) - Radar-style index that automatically scans for new dsh plugin candidates.
- [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) - Curated list of DSH plugins (CN/EN).
- [awesome-deepseek-harness (0xsline)](https://github.com/0xsline/awesome-deepseek-harness) - Curated plugins, tools, and infrastructure from dsh-external/hub and the public topic.
- [awesome-dsh-plugin (bruc3van)](https://github.com/bruc3van/awesome-dsh-plugin) - Find the right DSH plugin in 30 seconds — organized by problem, not just repo.
- [awesome-DSH-plugin (Alex-Yanggg)](https://github.com/Alex-Yanggg/awesome-DSH-plugin) - Plugins, extensions, tools, and development resources for DSH.
- [awesome-deepseek-harness (libukai)](https://github.com/libukai/awesome-deepseek-harness) - The ultimate guide: quickstart, resources, and selected plugins.
- [awesome-deepseek-harness (Dominic789654)](https://github.com/Dominic789654/awesome-deepseek-harness) - Plugins, skills, MCP servers, orchestrators, and UIs for DSH.

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
