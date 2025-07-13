# 🎯 Roop Framework LICENSE.md  
**📅 Effective Date:** July 13, 2025  
**✍️ Author:** KristoStl ([GitHub](https://github.com/KristoStl))  

---

## 📑 Table of Contents  
1. [Definitions](#definitions)  . . . ...............................................................................................
2. [Grant of License](#grant-of-license)  
3. [Installation & Activation](#installation--activation)  
4. [Scope of Use](#scope-of-use)  
5. [Model License (Annex A)](#model-license-annex-a)  
6. [Services License (Annex B)](#services-license-annex-b)  
7. [Permitted Use](#permitted-use)  
8. [Prohibited Use](#prohibited-use)  
9. [Distribution & Sub-Licensing](#distribution--sub-licensing)  
10. [Storage & Integration Guidelines](#storage--integration-guidelines)  
11. [Data Privacy & Security](#data-privacy--security)  
12. [Attribution & Branding](#attribution--branding)  
13. [Audit, Monitoring & Compliance](#audit-monitoring--compliance)  
14. [Support & Maintenance](#support--maintenance)  
15. [Fees & Commercial Licensing](#fees--commercial-licensing)  
16. [Intellectual Property Rights](#intellectual-property-rights)  
17. [Disclaimers & Limitation of Liability](#disclaimers--limitation-of-liability)  
18. [Indemnification](#indemnification)  
19. [Termination & Suspension](#termination--suspension)  
20. [Modifications & Updates](#modifications--updates)  
21. [Governing Law & Dispute Resolution](#governing-law--dispute-resolution)  
22. [No Waiver](#no-waiver)  
23. [Severability](#severability)  
24. [Assignment](#assignment)  
25. [Entire Agreement](#entire-agreement)  
26. [Revision History](#revision-history)  

---

## 1. Definitions  
- **“Roop”**  
  The Roblox framework—including model files (`.rbxm`, `.rbxl`), Remote Modules, Package contents, scripts, GUIs, signals, assets, configuration and documentation—authored by KristoStl.  

- **“Repository”**  
  The official GitHub repository ([github.com/KristoStl/Roop](https://github.com/KristoStl/Roop)) hosting all Roop code, assets, and this LICENSE.md.  

- **“Developer” / “You” / “Your”**  
  Any person or entity accessing, integrating, forking, distributing, or modifying Roop.  

- **“Experience”**  
  A Roblox Place or Universe that incorporates Roop.  

- **“License Key”**  
  A 32-character alphanumeric code issued by KristoStl to activate Roop features in one Experience.  

- **“Unauthorized Data”**  
  Any personal or usage data beyond the minimal identifier and telemetry Roop expressly collects.  

---

## 2. Grant of License  
1. Roop is licensed, not sold.  
2. You receive a limited, non-exclusive, non-transferable, revocable license to integrate and use Roop in **one** Roblox Experience per License Key.  
3. This license covers all v1.x minor updates and patches. Major upgrades (v2.0+) require a new license.  
4. You may clone or fork the Repository **privately** for internal development, testing, or staging.  

---

## 3. Installation & Activation  
1. Obtain Roop exclusively from this Repository.  
2. Follow the step-by-step guide in `/docs/INSTALL.md`.  
3. Insert your PlaceId and License Key into `Settings.lua`.  
4. Activation occurs at game startup; failure to authenticate disables Roop.  
5. Tampering with `Activation.lua` or repeated failed attempts (5+) locks out your License Key for 24 hours.  
6. License Key exposure or compromise must be reported to kristostl@example.com within 24 hours.  

---

## 4. Scope of Use  
- **Permitted**  
  - Personal, educational, non-commercial, or internal team deployments.  
  - Closed beta or invite-only testing environments.  

- **Prohibited**  
  - Bundling Roop with any external tool, platform, engine, or headless server.  
  - Integrations that circumvent Roblox’s Terms of Service or Community Standards.  

---

## 5. Model License (Annex A)  

**Effective Date:** July 12, 2025

This Annex governs the use of the Roop Services **model file** (`.rbxm` / `.rbxl`), including all embedded scripts, GUI components, ModuleScripts, LocalScripts, folders, assets, and configurations.

### A.1 Model Scope & Contents  
- Folder Architecture: `RClient`, `RServer`, `StarterKit`, `Signals`  
- Embedded `ModuleScripts` & `LocalScripts`  
- GUI Layouts & Containers  
- `RemoteEvents`, Signals & Handlers  
- Plugin-style Loaders & Setup Scripts  

### A.2 Permitted Use  
You may:  
- Use the model inside personal or team Roblox Experiences.  
- Modify scripts, GUIs, and assets for internal development.  
- Extend or wrap modules for custom onboarding flows, analytics, or developer tools.  

### A.3 Restricted Use  
You may **NOT**:  
- Re-upload or rebrand the model under your own name or group.  
- Sell, rent, or trade the model or its parts, individually or bundled.  
- Overwrite Roop’s core logic/storage with conflicting systems without clear separation.  

### A.4 Distribution Policy  
Authorized distribution only by KristoStl or explicit collaborators. Any reposting, cloning for resale, or inclusion in unrelated toolkits is forbidden without prior written approval.

### A.5 Storage & Runtime Guidelines  
- `RServer` → `ServerStorage`  
- `RClient` → `ReplicatedStorage`  
- GUIs → `StarterGui`  
- `RemoteEvents` → `ReplicatedStorage`

Re-location or renaming of core folders voids functionality and this license.

### A.6 Attribution  
Display “Roop Services” as a footer, loading-screen badge, or GitHub tag wherever the model is used.

### A.7 Termination (Model)  
Revocation of model privileges if used to:  
- Violate Roblox Terms or Community Standards  
- Mislead players or exploit consent systems  
- Falsely attribute support/staff to Roop’s creator  
- Overload events or break intended storage logic  

---

## 6. Services License (Annex B)  

**Effective Date:** July 12, 2025

This Annex covers Roop Services’ scripts and Roblox assets: modules, UI elements, `RemoteEvents`, folders, and consent systems.

### B.1 Use & Modification  
- Integrate Roop Services into any Roblox Experience.  
- Customize scripts & UI for internal use while preserving authorship.  
- Extend logic: onboarding, analytics, feature flags, modular tooling.  

### B.2 Redistribution  
Permitted **only** within Roblox Experiences.  
Prohibited outside Roblox or as downloadable `.rbxm`/`.rbxl` without written permission.

### B.3 Storage & Asset Guidelines  
- Do not rename: `RClient`, `RServer`, `RoopServicesGUI`.  
- Do not overwrite core modules or events without sandboxing.  
- Do not clone into unrelated projects or store non-Roop content inside Roop folders.  

### B.4 Branding & Attribution  
Encourage “Powered by Roop Services” in your game UI. Do not claim Roop as your own unless fully rewritten.

### B.5 Usage Limitations  
Roop Services must not be used to:  
- Break Roblox’s Terms or Community Standards  
- Mislead players about privacy or functionality  
- Exploit consent/UI outside intended scope  
- Handle sensitive or PII data  

### B.6 No Warranty  
Roop Services is provided “AS IS.” KristoStl disclaims all liability for bugs, misuse, or performance issues.

### B.7 Termination (Services)  
Revocation if assets are:  
- Misused, over-cloned, repurposed maliciously  
- Harming the Roblox ecosystem or reputation  

---

## 7. Permitted Use  
You may:  
- Integrate Roop into **one** Experience per License Key.  
- Fork/clone **privately** for QA, staging, CI/CD pipelines.  
- Display “Powered by Roop” branding on loading screens.  

---

## 8. Prohibited Use  
You may **NOT**:  
- Copy, clone, fork publicly, or mirror Roop code/assets.  
- Sublicense, sell, rent, lease, or assign Roop to third parties.  
- Circumvent license checks, rate-limits, or encryption.  
- Harvest or transmit Unauthorized Data.  
- Embed Roop in automated bots, adware, or phishing tools.  
- Integrate into Experiences targeting under-13 users without consent.  

---

## 9. Distribution & Sub-Licensing  
- Distribution limited to published Roblox Experiences under your account.  
- Offline backups and asset packs require prior written approval.  
- Public GitHub forks must remain **private**.  
- No republishing to package registries (NPM, Rojo, etc.) without consent.

---

## 10. Storage & Integration Guidelines  
- Preserve original folder hierarchy.  
- Do not relocate or rename core modules.  
- Place configuration scripts in locked `ServerStorage`.  
- Use secure HTTPS endpoints for Roop’s remote calls.

---

## 11. Data Privacy & Security  
- Collects only `UserId`, session tokens, API metrics, error logs.  
- No chat logs, IP addresses, emails, or PII.  
- All data encrypted in transit (TLS 1.2+) and at rest (AES-256).  
- Logs auto-purge after 30 days; backups after 60 days.  
- Developers must disclose any extra telemetry and obtain player consent.

---

## 12. Attribution & Branding  
- Include “ Roop Services” or “Powered by Roop” in UIs.  
- Retain original copyright headers.  
- Do not remove any “Authored by KristoStl” labels.

---

## 13. Audit, Monitoring & Compliance  
- KristoStl may audit your private repo with 30 days’ notice.  
- You must provide read-only access for compliance checks.  
- Non-cooperation constitutes material breach.  
- Remediation plans required within 15 days of findings.

---

## 14. Support & Maintenance  
- Community support via GitHub Issues (SLA: 3 business days).  
- Critical patches: within 48 hours of discovery.  
- Premium support available under separate paid agreement.

---

## 15. Fees & Commercial Licensing  
- Non-commercial use: free.  
- Commercial, enterprise, or paid support: separate agreement and fees.  
- Fee schedules negotiated in writing only.

---

## 16. Intellectual Property Rights  
- All Roop IP—code, assets, names, designs—remains KristoStl’s exclusive property.  
- Contributions or feedback you submit become KristoStl’s property under a royalty-free license.

---

## 17. Disclaimers & Limitation of Liability  
- Roop is provided “AS IS” without warranties.  
- KristoStl disclaims all liability for data loss, crashes, security breaches, or misuse.  
- Liability cap: **CAD 100** total under any theory.

---

## 18. Indemnification  
You agree to defend, indemnify, and hold harmless KristoStl and affiliates against any third-party claims arising from your breach or misuse of Roop.

---

## 19. Termination & Suspension  
- Breach of any term: immediate, automatic termination.  
- Upon termination, remove all Roop assets from Experiences and backups.  
- Destroy or encrypt any existing forks or CI artifacts.  
- Appeals for reinstatement accepted within 15 days; subject to KristoStl’s sole discretion.

---

## 20. Modifications & Updates  
- KristoStl may update this LICENSE.md at any time.  
- New Effective Date indicates revisions.  
- Continued use after changes = acceptance.  
- Major version upgrades require a new license.

---

## 21. Governing Law & Dispute Resolution  
- Governed by the laws of **Alberta, Canada**.  
- Disputes resolved exclusively in **Calgary courts** or binding arbitration under Canadian rules.

---

## 22. No Waiver  
Failure to enforce any provision does not waive future enforcement.

---

## 23. Severability  
If any provision is unenforceable, the remainder stay in effect.

---

## 24. Assignment  
You may not assign or transfer your rights without prior written consent from KristoStl.

---

## 25. Entire Agreement  
This document (including Annex A & B) is the entire agreement and supersedes any prior communications.

---

## 26. Revision History  
| Date       | Version | Summary                                                                      |
|------------|---------|-------------------------------------------------------------------------------|
| 2025-07-12 | 1.0     | Initial Model & Services annexes                                              |
| 2025-07-13 | 1.1     | Merged Original License, Annexes, expanded definitions & installation guides   |
| 2025-08-01 | 1.2     | Added audit, support, fees, indemnification, and commercial clauses            |
| 2025-08-25 | 1.3     | Enhanced Privacy Security rules, storage guidelines, and distribution controls |
| 2025-09-15 | 1.4     | Clarified termination, no-waiver, severability, and dispute-resolution clauses |

---

**By integrating, using, or distributing Roop in any form, you irrevocably agree to these terms in full. Build responsibly, safeguard player data, and honor the Roop framework. 🚀**  
