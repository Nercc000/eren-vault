---
stand: "2026-10-24"
tags: ["server"]
---

# Server und Dienste

- Ein Linux-Server, rund um die Uhr an. Darauf laufen OpenMausBot (die Bots), die Zentrale, rehsell.de und die ReSell-Plattform.
- **OpenMausBot** ist vom Handy und vom PC aus erreichbar und startet nach einem Absturz von selbst neu. Anhänge dürfen höchstens 512 MB belegen.
- Erens eigener SSH-Schlüssel ist nur beim Admin-Konto hinterlegt.

| Dienst | Ort | Adresse |
|---|---|---|
| Zentrale | `/srv/zentrale` | zentrale.celikmedia.de |
| RehSell-Landingpage | `/srv/rehsell` (Dienst `rehsell-web`) | rehsell.de, www.rehsell.de |
| ReSell-Plattform | `/opt/resell` (Docker) | intern |
| TikTok-Vault | `/home/maus/tiktok-vault` | GitHub tiktok-vault |
| Dieser Vault | `/home/maus/eren-vault` | GitHub eren-vault |

## Automationen (Serverzeit UTC)
| Wann | Was |
|---|---|
| alle 5 Min. | Mail-Abgleich, Drehtag-Abgleich |
| stündlich :07 | Flutlicht-Abruf |
| 07:05 / 13:05 / 19:05 UTC | Bankabgleich (nur lesend) |
| 05:20 UTC (07:20 Berlin) | TikTok-Vault-Update |
| 05:40 UTC (07:40 Berlin) | Update dieses Vaults |

## Domains
- celikmedia.de und rehsell.de liegen bei Cloudflare. Den DNS stellt Eren selbst um.
