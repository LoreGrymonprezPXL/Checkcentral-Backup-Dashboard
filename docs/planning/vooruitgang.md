# 🛡️ CheckCentral Back-up Automatisering Tracker

![Voortgang](https://geps.dev/progress/28) 

**Legende:**
- 🟢 **Actief in CheckCentral** (Volledig gekoppeld via API of unieke e-mailalias)
- 🟡 **Klaar voor kloon/template** (Regels bekend uit PoC: BackupAssist & AvePoint)
- 🔴 **Nog te analyseren / koppelen** (Voorbeeldmail nodig of manuele check)

---

### 📈 Voortgang per Softwarepakket
| Software | Methode | Status | Voortgang (Klantgroepen) |
| :--- | :--- | :--- | :--- |
| **N-able Cove** | Direct Integration (API) | 🟢 93% | 13 / 14 groepen actief (32 checks) |
| **LIPA (Intern)** | E-mail / API (PoC) | 🟢 100% | 8 / 8 taken actief |
| **BackupAssist** | E-mail (Kloonbaar) | 🟡 7% | 1 / 14 groepen actief |
| **AvePoint (M365)** | E-mail (Kloonbaar) | 🟡 9% | 1 / 11 groepen actief |
| **Synology** | E-mail | 🔴 0% | 0 / 7 groepen actief |
| **Iperius** | E-mail | 🔴 0% | 0 / 4 groepen actief |
| **Veeam** | E-mail | 🔴 0% | 0 / 3 groepen actief |
| **Acronis** | E-mail / API | 🔴 0% | 0 / 1 groep actief |

---

### 📋 Detailoverzicht per Klant (Geanonimiseerd)

#### 1. Klant BO
- [x] 🟢 **N-able** — `BO-RDS + BO-APP + BO-MGMT + BO-DC + BO-QLIK + BO-ORGANI` (6 - Cloud - API)
- [ ] 🟡 **Backup Assist** — `BO-RDS + BO-APP + BO-MGMT + BO-DC` (4 - NAS)
- [ ] 🔴 **Iperius** — `BO-RDS file backup + BO-NGINX VM backup` (2 - NAS)

#### 2. Klant CA
- [x] 🟢 **N-able** — `CA-SRV01 (Files + System State)` (2 - Cloud - API)
- [ ] 🟡 **Backup Assist** — `CA-SRV01 (System Protection)` (1 - CA-NAS01)
- [ ] 🟡 **AvePoint** — `M365 (Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams)` (7 - Cloud)
- [ ] 🔴 **Synology Hyper Backup** — `Network Backup NAS2NAS (CA-NAS01 to CA-NAS02)` (1 - NAS)

#### 3. Klant ETN
- [x] 🟢 **N-able** — `ETN-SRV02 (Data)` (Cloud - API)
- [x] 🟢 **N-able** — `ETN-SRV01 (Data)` (Cloud - API)
- [ ] 🟡 **Backup Assist** — `ETN-SRV02 (Archive backup - Enkel op vrijdag)` (1 - USB)
- [ ] 🔴 **Xcopy** — `ETN-SRV01 (Differential)` (1)

#### 4. Klant MGW
- [ ] 🟡 **Backup Assist** — `MGW-SRV01 (File protection)` (1 - NAS)
- [ ] 🟡 **Backup Assist** — `MGW-SRV01 (System Protection)` (1 - NAS)
- [ ] 🔴 **Synology** — `MGW-NAS01` (1 - NAS2NAS)

#### 5. Klant GGL
- [x] 🟢 **N-able** — `GGL-SRV11 + GGL-SRV14 (Files + System State)` (6 - Cloud - API, *let op: SRV11 nog nakijken in Cove*)
- [ ] 🟡 **Backup Assist** — `GGL-SRV14 + GGL-SRV11 (SQL)` (4 - GGL-NAS02)
- [ ] 🟡 **AvePoint** — `M365 (Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams)` (7 - Cloud)
- [ ] 🔴 **Synology** — `GGL-NAS02 to GGL-NAS01` (1 - Externe NAS)
- [ ] 🔴 **Veeam** — `GGL-SRV11 t/m GGL-SRV16` (1 - GGL-NAS02)

#### 6. Klant HVE
- [x] 🟢 **N-able** — `HVE-SRV11 (Files + System State)` (4 - Cloud - API)
- [x] 🟢 **N-able** — `HVE-SRV12 (Files + System State + MSQL)` (4 - Cloud - API)
- [ ] 🟡 **AvePoint** — `M365 (Exchange, OneDrive)` (2 - Cloud)
- [ ] 🔴 **Iperius** — `HVE-SRV11 + SRV12` (4 - NAS)

#### 7. Klant JM
- [x] 🟢 **N-able** — `JM-SRV11 + 12 + 13 + 14 (Files + System State)` (8 - Cloud - API)
- [ ] 🟡 **Backup Assist** — `JM-SRV11 (File + System protection)` (1 - JM-NAS01)
- [ ] 🟡 **Backup Assist** — `JM-SRV11 + 12 + 13 + 14 (System protection)` (4 - NAS)
- [ ] 🟡 **Backup Assist** — `JM-SRV12 + 13 (SQL)` (2 - SQL)

#### 8. Klant JAM
- [ ] 🟡 **Backup Assist** — `JAM-SRV01 (System Protect)` (1 - NAS)
- [ ] 🟡 **Backup Assist** — `JAM-SRV01 (File protection)` (1 - USB)

#### 9. Klant KW
- [ ] 🟡 **Backup Assist** — `Daily Backup Local NAS & Remote NAS (KW-SRV02 + 03)` (4 - NAS)
- [ ] 🔴 **Veeam** — `KW-SRV01 + 02 + 03 + 04 + 05` (1 - NAS)

#### 10. Klant LP
- [ ] 🟡 **AvePoint** — `M365` (2 - Cloud)
- [ ] 🔴 **Iperius** — `LP-LT17 (Manuele backup)` (1 - USB)

#### 11. Intern LIPA (PoC Voltooid)
- [x] 🟢 **Backup Assist** — `LIPA-SRV02 (SYSTEM PROTECT)` (1 - USB DISK)
- [x] 🟢 **Backup Assist** — `LIPA-SRV02 (Full Backup)` (1 - NAS)
- [x] 🟢 **Powershell robocopy** — `L
