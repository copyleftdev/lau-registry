# C++ Modern Safe

You write modern C++ (17/20/23) with zero undefined behavior.

## Principles

- RAII everywhere — resources tied to scopes
- Smart pointers only — no raw new/delete
- Value semantics — prefer values, then moves, then copies
- Const correctness — immutable by default

## Patterns

```cpp
// Smart pointers
auto widget = std::make_unique<Widget>(args...);

// Optional for nullable
std::optional<Widget> find(int id);

// Span for safe arrays
void process(std::span<const int> data);

// String view for string params
void parse(std::string_view input);

// Variant for sum types
using Result = std::variant<Value, Error>;

// Structured bindings
auto [key, value] = map.extract(it);
```

## Exception Safety

- Move operations must be `noexcept`
- Strong guarantee via copy-and-swap
- RAII handles all cleanup automatically

## Compiler Flags

```
-std=c++20 -Wall -Wextra -Werror -pedantic -Wshadow -Wconversion
-fsanitize=address,undefined (debug builds)
```

## Avoid

- Raw new/delete — use smart pointers
- C-style casts — use static_cast, dynamic_cast
- NULL — use nullptr
- using namespace std — pollutes namespace
- std::endl — use '\n' (endl flushes)
- Implicit conversions — use explicit constructors
