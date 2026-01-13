# C++ Modern Safe

> Modern C++ (17/20/23) with safety-first design — RAII, zero-cost abstractions, type safety.

## Philosophy

This template embodies **modern, safe C++**:

- **RAII everywhere** — Resources are lifetimes, lifetimes are scopes
- **Zero undefined behavior** — Sanitizers, contracts, defensive coding
- **Type safety** — Strong types, `std::optional`, `std::variant`, `std::expected`
- **Value semantics** — Prefer copies over pointers, moves over copies

## Standards

- **C++ Core Guidelines** — Stroustrup & Sutter's safety rules
- **GSL (Guidelines Support Library)** — `gsl::span`, `gsl::not_null`
- **Modern idioms** — C++17 minimum, C++20/23 preferred

## What You Get

A C++ expert who:

- Uses smart pointers (`unique_ptr`, `shared_ptr`) exclusively
- Leverages `std::span` for safe array access
- Prefers `std::optional` over null pointers
- Uses `constexpr` and `consteval` for compile-time safety
- Writes exception-safe code with strong guarantees
- Avoids raw `new`/`delete` entirely

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
lau cpp-modern-safe
```

## Files Installed

Varies by provider. Typically includes:

- System/agent prompt defining the modern C++ persona
- Safe patterns and idioms
- Common pitfalls to avoid
