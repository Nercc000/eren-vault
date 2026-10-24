---
stand: "2026-10-24"
tags: ["zentrale", "server"]
status: "live"
---

# Zentrale

- **https://zentrale.celikmedia.de**: Erens Übersicht für Handy und PC, auch als App auf dem iPhone mit Push-Mitteilungen. Anmeldung über Cloudflare Access mit Code per Mail.
- Technik: Next.js 15, React 19, SQLite. Läuft auf dem Server unter `/srv/zentrale` (Port 3200).
- Seiten: Heute, Aufgaben, Mail, Notizen, Plan, Drehtag, RehSell, TikTok, Wirlo, Geld, System, Mehr.

## Quellen (Stand 24.10.2026)
| Quelle | Status |
|---|---|
| Mail (eren@celikmedia.de), Gmail | verbunden, Abgleich alle 5 Minuten. Jev sortiert über OpenRouter. |
| Aufgaben, System | verbunden |
| RehSell | verbunden, nur lesend |
| TikTok | über [[Flutlicht]], stündlicher Abruf |
| Geld | Bankabgleich 3× täglich, nur lesend ([[Konten und Geld]]) |
| Kalender, Wrilo (Seite heißt „Wirlo“) | nicht verbunden |

## Regeln
- Jeder Bot darf nur seine eigene Quelle beschreiben (Email Manager → Mail, RehSell → RehSell, Wirlo → Wrilo, TikTok → TikTok, Chef → Aufgaben/System).
- Bot-Schnittstellen sind nur innerhalb des Servers erreichbar, nie über den Tunnel.
- Mail-Entwürfe schreibt der Email Manager. Gesendet wird nichts ohne Freigabe.
