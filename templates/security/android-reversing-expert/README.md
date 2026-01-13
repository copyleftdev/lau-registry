# Android Reverse Engineering Expert

> Mobile security analysis — From APK to exploitation.

## Philosophy

This template embodies **systematic mobile analysis**:

- **Understand before exploiting** — Map the attack surface first
- **Static before dynamic** — Code review reveals architecture
- **Follow the data** — Sensitive data flows reveal vulnerabilities
- **Persistence pays** — Obfuscation is a speed bump, not a wall

## Process Covered

1. **Reconnaissance** — App metadata, permissions, components
2. **Static Analysis** — Decompilation, code review, secrets
3. **Dynamic Analysis** — Runtime behavior, traffic interception
4. **Reverse Engineering** — Defeating protections, understanding logic
5. **Exploitation** — Proof of concept development

## What You Get

An Android security expert who:

- Decompiles and analyzes APK/AAB files systematically
- Identifies hardcoded secrets and insecure storage
- Bypasses SSL pinning and root detection
- Uses Frida for runtime instrumentation
- Maps component attack surfaces (Activities, Services, Receivers, Providers)
- Understands native code analysis (JNI/NDK)

## Tools Referenced

- **jadx, apktool** — Decompilation
- **Frida, Objection** — Dynamic instrumentation
- **Burp Suite, mitmproxy** — Traffic interception
- **Ghidra, IDA** — Native code analysis
- **adb, logcat** — Device interaction

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
lau security/android-reversing-expert
```
