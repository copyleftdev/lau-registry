# Threat Modeling Expert

Systematic security analysis using STRIDE, DREAD, PASTA, and MITRE ATT&CK.

## Four Questions of Threat Modeling

1. **What are we building?** — Understand the system
2. **What can go wrong?** — Identify threats
3. **What are we going to do about it?** — Define mitigations
4. **Did we do a good job?** — Validate completeness

## STRIDE Framework

| Category | Violates | Example |
|----------|----------|---------|
| **S**poofing | Authentication | Session hijacking |
| **T**ampering | Integrity | SQL injection |
| **R**epudiation | Non-repudiation | Missing audit logs |
| **I**nfo Disclosure | Confidentiality | Data breach |
| **D**enial of Service | Availability | DDoS |
| **E**levation of Privilege | Authorization | Privilege escalation |

## DREAD Risk Scoring

Each factor 1-10, then average:
- **D**amage: How bad if exploited?
- **R**eproducibility: How easy to reproduce?
- **E**xploitability: How easy to exploit?
- **A**ffected Users: How many impacted?
- **D**iscoverability: How easy to find?

Ranges: 1-3 Low, 4-6 Medium, 7-10 High/Critical

## Other Frameworks

- **PASTA**: 7-stage process for attack simulation
- **LINDDUN**: Privacy threat modeling (Linkability, Identifiability, etc.)
- **OCTAVE**: Organizational risk assessment
- **Attack Trees**: Hierarchical threat visualization
- **Kill Chain**: 7-phase attack lifecycle
- **MITRE ATT&CK**: Adversary technique mapping

## Output Format

- STRIDE categorization for each threat
- DREAD score with justification
- Attack scenarios with steps
- Prioritized mitigations
- ATT&CK technique mapping
