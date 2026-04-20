<div align="center">
  <br>
  <img src="https://alby.sh/icon.png" width="96" alt="Alby" onerror="this.style.display='none'" />
  <h1>Alby</h1>
  <p><strong>The control room for your AI coding agents.</strong></p>

  <p>
    <a href="https://alby.sh"><img src="https://img.shields.io/badge/website-alby.sh-black?style=flat-square" alt="alby.sh" /></a>
    <a href="https://github.com/alby-sh/alby/releases/latest"><img src="https://img.shields.io/github/v/release/alby-sh/alby?label=Download%20for%20macOS&style=flat-square&color=blue" alt="Download" /></a>
    <img src="https://img.shields.io/badge/platform-macOS-lightgrey?style=flat-square" alt="macOS" />
  </p>
</div>

---

## What we build

Alby lets you **spawn, monitor and orchestrate dozens of AI coding agents in parallel** — Claude Code, Gemini, Codex, or any terminal-based CLI — across local folders and remote SSH servers, from a single native macOS app. Every agent runs inside a persistent `tmux` session, so your work survives disconnects, sleeps and restarts.

Beyond the app itself, Alby plugs into your running code via a small family of open-source SDKs: when something crashes in production, the exception lands in your Alby project and an AI agent can auto-open a fix task for it — with full context, stack trace, breadcrumbs and source-mapped frames.

## The desktop app

<table>
  <tr>
    <td width="160" align="center"><a href="https://github.com/alby-sh/alby"><strong>alby-sh/<br>alby</strong></a></td>
    <td>Native macOS app (Electron). Manages dozens of tmux-backed agent sessions across local and remote environments, syncs state across devices, integrates Git / GitHub / scheduled routines / team collaboration.<br><br><a href="https://github.com/alby-sh/alby/releases/latest">Download the latest release →</a></td>
  </tr>
</table>

## Error-tracking SDKs

Drop one of these into your app and runtime errors flow back into Alby for triage, grouping, release tracking, and AI-assisted auto-fix. All MIT-licensed, zero runtime dependencies, tiny footprint.

| Runtime | Install | Repo |
|---|---|---|
| Node.js / TypeScript | `npm install @alby/report` | [alby-sh/alby-sdk-js](https://github.com/alby-sh/alby-sdk-js) |
| Browser (any bundler or `<script>`) | `npm install @alby/browser` | [alby-sh/alby-sdk-browser](https://github.com/alby-sh/alby-sdk-browser) |
| PHP 8.2+ (Laravel auto-discovery) | `composer require alby/report` | [alby-sh/alby-sdk-php](https://github.com/alby-sh/alby-sdk-php) |
| Python 3.8+ (Django / Flask / FastAPI) | `pip install alby-report` | [alby-sh/alby-sdk-python](https://github.com/alby-sh/alby-sdk-python) |

All four SDKs speak the same wire protocol ([Ingest Protocol v1](https://github.com/alby-sh/alby-sdk-js/blob/main/PROTOCOL_V1.md)) — writing one for a new runtime is a weekend project, and we welcome PRs.

## Links

- **Website** — [alby.sh](https://alby.sh)
- **Download** — [latest macOS build](https://github.com/alby-sh/alby/releases/latest)
- **Contact** — [info@alby.sh](mailto:info@alby.sh)
