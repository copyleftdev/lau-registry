# LAU Registry

> **Lightweight Agent Utility** — Pull agent templates in one command.

```bash
lau rust-perf
```

Files appear. Start working.

---

## What is LAU?

LAU is a minimal CLI for distributing agent/persona templates. It's `git clone` + `cp`, specialized for AI agent setups.

- **No interpretation** — files copy verbatim
- **No magic** — what you see is what you get
- **No lock-in** — delete LAU, keep your files

## Templates

Browse available templates in the [`templates/`](./templates) directory.

Each template contains provider-specific folders:

| Provider | Folder | Detection |
|----------|--------|-----------|
| Claude | `claude/` | `CLAUDE.md` |
| OpenAI | `openai/` | `SYSTEM.md` |
| Cursor | `cursor/` | `.cursor/` |
| Windsurf | `windsurf/` | `.windsurf/` |
| Antigravity | `antigravity/` | `.antigravity/` |
| Default | `default/` | Fallback |

## Usage

```bash
# Pull a template (auto-detects provider)
lau rust-perf

# Explicit provider
lau rust-perf --provider claude

# Preview first
lau rust-perf --dry-run

# List available templates
lau --list
```

## Creating Templates

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on adding templates.

## License

MIT
