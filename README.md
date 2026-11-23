# MODERN STACK // 2026

> **[English](README.md)** | **[Русский](README.ru.md)**

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-00F0FF?style=for-the-badge&logo=github)](https://vedariy.github.io/modern-stack/)
[![Zero Dependencies](https://img.shields.io/badge/Build%20Step-Zero%20Dependencies-10B981?style=for-the-badge)](https://vedariy.github.io/modern-stack/)
[![Native Web APIs](https://img.shields.io/badge/APIs-100%25%20Browser%20Native-7C3AED?style=for-the-badge)](https://vedariy.github.io/modern-stack/modern-stack-2026.html)

**Interactive visual simulators of modern and late-2026 web architecture.**  
Explore React Server Components & Islands, Edge Computing, Native CSS & WebAssembly, Offline-First PWA & VAPID Web Push, WebRTC/QUIC, FIDO2 Passkeys, SubtleCrypto, WebMCP, and Local-First OPFS/CRDT engines directly in your browser — with zero build steps or external backend dependencies.

---

## Live Deployment

- **Portfolio Hub (EN / RU):** [https://vedariy.github.io/modern-stack/](https://vedariy.github.io/modern-stack/)
- **Flagship 7-Module Simulator (`MODERN STACK // 2026`):** [https://vedariy.github.io/modern-stack/modern-stack-2026.html](https://vedariy.github.io/modern-stack/modern-stack-2026.html)
- **Standalone Web Push & VAPID Simulator:** [https://vedariy.github.io/modern-stack/webpush-simulator.html](https://vedariy.github.io/modern-stack/webpush-simulator.html)

---

## Interactive Simulators

### 1. [MODERN STACK // 2026](https://vedariy.github.io/modern-stack/modern-stack-2026.html) (`modern-stack-2026.html`)
A cinema-class, 7-module architecture showcase with an interactive fiber-optic pipeline, **Auto-Tour** mode, and a **`⌘K` Agentic Command Bar**:

| Module | Topic | What You Can Test |
| :--- | :--- | :--- |
| **01** | **Islands Architecture & RSC** | Switch between Legacy Monolithic SPA and Modern RSC + Islands; hydrate individual islands and watch LCP, INP, JS payload, and the main-thread flamegraph update live. |
| **02** | **Edge Computing & Global Routing** | Fire requests from Berlin, Tokyo, and São Paulo to compare Edge Workers + KV (`5–8ms`) against Single Origin DB round-trips (`148–214ms`). |
| **03** | **Native Browser Superpowers** | Resizable CSS `@container` queries, View Transitions API shared-element gallery, and a Wasm SIMD vs. Single-Thread JS particle benchmark. |
| **04** | **Offline-First PWA & Web Push** | Simulate Airplane Mode and a Closed Browser Tab while `sw.js` wakes in the background to decrypt VAPID `p256dh`/`auth` notifications. |
| **05** | **End-to-End Type Safety** | Toggle a database column type (`number` vs. `string`) and watch inference or compile-time TypeScript errors propagate across DB Schema → Server RPC → React UI Props. |
| **06** | **Real-Time & Zero-Trust Crypto** | 4-lane packet highway comparing **WebRTC (UDP/SRTP)**, **WebTransport (QUIC)**, and **WebSockets (TCP)** with 15% packet loss; **FIDO2 Passkey** phishing simulator; live `window.crypto.subtle` (`ES256`, `HMAC-SHA256`, `DPoP`) signing & tamper test. |
| **07** | **Late-2026 Browser Frontier** | **WebMCP** (`navigator.modelContext`) agent tool registry vs. DOM scraping; **Local-First OPFS SQLite + CRDT** dual-device offline sync; draggable **CSS Anchor Positioning + `contrast-color()`**; **WebGPU / WebNN** inference meter. |

### 2. [Web Push & VAPID Simulator](https://vedariy.github.io/modern-stack/webpush-simulator.html) (`webpush-simulator.html`)
A focused, step-by-step visual simulator (RU UI) demonstrating Service Worker registration, `PushSubscription` (`endpoint`, `p256dh`, `auth`), VAPID JWT signing, E2E encryption, and background OS notifications when the browser tab is closed.

---

## Repository Structure

```text
Vedariy/modern-stack/
├── index.html                  # Bilingual EN/RU Landing Hub with ⌘K Command Palette
├── modern-stack-2026.html      # Flagship 7-Module Web Architecture Simulator
├── webpush-simulator.html      # Standalone Web Push & VAPID Simulator
├── README.md                   # English documentation
└── README.ru.md                # Russian documentation
```

### Roadmap Blueprints
- **Module 08 (`zero-latency-identity.html`):** Speculation Rules 0ms MPA prerendering, Trusted Types DOM XSS Firewall, W3C Digital Credentials & SD-JWT.
- **Module 09 (`hardware-spatial-web.html`):** WebHID/WebSerial/WebBluetooth, WebXR Spatial Computing, WebCodecs + AudioWorklet DSP, HDR `oklch()`.

---

## Run Locally

Because every simulator is a self-contained static HTML file using native browser APIs (including Web Crypto), serve the directory over a local HTTP server:

```bash
git clone https://github.com/Vedariy/modern-stack.git
cd modern-stack
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.