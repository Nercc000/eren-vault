---
stand: "2026-10-24"
tags: ["tiktok", "server"]
---

# Flutlicht

- **flutlicht.celikmedia.de**: Erens TikTok-Zentrale (React + Vite + Hono). Läuft auf seinem Windows-PC, Fernzugang über Cloudflare Pages und Tunnel, Verlauf in Cloudflare D1/KV.
- Repo `Nercc000/flutlicht` (privat).
- Die Zentrale liest stündlich (`/api/tiktok/status`, `/verlauf`), nur lesend.
- Der TikTok-Vault holt sich daraus jeden Morgen frische Zahlen.
