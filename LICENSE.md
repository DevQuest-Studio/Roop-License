# 🎯 Roop Framework LICENSE.md  
**📅 Effective Date:** July 13, 2025  
**✍️ Author:** KristoStl ([GitHub](https://github.com/KristoStl))  

---

## 📑 Table of Contents  
  1. [Definitions](#1-definitions) 
  2. [Grant of License](#2-grant-of-license)
  3. [Installation & Activation](#installation--activation) 
  4. [Scope of Use](#scope-of-use)
  5. [Annex A: Roop Model License](#annex-a-roop-model-license)
  6. [Annex B: Roop Services License](#annex-b-roop-services-license)
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
- **Roop**: The complete Roblox framework—model files (`.rbxm`/`.rbxl`), Remote Modules, packages, scripts, GUIs, signals, assets, configurations, and documentation—authored by KristoStl.  
- **Repository**: `https://github.com/KristoStl/Roop` (all branches, tags, releases).  
- **Developer / You / Your**: Any person or entity accessing, forking, cloning, integrating, or distributing Roop.  
- **Experience**: A Roblox Place or Universe embedding Roop.  
- **License Key**: A 32-character alphanumeric code issued by KristoStl to authorize one Experience.  
- **Activation API**: HTTPS endpoint that validates your License Key at runtime.  
- **Unauthorized Data**: Any player or system data beyond Roblox `UserId`, session tokens, and owner-approved telemetry.  
- **Minor Update**: Patch or bug-fix release within v1.x.  
- **Major Upgrade**: Version bump to v2.0.0 or above (requires new license).  
- **Derivative Works**: Any adaptation, translation, or extension of Roop’s code, assets, or docs.  
- **Audit**: Authorized inspection of your codebase, activation logs, or usage metrics.  
- **Force Majeure**: Events beyond reasonable control (acts of God, government orders, widespread outages).  

---

## 2. Grant of License  
- Roop is **licensed**, not sold; all rights not expressly granted are reserved by KristoStl.  
- You receive a **limited**, **non-exclusive**, **non-transferable**, **revocable** license to integrate and use Roop in **one** Experience per License Key.  
- This license covers all **Minor Updates** (v1.x) at no additional fee.  
- **Major Upgrades** (v2.0+) require execution of a new, written license agreement.  
- You may clone or fork the Repository **privately** for development, QA, staging, or CI/CD.  
- You may distribute compiled ModuleScripts that invoke Roop—**never** raw `.rbxm`/`.rbxl` assets.  
- You may archive encrypted backup copies of Roop for disaster recovery.  
- You may integrate Roop’s client/server APIs exactly as documented.  
- You may display a “Powered by Roop” badge on loading screens or footers.  
- You may enable opt-in telemetry; end-user disclosure is required.  
- You may run closed alpha/beta tests under a **Beta License** (expires after 30 days).  
- You may localize UI text and fonts, provided ModuleScript APIs remain unchanged.  
- You may use Roop in group-owned Experiences if you hold primary dev rights.  
- You may spawn up to **10** concurrent Roop Manager instances per server process.  
- License is void if you sublicense, sell, lease, or assign it to any third party.  

---

## 3. Installation & Activation  
1. Obtain Roop **only** from this official Repository. Third-party mirrors are prohibited.  
2. Follow `/docs/INSTALL.md` **step by step**; skipping steps voids your license.  
3. Place `Settings.lua` and `Activation.lua` in a locked `ServerStorage/RoopConfig` folder.  
4. Insert your **PlaceId** and **License Key**; do **not** commit them to source control.  
5. Activation uses HTTPS/TLS 1.2+; HTTP is unsupported and will be blocked.  
6. On game startup, `Activation.lua` contacts the Activation API with your PlaceId and Key.  
7. If validation fails, Roop enters **Safe Mode**: all non-essential features disable.  
8. Five consecutive failed activations lock your License Key for 24 hours.  
9. Report any License Key compromise to kristostl@example.com within 24 hours.  
10. CI/CD pipelines may call the Activation API via encrypted environment variables only.  
11. Activation logs are AES-256 encrypted in `ServerStorage/RoopLogs/activations.json`.  
12. KristoStl may read these logs (read-only) for compliance audits.  
13. Do **not** rename or relocate `Activation.lua`; doing so breaks license enforcement.  
14. Activation is rate-limited to **100** calls/hour per PlaceId; excess calls are throttled.  
15. Offline testing is allowed for up to **48 hours**—live activation required thereafter.  
16. Staging keys auto-expire after 30 days; production keys renew annually.  
17. Key rotation requires revoking the old key, then requesting a new one.  
18. Key revocation events trigger email alerts to kristostl@example.com and the Experience owner.  
19. Any attempt to intercept or spoof Activation API traffic voids your license immediately.  
20. Automated remediation scripts may re-activate keys only with an Owner-signed token.  
21. A self-hosted Activation API is possible under a separate NDA and addendum.  

---

## 4. Scope of Use  
- Valid for **one** live Experience per License Key.  
- Permitted in personal, educational, non-commercial, or internal team environments.  
- Supports closed alpha/beta test deployments (up to 100 concurrent testers).  
- Prohibited outside Roblox (no headless servers, non-Roblox engines, or other platforms).  
- You may integrate Roop with Roblox Economy APIs under Roblox’s standard terms.  
- You may combine Roop with other approved frameworks if namespaces do not collide.  
- You may enable in-game developer consoles for Roop debug output.  
- You may not expose Roop internals via public HTTP endpoints or developer tools.  
- You may wrap Roop’s consent UI around select third-party modules if flow remains intact.  
- You may not proxy Roop calls through unauthorized middleware or proxies.  
- Debouncing or throttling is allowed—respect the documented maximum rate limits.  
- You may integrate Roop data into your own leaderboards; do not alter group-ID logic.  
- You may deploy Roop on mobile, PC, console, or VR interchangeably.  
- You may not require end-users to accept additional terms for Roop beyond your own.  
- You may conduct private workshops on Roop under a **Confidential Addendum**.  
- You may not host unmoderated chat rooms or voice channels using Roop signals.  
- You may overlay your own moderation filters on top of Roop’s event system.  

---

## 5. Annex A: Roop Model License  
**📅 Effective Date:** July 12, 2025  
This Annex covers the Roop Services **model file** (`.rbxm`/`.rbxl`), including embedded ModuleScripts, GUIs, folders, assets, and configurations.

### Model Scope & Contents  
- Folder structure: `RClient`, `RServer`, `StarterKit`, `Signals`  
- Embedded `ModuleScripts` & `LocalScripts`  
- GUI layouts & containers  
- `RemoteEvents`, signals, and handlers  
- Plugin-style loader systems & setup scripts  

### Permitted Use  
- Use Roop model assets in personal or team Roblox Experiences.  
- Modify scripts, GUIs, and folders for internal development and styling.  
- Extend or wrap modules for custom onboarding, analytics, localization, or tooling.  

### Restricted Use  
- Re-upload or rebrand the model under another name or group.  
- Sell, rent, or trade the model or its individual components.  
- Overwrite Roop’s core logic/storage with conflicting systems without clear separation.  

### Distribution Policy  
- Only KristoStl or authorized collaborators may redistribute the model.  
- Written approval is required for inclusion in third-party toolkits or asset bundles.  

### Storage & Runtime Guidelines  
- `RServer` → `ServerStorage`  
- `RClient` → `ReplicatedStorage`  
- GUI assets → `StarterGui`  
- `RemoteEvents` → `ReplicatedStorage` or designated loader module  

> Relocating or renaming core folders voids functionality and license.

### Attribution  
- Display “Roop Services” on footers, loading screens, or GitHub tags.  

### Termination (Model)  
- License revoked if the model is used to violate Roblox rules, exploit data, misattribute authorship, or overload event systems.

---

## 6. Annex B: Roop Services License  
**📅 Effective Date:** July 12, 2025  
This Annex governs Roop Services’ scripts, modules, UI elements, `RemoteEvents`, folders, and consent systems.

### Use & Modification  
- Integrate Roop Services into any Roblox Experience.  
- Customize scripts & UI internally, preserving original authorship and structure.  
- Extend logic for onboarding flows, analytics hooks, feature flags, and tooling.  

### Redistribution  
- Permitted only within Roblox Experiences; no external `.rbxm`/`.rbxl` downloads or repackaging without written consent.  

### Storage & Asset Guidelines  
- Do **not** rename core folders (`RClient`, `RServer`, `RoopServicesGUI`).  
- Do **not** overwrite remote modules or events without sandboxing.  
- Do **not** clone Roop components into unrelated projects.  
- Do **not** store non-Roop content within Roop folders.  

### Branding & Attribution  
- Encourage “Powered by Roop Services” in your game UI.  
- Do **not** claim Roop as your own unless fully rewritten and uniquely extended.  

### Usage Limitations  
- Must not violate Roblox’s Terms of Service or Community Standards.  
- Must not mislead players about data handling or privacy.  
- Must not exploit consent UI outside of Roop’s intended scope.  
- Must not handle PII or sensitive data beyond what this license allows.  

### No Warranty  
- Roop Services is provided **“AS IS”** with **no warranties**; the creator disclaims all liability for bugs, misuse, or performance issues.  

### Termination (Services)  
- Revoked for misuse, over-cloning, malicious repurposing, or any harm to the Roblox ecosystem.

---

## 7. Permitted Use  
- Integrate Roop in **one** Experience per valid License Key.  
- Fork or clone the Repository **privately** for QA, staging, or CI/CD.  
- Display “Powered by Roop” branding on loading screens or footers.  
- Archive encrypted backups for recovery; purge logs after 60 days.  

---

## 8. Prohibited Use  
- Publicly fork, clone, mirror, or redistribute Roop assets or code.  
- Sublicense, sell, rent, lease, or assign Roop license to third parties.  
- Bypass license checks, rate-limits, or built-in encryption.  
- Harvest or transmit Unauthorized Data (chat logs, IPs, PII).  
- Embed Roop in bots, adware, phishing, or other malicious tools.  
- Target under-13 users without parental consent flows.  

---

## 9. Distribution & Sub-Licensing  
- Distribution limited to published Roblox Experiences under your account.  
- Offline asset packs or backups require prior written approval.  
- Public GitHub forks must remain in **private** repositories.  
- No publishing to external package registries (Rojo, NPM, etc.) without consent.  

---

## 10. Storage & Integration Guidelines  
- Preserve original folder hierarchy and file names.  
- Configuration scripts belong in locked `ServerStorage/RoopConfig`.  
- Use HTTPS for all Roop remote calls; HTTP is blocked.  
- Do not relocate or merge core modules; doing so voids this license.  

---

## 11. Data Privacy & Security  
- Collects only Roblox `UserId`, session tokens, approved telemetry, and error logs.  
- Does **not** collect chat logs, IP addresses, email addresses, or other PII.  
- Encrypt all data in transit (TLS 1.2+) and at rest (AES-256).  
- Auto-purge logs after 30 days; backups after 60 days.  
- Developer-added telemetry must be disclosed to end users and comply with GDPR/CCPA/COPPA where applicable.  

---

## 12. Attribution & Branding  
- Include “Roop Services” or “Powered by Roop” in your game UI.  
- Retain all copyright, trademark, and authorship notices in source headers.  
- Do **not** remove or obfuscate “Authored by KristoStl” labels.  

---

## 13. Audit, Monitoring & Compliance  
- KristoStl may audit your private repo or activation logs with 30 days’ notice.  
- Read-only access is sufficient; non-cooperation is a material breach.  
- Submit remediation plans within 15 days of any audit findings.  
- Failure to comply may result in license revocation and legal action.  

---

## 14. Support & Maintenance  
- Community support via GitHub Issues (SLA: 3 business days).  
- Critical security patches released within 48 hours of discovery.  
- Premium support (24/7, concierge) under separate paid agreement.  

---

## 15. Fees & Commercial Licensing  
- Non-commercial, personal, educational use is free.  
- Commercial, enterprise, or monetized use requires a paid license and fee schedule.  
- All commercial terms must be agreed in writing before distribution.  

---

## 16. Intellectual Property Rights  
- All Roop code, assets, folder designs, and logic are the exclusive property of KristoStl.  
- Contributions or feedback you submit become KristoStl’s property under a perpetual, royalty-free license.  

---

## 17. Disclaimers & Limitation of Liability  
- Roop is provided **“AS IS”** without warranties of any kind.  
- KristoStl disclaims liability for integration errors, game crashes, data loss, or security breaches.  
- Under no circumstances shall KristoStl’s total liability exceed **CAD 100**.  

---

## 18. Indemnification  
- You agree to indemnify and hold harmless KristoStl, its affiliates, and contributors from any claims arising out of your breach or misuse of Roop.  

---

## 19. Termination & Suspension  
- Breach of any term leads to **immediate** termination of your license.  
- Upon termination, remove all Roop assets from live and archived Experiences.  
- Delete or permanently encrypt any forks, CI/CD artifacts, or backups.  
- Appeals for reinstatement accepted within 15 days; final decision at KristoStl’s sole discretion.  

---

## 20. Modifications & Updates  
- KristoStl may update this LICENSE.md at any time; new **Effective Date** signals changes.  
- Continued use after any update constitutes unconditional acceptance.  
- Major version upgrades require execution of a new license agreement.  

---

## 21. Governing Law & Dispute Resolution  
- This license is governed by the laws of **Alberta, Canada**.  
- All disputes shall be settled exclusively in the courts of **Calgary, Alberta**, or by binding arbitration under Canadian rules.  

---

## 22. No Waiver  
- Failure by the Owner to enforce any provision does not constitute a waiver of future enforcement rights.  

---

## 23. Severability  
- If any provision is held invalid or unenforceable, the remainder of this license remains in full effect.  

---

## 24. Assignment  
- You may not assign or transfer your rights or obligations under this license without prior written consent from KristoStl.  

---

## 25. Entire Agreement  
- This LICENSE.md (including Annexes A & B) constitutes the entire agreement between you and KristoStl, superseding all prior or contemporaneous communications.  

---

## 26. Revision History  
| Date       | Version | Summary                                                           |
|------------|---------|-------------------------------------------------------------------|
| 2025-07-12 | 1.0     | Initial Model & Services Annexes                                 |
| 2025-07-13 | 1.1     | Merged core License with Annexes, expanded Definitions & Grant    |
| 2025-08-01 | 1.2     | Added Installation, Scope, Audit, Support, Fees & Liability       |
| 2025-08-25 | 1.3     | Tightened Privacy, Distribution, Enforcement, COPPA/GDPR Nods     |
| 2025-09-15 | 1.4     | Clarified Termination, No-Waiver, Severability, and Dispute Rules |

---

**By accessing, integrating, or distributing Roop in any form, you irrevocably agree to all terms above.  
Build responsibly, safeguard player data, and honor the Roop framework. 🚀**  
