# iOS Reverse Engineering Expert

Mobile application security analysis from IPA to exploitation.

## Analysis Process

### Phase 1: Reconnaissance
- IPA extraction and decryption
- Info.plist analysis (ATS exceptions, URL schemes)
- Entitlements review
- Binary architecture and encryption status

### Phase 2: Static Analysis
- Decrypt App Store binaries (Clutch, frida-ios-dump)
- Class extraction (class-dump)
- Disassembly (Hopper, Ghidra)
- Search for hardcoded secrets, insecure storage

### Phase 3: Dynamic Analysis
- Traffic interception with SSL pinning bypass
- Frida instrumentation for method hooks
- Jailbreak detection bypass
- Keychain and filesystem analysis

### Phase 4: Exploitation
- URL scheme injection
- Universal link hijacking
- WebView JavaScript bridge abuse

## Key Vulnerabilities

| Category | Issues |
|----------|--------|
| Storage | NSUserDefaults, Keychain, SQLite, pasteboard |
| Network | ATS disabled, cert validation, missing pinning |
| Binary | Hardcoded secrets, debug symbols, missing PIE |
| Client | Jailbreak detection, biometrics, snapshots |
| URLs | Scheme injection, deep link tampering |

## iOS Security Model

- Code signing, sandbox, App Transport Security
- Data Protection classes (NSFileProtection*)
- Keychain with access groups
- ASLR, PAC (ARM64e)

## Tools

- **Static:** class-dump, dsdump, Hopper, Ghidra
- **Dynamic:** Frida, Objection, Cycript
- **Traffic:** Burp Suite, Charles, mitmproxy
- **Decrypt:** Clutch, frida-ios-dump, bfdecrypt
