# 🌟 Roop Official GitHub Repository  
## ⚖️ Terms of Service · Privacy Policy · Integration & Usage License  
**Effective Date:** July 13, 2025  

---

## 📑 Table of Contents

1. [Definitions](#1-definitions)  
2. [End User License Agreement (EULA)](#2-end-user-license-agreement-eula)  
3. [Privacy Policy](#3-privacy-policy)  
4. [Integration & Usage License](#4-integration--usage-license)  
5. [Usage Rules & Prohibited Practices](#5-usage-rules--prohibited-practices)  
6. [Intellectual Property & Ownership](#6-intellectual-property--ownership)  
7. [Third-Party Components & Dependencies](#7-third-party-components--dependencies)  
8. [Fees & Commercial Licensing](#8-fees--commercial-licensing)  
9. [Disclaimers & Limitation of Liability](#9-disclaimers--limitation-of-liability)  
10. [Indemnification](#10-indemnification)  
11. [Termination & Enforcement](#11-termination--enforcement)  
12. [Modifications & Updates](#12-modifications--updates)  
13. [Governing Law & Jurisdiction](#13-governing-law--jurisdiction)  
14. [Notices & Contact](#14-notices--contact)  
15. [Revision History](#15-revision-history)  

---

## 1. Definitions

- Roop: The Roblox Model, Remote Module, Package, assets, code, and documentation provided by @kristostl.  
- Repository: This GitHub repo hosting Roop’s source, docs, and license.  
- Developer: Any person or organization accessing, cloning, forking, or integrating Roop.  
- You/Your: Synonymous with “Developer.”  
- Unauthorized Data: Any personal player data or usage metrics beyond what Roop expressly collects.  

---

## 2. End User License Agreement (EULA)

### 2.1 Grant of License  
- Roop is licensed, not sold, to you under this EULA.  
- You receive a limited, non-exclusive, non-transferable license to install Roop in one Roblox game.  
- This license permits up to five instances of Roop per game, for development, testing, and production.  
- You may create derivative game logic around Roop’s APIs but not derivative copies of Roop assets.  
- License covers all current versions and minor updates (bug-fixes, performance patches).  
- Major version upgrades may require a renewed license agreement.  
- License includes use of Roop’s user interface components in accordance with branding guidelines.  
- You may distribute compiled Lua scripts that invoke Roop but not Roop’s source files themselves.  
- You may bundle Roop with your game on Roblox, provided Roop’s files remain individually named and unencrypted.  
- You may implement Roop in closed or invite-only experiences, respecting Roblox Terms of Service.  
- You may customize UI labels and colors, but not the core functionality signature of Roop.  
- You may use Roop in non-commercial, educational, or testing environments without additional fees.  
- You may integrate Roop with internal analytics, as long as you do not extract data beyond Section 3.  
- You may enable logging of Roop error codes in your own dashboards for debugging.  
- You may share screenshots or demo videos of Roop in action for marketing your game.

### 2.2 Installation & Activation  
- Obtain Roop from this GitHub repository; do not rely on third-party mirrors.  
- Follow the installation guide in /docs/INSTALL.md exactly.  
- Activation requires embedding your Roblox place ID and license key in Settings.lua.  
- License key is single-use per project and must not be exposed publicly.  
- Activation call occurs at game initialization; failure to activate disables Roop features.  
- Installation via Asset-Service is permitted only with the official asset bundle ID.  
- Do not rename folders or mismatch module script hierarchies; this voids the license.  
- Ensure network requests to Roop’s CDN are allowed; offline operation is unsupported.  
- Activation logs are stored encrypted in ServerStorage/roop_activations.json.  
- Unauthorized tampering with Activation.lua triggers self-destruct logic after five failed attempts.  
- You may automate activation in CI/CD pipelines with encrypted environment variables.  
- You must record activation transactions for audit by @kristol upon request.  
- Installation into multiple games requires a separate license per game.  
- Testing licenses may be issued upon request for quality assurance purposes.  
- All installation scripts must include a header comment linking back to this EULA.

### 2.3 Scope of Use  
- Licensed use is limited to one published Roblox place per license key.  
- You may use Roop in experience bundles and group universe games if they share a single place ID.  
- You may allow others to play in your universe but not to access Roop’s codebase.  
- You may not bundle Roop with any game editor or modding tool for external distribution.  
- You may reference Roop’s API in your game documentation for end users.  
- You may teach Roop integration in closed workshops under a temporary educational addendum.  
- You may not use Roop in headless server deployments outside Roblox’s official hosting.  
- You may not use Roop to provide a multiplayer lobby system outside your own experience.  
- You may call Roop’s functions only from authorized contexts (server or client as specified).  
- Roop’s data endpoints may only be invoked over secure HTTPS channels.  
- Roop’s services must not be proxied through third-party gateways without approval.  
- You may not circumvent Roblox rate limits for HTTPService when using Roop.  
- You may log usage counts but must not exceed 1,000 API calls per minute aggregate.  
- You may not use Roop to perform batch downloads or bulk player exports.  
- You may not rent or sell access to Roop’s license to any third party.

### 2.4 License Restrictions  
- You may not sublicense, resell, rent, lease, or assign your license to any third party.  
- You may not reverse-engineer, decompile, disassemble, or otherwise attempt to derive source from Roop.  
- You may not remove, obscure, or alter any proprietary notices or labels in Roop assets.  
- You may not use Roop to create illegal, harmful, or offensive content within Roblox.  
- You may not use Roop to mine cryptocurrency or perform unauthorized compute tasks.  
- You may not host Roop’s components on servers outside the Roblox platform.  
- You may not integrate Roop into bots or automated accounts that violate Roblox rules.  
- You may not combine Roop with DRM or licensing wrappers that obscure its origin.  
- You may not use Roop to generate false or misleading logs or audit trails.  
- You may not bypass Roop’s built-in rate limiting, authentication, or encryption.  
- You may not adapt Roop for other game engines or platforms without a distinct cross-platform license.  
- You may not claim ownership of Roop or represent it as your own work.  
- You may not affiliate Roop with political or religious campaigns without explicit approval.  
- You may not publish comparative benchmarks of Roop that are inaccurate or defamatory.  
- You may not exploit Roop’s feedback channels to spam or harass @kristol.

### 2.5 Termination & Consequences  
- Your license terminates immediately upon breach of any EULA term.  
- Upon termination you must remove Roop modules from all places and archives.  
- You must purge any backups or CI caches containing Roop source.  
- You may be required to furnish a sworn statement of compliance within 10 days.  
- We may remotely deactivate your license key if we detect unauthorized use.  
- Termination does not waive @kristol’s rights to seek injunctive relief.  
- You remain liable for any unpaid fees or damages incurred prior to termination.  
- If you cease development, notify kristol@example.com to deactivate the license.  
- Survival clauses: Sections 6, 9, 10, 11, 13, and 15 survive termination.  
- Disputes over termination are governed by Section 13’s jurisdiction clause.  
- You may appeal termination within 15 days with documented corrective actions.  
- Appeals must include remediation plans and timeline for compliance.  
- Requests for reinstatement are at @kristol’s sole discretion.  
- Termination or suspension may also occur for repeated support neglect.  
- Any extension of license post-termination requires execution of a new agreement.  

---

## 3. Privacy Policy

### 3.1 Data Collection  
- Roop collects Roblox UserId and session tokens for authentication.  
- Usage metrics include API call names, counts, timestamps, and error codes.  
- Performance logs capture memory usage and execution time per call.  
- No collection of player chat, voice, personal details, or IP addresses.  
- Optional telemetry may capture device OS, client version, and region code.  
- Telemetry is off by default; you must opt in via Settings.lua.  
- Opt-in telemetry does not send player identifiers beyond anonymous IDs.  
- We do not store any user email, username, or profile picture.  
- We do not integrate with external advertising or marketing lists.  
- Data flows only between Roblox servers and Roop’s secured cloud endpoints.  
- Developers may configure additional data collection under their own policies.  
- Any additional data collected by your game is outside Roop’s scope.  
- You must disclose any developer-custom data collection in your own policy.  
- Roop’s data collection is scoped per-instance and segregated by GameId.  
- Data snapshots are hashed and cannot be reverse-engineered into raw logs.

### 3.2 Use of Cookies & Tracking  
- Roop’s web-based dashboard (if used) employs secure cookies for session keep-alive.  
- Cookies are session-only and expire on browser close.  
- No persistent tracking cookies, third-party trackers, or cross-site scripts.  
- CSRF tokens protect any dashboard forms.  
- LocalStorage is not used for sensitive information.  
- Browser fingerprinting is explicitly prohibited.  
- We do not place analytics scripts on your Roblox game pages.  
- Any cookies on developer tools are fully documented and user-controlled.  
- Cookie settings and opt-out instructions are published at /docs/PRIVACY.md.  
- You as Developer must inform players if you enable the dashboard feature.

### 3.3 Data Sharing & Disclosure  
- We share data only with your own game’s authorized servers.  
- We do not sell, trade, or rent any collected data to third parties.  
- We may disclose data to comply with legal obligations (subpoenas, DMCA).  
- We may disclose to prevent imminent physical harm or fraud.  
- We notify affected Developers within 48 hours of compelled disclosure.  
- Aggregated anonymous metrics may be published for community insights.  
- Aggregated data never includes raw UserIds or session tokens.  
- Developer may request a full audit log report via kristol@example.com.  
- We do not transfer data to jurisdictions lacking adequate privacy laws without notice.  
- Cross-border transfers occur via encrypted channels with standard contractual clauses.  

### 3.4 User Rights  
- Players have the right to access what data Roop holds on them (UserId logs).  
- Players may request deletion of their session logs within 30 days of activity.  
- Deletion requests processed within 14 days of verified request.  
- Players may object to certain data processing by contacting the Developer.  
- You must publish your own in-game data request UI if you collect additional data.  
- Data portability: players may request export of their anonymous usage metrics.  
- You as Developer must inform players of their rights where Roop is integrated.  
- Roop itself does not provide direct player UI; Developers must implement request flows.  
- Complaints about Roop’s data practices route to kristol@example.com.  

### 3.5 Data Security  
- All data in transit is encrypted via HTTPS/TLS 1.2 or higher.  
- At rest, data is encrypted using AES-256 or equivalent.  
- Access to production logs restricted to authorized DevOps personnel.  
- Daily vulnerability scans and quarterly penetration tests are conducted.  
- You must not store sensitive data in plain text within your game’s DataStores.  
- Security incidents are reported to affected Developers within 72 hours.  
- We maintain an incident response plan with escalation to CERT standards.  
- You must update to the latest Roop version within 30 days of a critical fix.  
- You may subscribe to security bulletins via the GitHub Releases RSS feed.  

### 3.6 Data Retention  
- Usage metrics and logs are retained for a maximum of 30 days.  
- After 30 days, data is automatically purged without manual intervention.  
- Backups containing logs are purged on a 60-day rotation.  
- You may configure shorter retention within Settings.lua.  
- You may request manual purge of all logs at any time via email.  

### 3.7 Children’s Privacy  
- Roop is not directed at children under 13.  
- If your game attracts users under 13, you must obtain parental consent.  
- You may disable telemetry and analytics for accounts under 13.  
- You must not collect any PII from users under 13 through Roop.  
- You must provide you own parental control disclosures if needed.  
- You must comply with COPPA or equivalent local laws when applicable.  

### 3.8 Data Breach Notification  
- In the event of a breach, we will notify affected Developers within 72 hours.  
- Notification includes nature of breach, data types affected, and remediation steps.  
- We will cooperate with you on public disclosures if required by law.  
- You must follow your own breach-response plan for player notification.  
- We will not be held liable for third-party breaches outside Roop’s infrastructure.  

### 3.9 Cross-Border Transfers  
- Data may be stored in data centers in Canada and the United States.  
- Transfers comply with Standard Contractual Clauses (SCC) where required.  
- Developers may request a data processing addendum for GDPR compliance.  

### 3.10 Policy Updates & Notices  
- Privacy Policy may be updated; Effective Date will reflect changes.  
- Material changes will be highlighted in the Revision History.  
- Continued use after updates constitutes acceptance.  
- You must surface policy changes to your players via in-game notices.

---

## 4. Integration & Usage License

### 4.1 License Scope  
- This license covers integration of Roop’s Model, Remote Module, and Package in one Roblox game.  
- Permitted to distribute your final game build on Roblox anonymously named “Roop-enabled.”  
- You may embed Roop’s remote calls only within authorized ServiceScripts and ModuleScripts.  
- You may invoke Roop’s APIs for group creation, membership checks, and data fetches.  
- You may extend Roop’s event handlers to trigger custom in-game logic (e.g., UI popups).  
- You may map Roop’s group data onto your own leaderboard or statistics panel.  
- You may schedule automated in-game announcements based on Roop data.  
- You may use Roop’s utility functions for caching and debounce mechanics.  
- You may instantiate up to 10 concurrent Roop objects per server instance.  
- You may implement Roop’s feature flags to enable/disable modules in runtime.  
- You may include Roop in game templates distributed to your team members.  
- You may use Roop’s test suite in CI; you may not include license keys in public repos.  
- You may call Roop from client scripts only for UI and read-only operations.  
- You may call Roop from server scripts for read/write operations, subject to rate limits.  
- You may whitelist specific UserIds in Settings.lua for alpha/beta testing.

### 4.2 Distribution & Sub-licensing  
- You may package your game as an Experience Bundle including Roop.  
- You may not create a separate sub-license; distribution rights do not extend to Roop.  
- Every end user must agree to your game’s EULA which must reference Roop’s EULA.  
- You may not distribute Roop’s source; only compiled ModuleScripts and Asset IDs.  
- Redistribution of Roop outside Roblox’s platform is forbidden.  
- You may create custom installers for private servers, provided Roop’s license is enforced.  
- You may not embed Roop’s files in non-Roblox executables.  
- You may not rent or sell server-hosted instances of your game with Roop included.  
- You may offer managed hosting of your Experience Bundle, subject to commercial license.  
- You may archive offline backups for disaster recovery; access restricted to your org.  
- You may not deposit Roop modules in any public package registry.  
- You may not use Roop modules in any service outside of Roblox Universe.

### 4.3 Modification & Customization  
- You may patch Roop’s UI templates for color, font, and layout alignment.  
- You may not modify core Remote Module logic, function names, or parameter contracts.  
- You may wrap Roop’s functions in your own abstractions but may not alter return values.  
- You may not extend ModuleScripts in-place; create wrappers in separate files.  
- You may define new event listeners on Roop’s signal objects.  
- You may customize error messages for localization but not remove original codes.  
- You may add debug hooks around Roop’s performance counters.  
- You may not rename Roop’s primary ModuleScript files or class names.  
- You may not strip out license checks or obfuscate activation logic.  
- You may maintain your own fork for internal use only; no public forks allowed.  
- You may propose changes via pull requests but require explicit merge approval.  
- You may not submit pull requests that remove license or copyright headers.  
- You may include your own asset references alongside Roop’s assets.  
- You may adjust retry logic on failed HTTP calls within Roop’s settings.  
- You may disable optional modules in Settings.lua by toggling feature flags.

### 4.4 Deployment & Compliance  
- You must deploy only through Roblox’s official publishing workflows.  
- You must tag all releases with semantic versioning prefixed by “roop-” (e.g. roop-1.0.0).  
- You must include LICENSE.md and PRIVACY.md in your repository root.  
- You must run an automated compliance check before each release.  
- You must ensure that no unauthorized code commits reach your main branch.  
- You must document any custom integration steps in /docs/INTEGRATION.md.  
- You must provide a changelog of your own modifications in /CHANGELOG.md.  
- You must label all code that interacts with Roop as “Roop Integration Code.”  
- You may not circumvent Roblox’s moderation review by hiding Roop usage.  
- You must confirm compliance with this license in writing annually.  
- You grant @kristol the right to audit your repository on 30 days’ notice.  
- You must respond to audit findings within 15 days with corrective actions.  
- You must ensure that your team is informed of all license obligations.  
- You may not delegate license compliance to third-party contractors without written notice.  
- You may not employ rogue or unvetted developers to work on Roop-enabled code.

### 4.5 License Key & Activation  
- Each license key is a 32-character alphanumeric string tied to your GameId.  
- License key must be stored securely in encrypted form within ServerStorage.  
- Activation API is rate-limited to 100 calls per hour per GameId.  
- Failed activation attempts above 5 in a rolling hour lock out the GameId for 24 hours.  
- License key rotation is supported via Admin API; old keys must be revoked.  
- Emergency key revocation may occur if key compromise is detected.  
- You may script automated key rotation but must update Settings.lua accordingly.  
- Activation events are logged with timestamp, GameId, and IP of Roblox gateway.  
- You may view activation logs in the Roop Dashboard under “License Activity.”  
- License breach detection triggers an alert to kristol@example.com and game owner.  
- You may request additional keys for staging environments; these expire in 30 days.  
- You may not use staging keys in production experiences.  
- You must notify @kristol within 24 hours of any key exposure incident.  
- You must confirm re-securing keys before resuming Roop functionality.  
- You agree that license keys are encrypted at rest and not human-readable.

### 4.6 Audit & Compliance Rights  
- @kristol may conduct quarterly compliance audits with 30 days’ notice.  
- Audits cover license usage, source integrity, and data handling practices.  
- You must provide read-only access to your private repo for audit scope.  
- Failure to cooperate with audits constitutes a material breach.  
- Remediation plans must be submitted within 15 days of audit findings.  
- We may revoke your license mid-cycle if critical violations are uncovered.  
- We will provide a confidential audit report with findings and recommendations.  
- You may dispute audit findings by providing counter-evidence.  
- You agree to implement final audit recommendations or face termination.  
- Audit costs beyond routine reviews may be billed to you if non-compliance occurs.

### 4.7 Support & Maintenance  
- Basic support is provided via GitHub Issues under “Support” label.  
- Response SLA: 3 business days for standard issues, 24 hours for critical outages.  
- Premium support (24/7, concierge) available under paid agreement.  
- Patches for critical vulnerabilities will be released within 48 hours of discovery.  
- Non-critical feature requests will be triaged and scheduled per roadmap.  
- You may access Roop’s private Slack channel for support if invited.  
- You may attend quarterly live webinars on upcoming Roop features.  
- You may access internal beta builds under NDA.  
- You may opt into early access by subscribing on the Roop Dashboard.  
- You may report bugs anonymously but providing logs accelerates fixes.  
- End-of-life announcements for major versions will be given 6 months in advance.  
- You must upgrade off EOL versions within 90 days to maintain support.  
- You may request extended support for deprecated versions under separate terms.  
- Support scope excludes issues caused by your own custom code.  
- We reserve the right to charge for excessive support beyond normal use.

---

## 5. Usage Rules & Prohibited Practices

- **Respect Players**: No harassment, hate speech, or discrimination in your game’s chat or UI.  
- **No Malicious Code**: Do not inject malware, spyware, adware, or any code that compromises player devices.  
- **No Unauthorized Profiling**: Do not combine Roop with external tracking or analytics to profile players.  
- **Content Moderation**: Implement clear channels for reporting abuse, and enforce bans on cheaters or harassers.  
- **Age Compliance**: Do not target or knowingly collect data from players under 13 without parental consent.  

---

## 6. Intellectual Property & Ownership

- All original IP (code, assets, docs) remain the sole property of @kristol.  
- Roop’s trademarks, logos, and service marks may not be used without express license.  
- Any feedback or contributions you submit are deemed non-confidential and become @kristol’s property.

---

## 7. Third-Party Components & Dependencies

Roop may bundle open-source or third-party libraries. You must:

- Comply with each third party’s license.  
- Acknowledge their copyright in your distributions.  
- Assume all risk and liability for third-party vulnerabilities.

---

## 8. Fees & Commercial Licensing

- This license covers **non-commercial** use only.  
- Commercial use (including monetized games, asset packs, or selling access) requires a separate paid agreement.  
- Fee schedules and terms will be negotiated in writing.

---

## 9. Disclaimers & Limitation of Liability

- **“AS IS”**: Roop comes with no warranties—express or implied, including merchantability or fitness for purpose.  
- **No Uptime Guarantee**: We do not promise continuous availability.  
- **Liability Cap**: In no event shall @kristostl’s total liability exceed CAD 100.  

---

## 10. Indemnification

You agree to indemnify and hold harmless @kristostl, contributors, and their successors from any claims, losses, damages, costs, or expenses relating to:

- Your breach of these Terms.  
- Your misuse of Roop or player data.  

---

## 11. Termination & Enforcement

- Breach of any term results in immediate, automatic termination of your license.  
- Upon termination you must remove all Roop components from your game and destroy all copies.  
- We may seek injunctive relief, damages, and attorneys’ fees.

---

## 12. Modifications & Updates

- We reserve the right to update Roop or these Terms at any time.  
- The “Effective Date” at the top will reflect the latest version.  
- Your continued use constitutes acceptance of such changes.

---

## 13. Governing Law & Jurisdiction

These Terms are governed by the laws of Alberta, Canada. All disputes will be resolved exclusively in the courts of Calgary, Alberta.

---

## 14. Notices & Contact

All notices, requests for permission, or inquiries must be sent to:

- **Email:** kristo.stlo@gmail.com  
- **GitHub:** [@kristostl](https://github.com/kristostl)
- **Roblox:** [@KristoStl](https://www.roblox.com/users/3583112108/profile) 

---

## 15. Revision History

| Date       | Version | Notes                                                                                                                       |
|------------|---------|-----------------------------------------------------------------------------------------------------------------------------|
| 2025-07-13 | 1.0     | Initial release                                                                                                             |
| 2025-07-20 | 1.1     | Added strict anti-replication and data-harvest prohibitions                                                                 |
| 2025-08-05 | 1.2     | Clarified EULA scope, updated privacy retention, cap on liability                                                           |
| 2025-08-25 | 1.3     | Expanded EULA (2.1–2.5) with 75 new lines; Privacy Policy (3.1–3.10) with 75 new lines; License (4.1–4.7) with 75 new lines |
