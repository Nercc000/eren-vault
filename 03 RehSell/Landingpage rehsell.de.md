---
stand: "2026-10-24"
tags: ["rehsell", "web"]
status: "live"
---

# Landingpage rehsell.de

- **Live seit 23.10.2026** mit dem neuen Design (PS5-Reparatur und Ankauf, WhatsApp-Ablauf).
- Technik: Next.js. Läuft auf dem Server als Dienst `rehsell-web` (`/srv/rehsell`, Port 3300), erreichbar über den Cloudflare-Tunnel „zentrale“. Den DNS-Eintrag hat Eren selbst umgestellt.
- Code: Repo `Nercc000/rehsell-landingpage`, Branch `brand-relaunch`. Chef 2 hat nur Lesezugriff und arbeitet in `/home/maus/repos/rehsell-landingpage`.
- Der alte Shop liegt weiter bei Vercel (mit Passwort) und dient als Rückfallweg.
- Seiten: Start, Reparatur, Ankauf, Über uns, Kontakt, AGB, Impressum, Datenschutz.

## Offen
- AGB: nicht juristisch geprüft. Vorläufig: Diagnose kostenlos, Versand zahlt der Kunde.
- Öffnungszeiten sind Platzhalter.
- Bilder sind KI-Platzhalter, echte Werkstattfotos fehlen.
- Kleinunternehmer-Hinweis (§ 19 UStG) fehlt, weil unbestätigt.
