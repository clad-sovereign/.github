**Sovereign bond tokenization infrastructure for emerging markets**

Clad Sovereign provides compliance-first tokenization infrastructure for finance ministries, debt offices, and state issuers in emerging markets. Built on Substrate/Polkadot for full operational sovereignty.

**Repositories:**
   - `clad-studio` — Open-source Substrate pallet and node
   - `clad-dashboard` — Read-only monitoring dashboard
   - `clad-mobile` — Native mobile signer (private)

**Signing Architecture:**
```mermaid
  flowchart LR
      D[Dashboard<br/>prepare] --> S[Server<br/>call data/proposals]
      S --> MO[Mobile online<br/>show QR]
      MO --> MA[Mobile air-gapped<br/>sign via QR]
      MA -->|signed QR back| MO
```
  - Keys never leave device or touch network
  - All signatures air-gapped
  - Mobile-to-mobile QR only
  - Dashboard = monitoring + batch prep

*[Watch 60-second demo – November 2025](https://www.loom.com/share/dd334230db154f9891f46664ae02aec4)*  
![Clad Signer Demo – Native iOS & Android](https://cdn.loom.com/sessions/thumbnails/dd334230db154f9891f46664ae02aec4-9e6c0699711bd8ff-full-play.gif#t=0.1)\
_(Initial demo shows native iOS/Android biometric connection + live block stream.)_
