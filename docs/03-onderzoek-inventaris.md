# 3. Onderzoek & inventaris (beginsituatie)

## 3.1 Doel
Exact weten wat Lipa ICT back-upt, met welke software en hoeveel meldingen daaruit volgen, vóór CheckCentral wordt ingericht.

## 3.2 Methode
Inventarisatie (Excel-overzicht van Lipa ICT), observatie van de huidige opvolging, literatuurstudie (CheckCentral-documentatie).

## 3.3 Resultaat in cijfers
| Kerncijfer | Waarde |
|---|---|
| Klanten (incl. intern Lipa) | 22 |
| Inventarisregels (jobs) | 71 |
| Softwaretypes | 12 |
| Checks ondergrens (1 per regel) | 71 |
| Checks bovengrens (som 'Aantal') | 168 |
| Regels met onbekend aantal | 5 |

De echte aantallen hangen af van het mailgedrag per software (1 mail per job, per server of per tenant). Dat is onderdeel van de mailanalyse.

## 3.4 Per software
| Software | Regels | Klanten | Checks min–max | Wave |
|---|---|---|---|---|
| Backup Assist | 20 | 13 | 20–35 | 2 |
| N-able Cove | 18 | 14 | 18–57 | 1 |
| Avepoint | 11 | 11 | 11–50 | 2 |
| Synology | 6 | 6 | 6–6 | 2 |
| Iperius | 4 | 4 | 4–8 | 2 |
| Acronis | 4 | 1 | 4–4 | 2 |
| Veeam | 3 | 3 | 3–3 | 2 |
| Nakivo | 1 | 1 | 1–1 | 2 |
| Xcopy, PowerShell/Robocopy, Proxmox, BackupNet2Access | 4 | 4 | 4–4 | later |

Geanonimiseerde gegevens: [`data/backup-inventaris.csv`](../data/backup-inventaris.csv). Het volledige Excel-overzicht met echte klantnamen blijft **lokaal** (niet in deze publieke repo).

## 3.5 Bevindingen
- CheckCentral biedt directe integraties voor o.a. **Cove Data Protection** en **Acronis** (zie site, Direct Integrations). Voor Wave 1 is dus mogelijk geen mailparsing nodig.
- Vier softwaretypes sturen mogelijk geen standaardmail; zonder scripts zijn ze mogelijk niet te monitoren.
- Eén job loopt enkel op vrijdag: aangepast tijdvenster voor de dead man's switch.

## 3.6 Open vragen
Zie tabblad *Open vragen* in het Excel-overzicht en de vragenlijst voor de demo.
