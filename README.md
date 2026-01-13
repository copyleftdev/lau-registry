# LAU Registry

> **Lightweight Agent Utility** — Pull agent templates in one command.

```bash
lau languages/pythonic-expert
```

Files appear. Start working.

---

## What is LAU?

LAU is a minimal CLI for distributing agent/persona templates. It's `git clone` + `cp`, specialized for AI agent setups.

- **No interpretation** — files copy verbatim
- **No magic** — what you see is what you get
- **No lock-in** — delete LAU, keep your files

## Templates

Browse available templates in the [`templates/`](./templates) directory, organized by category:

### 📁 Categories

| Category | Description |
|----------|-------------|
| [`languages/`](./templates/languages) | Programming language experts |
| [`testing/`](./templates/testing) | Testing methodologies & frameworks |
| [`devops/`](./templates/devops) | CI/CD, infrastructure as code |
| [`security/`](./templates/security) | AppSec, threat modeling |
| [`infrastructure/`](./templates/infrastructure) | SRE, observability |

### 🗂️ Available Templates

| Template | Category | Description |
|----------|----------|-------------|
| `languages/pythonic-expert` | Languages | Idiomatic Python, PEP-8, type hints |
| `languages/c-safety-expert` | Languages | NASA Power of 10, MISRA-C, CERT-C |
| `languages/cpp-modern-safe` | Languages | C++17/20/23, RAII, smart pointers |
| `languages/zig-perf-expert` | Languages | TigerBeetle-grade systems programming |
| `testing/test-vopr-expert` | Testing | DST, multiverse testing, invariants |

### Provider Support

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
lau languages/pythonic-expert

# Explicit provider
lau languages/c-safety-expert --provider claude

# Preview first
lau testing/test-vopr-expert --dry-run

# List available templates
lau --list
```

## Creating Templates

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on adding templates.

## License

MIT
