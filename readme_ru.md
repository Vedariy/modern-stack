# MODERN STACK // 2026

> **[Русский](README.ru.md)** | **[English](README.md)**

[![GitHub Pages](https://img.shields.io/badge/Открыть%20демо-GitHub%20Pages-00F0FF?style=for-the-badge&logo=github)](https://vedariy.github.io/modern-stack/)
[![Без сборки](https://img.shields.io/badge/Сборка-Без%20зависимостей-10B981?style=for-the-badge)](https://vedariy.github.io/modern-stack/)
[![Нативные API](https://img.shields.io/badge/API-100%25%20браузерные-7C3AED?style=for-the-badge)](https://vedariy.github.io/modern-stack/modern-stack-2026.html)

**Интерактивные визуальные симуляторы современной веб-архитектуры и стандартов конца 2026 года.**  
Изучайте React Server Components и архитектуру островов, граничные вычисления (Edge KV), нативный CSS и WebAssembly, офлайн-PWA и VAPID Web Push, WebRTC/QUIC, FIDO2 Passkeys, SubtleCrypto, WebMCP и Local-First движки на OPFS/CRDT прямо в браузере — без сборщиков и внешнего бэкенда.

---

## Опубликованная страница (GitHub Pages)

- **Главный хаб портфолио (EN / RU):** [https://vedariy.github.io/modern-stack/](https://vedariy.github.io/modern-stack/)
- **Флагманский симулятор из 7 модулей (`MODERN STACK // 2026`):** [https://vedariy.github.io/modern-stack/modern-stack-2026.html](https://vedariy.github.io/modern-stack/modern-stack-2026.html)
- **Симулятор Web Push и VAPID:** [https://vedariy.github.io/modern-stack/webpush-simulator.html](https://vedariy.github.io/modern-stack/webpush-simulator.html)

---

## Интерактивные симуляторы

### 1. [MODERN STACK // 2026](https://vedariy.github.io/modern-stack/modern-stack-2026.html) (`modern-stack-2026.html`)
Визуальный симулятор из 7 модулей с интерактивным конвейером передачи данных, режимом **Auto-Tour** и агентной командной палитрой **`⌘K`**:

| Модуль | Тема | Что можно протестировать |
| :--- | :--- | :--- |
| **01** | **Архитектура островов и RSC** | Сравнение монолитного SPA и RSC + Islands; включайте гидратацию отдельных островов и наблюдайте за LCP, INP, размером JS-бандла и флеймграфом главного потока. |
| **02** | **Граничные вычисления (Edge KV)** | Запросы из Берлина, Токио и Сан-Паулу: сравнение Edge Workers + KV (`5–8 мс`) с запросами к единой БД Origin (`148–214 мс`). |
| **03** | **Нативные возможности браузера** | Интерактивный слайдер CSS `@container`, галерея View Transitions API и бенчмарк физики частиц Wasm SIMD против однопоточного JS. |
| **04** | **Офлайн-PWA и Web Push** | Режим полёта и закрытая вкладка с фоновым пробуждением `sw.js` и расшифровкой уведомлений VAPID `p256dh`/`auth`. |
| **05** | **Сквозная типизация TypeScript** | Переключение типа поля `price` (`number` / `string`) и мгновенное распространение вывода типов или ошибок компиляции по цепочке Схема БД → Server RPC → React Props. |
| **06** | **Real-Time транспорт и Zero-Trust крипто** | 4-полосная трасса пакетов **WebRTC (UDP/SRTP)**, **WebTransport (QUIC)** и **WebSockets (TCP)** с потерей 15% пакетов; симулятор защиты **FIDO2 Passkeys** от фишинга; живая подпись `window.crypto.subtle` (`ES256`, `HMAC-SHA256`, `DPoP`) и тест подмены. |
| **07** | **Фронтир браузера конца 2026** | **WebMCP** (`navigator.modelContext`) против DOM-скрейпинга; **Local-First OPFS SQLite + CRDT** синхронизация двух устройств; **CSS Anchor Positioning + `contrast-color()`**; замер локального ИИ на **WebGPU / WebNN**. |

### 2. [Симулятор Web Push и VAPID](https://vedariy.github.io/modern-stack/webpush-simulator.html) (`webpush-simulator.html`)
Пошаговый визуальный симулятор работы Web Push: регистрация Service Worker (`sw.js`), получение `PushSubscription` (`endpoint`, `p256dh`, `auth`), подпись VAPID JWT, сквозное E2E-шифрование и доставка системного уведомления при закрытой вкладке браузера.

---

## Структура репозитория

```text
Vedariy/modern-stack/
├── index.html                  # Двуязычный хаб-лендинг (EN/RU) с палитрой ⌘K
├── modern-stack-2026.html      # Флагманский симулятор веб-архитектуры (7 модулей)
├── webpush-simulator.html      # Симулятор Web Push и VAPID
├── README.md                   # Документация на английском
└── README.ru.md                # Документация на русском
```

### Планы развития (Roadmap)
- **Модуль 08 (`zero-latency-identity.html`):** Speculation Rules (пререндеринг MPA за 0 мс), Trusted Types (защита от DOM XSS), W3C Digital Credentials и SD-JWT.
- **Модуль 09 (`hardware-spatial-web.html`):** WebHID/WebSerial/WebBluetooth, WebXR Spatial Computing, WebCodecs + AudioWorklet DSP и HDR `oklch()`.

---

## Локальный запуск

Все симуляторы выполнены в виде автономных HTML-файлов и используют нативные API браузера (включая Web Crypto), поэтому запускайте папку через локальный HTTP-сервер:

```bash
git clone https://github.com/Vedariy/modern-stack.git
cd modern-stack
python3 -m http.server 8000
```

После запуска откройте [http://localhost:8000](http://localhost:8000) в браузере.