---
stand: "2026-10-24"
tags: ["rehsell", "software"]
status: "live"
---

# ReSell-Plattform

- Eigene **Multi-Tenant-SaaS** für Reselling: Marktplatz-Scanner, Ankauf, Bestand, Reparatur, Verkauf, Benachrichtigungen.
- Technik: FastAPI, PostgreSQL 17, Redis/RQ, React + Vite, Docker Compose. KI-Entscheidungen über OpenRouter („Jev“).
- Marktplätze: Kleinanzeigen (eigener Adapter, Auto-Send an), eBay-Anbindung.
- Läuft produktiv auf dem Server unter `/opt/resell`, seit 25.09.2026 mit echten Daten.
- Repo `Nercc000/ReSell-Platform` (privat, Chef 2 nur lesend). Laut README sind die Phasen 0–13 abgeschlossen. Der Server ist neuer als GitHub (letzter Commit 07.10.2026).
- Die Zentrale liest Gewinn, Umsatz, Bestand und gebundenes Kapital **nur lesend** über `/api/v1/zentrale/summary`.
