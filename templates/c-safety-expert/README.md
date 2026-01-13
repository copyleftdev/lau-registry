# C Safety Expert

> Security-minded C development — NASA Power of 10, MISRA-C, CERT-C.

## Philosophy

This template embodies **defensive, safety-critical C programming**:

- **Prove correctness, don't assume it** — Static analysis, bounded operations
- **Fail predictably** — Defined behavior in all error paths
- **Minimize attack surface** — No undefined behavior, no memory corruption
- **Verify everything** — Assertions, invariants, pre/post conditions

## Standards Referenced

- **NASA JPL Power of 10** — 10 rules for safety-critical code
- **MISRA-C:2012** — Automotive/embedded safety standard
- **CERT-C** — SEI secure coding standard
- **CWE Top 25** — Common weakness enumeration

## What You Get

A C expert who:

- Writes bounded, statically analyzable code
- Avoids undefined behavior religiously
- Uses static allocation over dynamic when possible
- Validates all inputs at trust boundaries
- Handles every error path explicitly
- Writes code that passes `-Wall -Wextra -Werror -pedantic`

## Provider Coverage

| Provider | Status |
|----------|--------|
| Claude | ✅ |
| OpenAI | ✅ |
| Cursor | ✅ |
| Windsurf | ✅ |
| Antigravity | ✅ |
| Default | ✅ |

## Usage

```bash
lau c-safety-expert
```

## Files Installed

Varies by provider. Typically includes:

- System/agent prompt defining the safety-critical C persona
- NASA Power of 10 rules reference
- Common vulnerability patterns to avoid
