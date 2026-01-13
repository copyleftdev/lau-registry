# Contributing Templates

## Template Structure

Templates are organized by category in `templates/`:

```
templates/
  <category>/
    your-template/
      README.md           # Required: describe the template
      claude/             # Provider folder
        CLAUDE.md
        skills/
      openai/
        SYSTEM.md
      cursor/
        .cursor/rules/
      windsurf/
        rules/
      antigravity/
        rules/
      default/            # Fallback if no provider matches
        AGENT.md
```

### Categories

| Category | Use For |
|----------|---------|
| `languages/` | Programming language experts (Python, C, Rust, etc.) |
| `testing/` | Testing methodologies, frameworks, DST |
| `devops/` | CI/CD, IaC, containerization, GitOps |
| `security/` | AppSec, threat modeling, secure coding |
| `infrastructure/` | SRE, observability, platform engineering |

## Rules

1. **README.md is required** — Describe what the template does, who it's for, and what files are included.

2. **Provider folders are optional** — Include only the providers you support.

3. **`default/` is the fallback** — If a user's provider isn't available, LAU falls back to `default/`.

4. **No transformation** — Files are copied verbatim. Don't assume LAU will process anything.

5. **Keep it focused** — One template, one purpose. Don't bundle unrelated personas.

## Naming

- Use lowercase with hyphens: `rust-perf`, `code-review`, `security-audit`
- Be descriptive but concise
- Avoid generic names like `default` or `general`

## Testing

Before submitting:

1. Verify all provider folders contain valid files
2. Ensure README accurately describes contents
3. Test with `lau your-template --dry-run` (once LAU exists)

## Submitting

1. Fork this repository
2. Add your template to `templates/`
3. Open a pull request with a clear description
