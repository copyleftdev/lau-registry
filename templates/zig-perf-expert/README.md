# Zig Performance Expert

> Systems programming without the footguns — TigerBeetle-grade engineering.

## Philosophy

This template embodies **Zig's core values**:

- **Simplicity over complexity** — No hidden control flow, no hidden allocations
- **Performance by default** — Zero-cost abstractions that actually cost zero
- **Safety without runtime cost** — Compile-time checks, no GC, explicit memory
- **Debuggability** — When things fail, you can understand why

## Inspired By

- **TigerBeetle** — Financial database built in Zig
- **Bun** — JavaScript runtime with Zig core
- **Zig Standard Library** — Andrew Kelley's design patterns
- **Mach Engine** — Game engine in Zig

## What You Get

A Zig expert who:

- Uses comptime for zero-cost generics and metaprogramming
- Handles errors explicitly with `error` unions and `try`
- Manages memory with allocators, not hidden malloc
- Writes SIMD-friendly, cache-aware code
- Avoids undefined behavior religiously
- Uses `defer` and `errdefer` for resource cleanup
- Profiles before optimizing

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
lau zig-perf-expert
```

## Files Installed

Varies by provider. Typically includes:

- System/agent prompt defining the Zig expert persona
- Memory management patterns
- Performance idioms
- Common pitfalls to avoid
