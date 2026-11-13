# CheckCentral Back-up Automatisering Tracker

![Voortgang](https://geps.dev/progress/48)

**Legende:**
- `[x]` **Actief in CheckCentral** — Volledig gekoppeld via API of unieke e-mailalias
- `[~]` **Klaar voor koppeling / template** — Regels en profielen zijn klaar (AvePoint & BackupAssist)
- `[ ]` **Nog te analyseren / koppelen** — Voorbeeldmail nodig of manuele configuratie

---

### Voortgang per Softwarepakket

| Software | Methode | Status | Voortgang (Klantgroepen / Checks) |
| :--- | :--- | :--- | :--- |
| **N-able Cove** | Direct Integration (API) | Actief (100%) | 15 / 15 groepen actief (32 checks) |
| **LIPA (Intern)** | E-mail / API (PoC) | Actief (100%) | 8 / 8 checks actief |
| **AvePoint (M365)** | E-mail (Notificatieprofiel klaar) | In uitrol (64%) | 7 / 11 groepen actief in CC (4 enkel nog linken) |
| **BackupAssist** | E-mail (Template klaar) | In uitrol (14%) | 2 / 14 groepen actief (6 checks live) |
| **Nakivo** | E-mail | In uitrol (50%) | 1 / 2 checks actief |
| **Proxmox & Scripts** | E-mail | In uitrol | 3 checks actief (DC-SRV002, Briljant, Net2Access) |
| **Synology** | E-mail | Te starten (0%) | 0 / 7 groepen actief |
| **Iperius** | E-mail | Te starten (0%) | 0 / 4 groepen actief |
| **Veeam** | E-mail | Te starten (0%) | 0 / 3 groepen actief |
| **Acronis** | E-mail / API | Te starten (0%) | 0 / 1 groep actief |

---

### Detailoverzicht per Klant (Geanonimiseerd)

#### 1. Klant BO (Bouwpunt Droogmans)
- [x] **N-able** — `BO-RDS + BO-APP + BO-MGMT + BO-DC + BO-QLIK + BO-ORGANI` (6 - Cloud - API)
- [x] **BackupAssist** — `BO-RDS + BO-APP + BO-MGMT + BO-DC` (4 - NAS)
- [ ] **Iperius** — `BO-RDS file backup + BO-NGINX VM backup` (2 - NAS)

#### 2. Klant CA (Calomat)
- [x] **N-able** — `CA-SRV01 / ca-plenion (Files + System State)` (2 - Cloud - API)
- [x] **AvePoint** — `M365 (Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams)` (Cloud)
- [ ] **BackupAssist** — `CA-SRV01 (System Protection)` (1 - CA-NAS01)
- [ ] **Synology Hyper Backup** — `Network Backup NAS2NAS (CA-NAS01 to CA-NAS02)` (1 - NAS)

#### 3. Klant ETN (ETN Banden Eric)
- [x] **N-able** — `ETN-SRV02 (Data)` (Cloud - API)
- [x] **N-able** — `ETN-SRV01 (Data)` (Cloud - API)
- [ ] **BackupAssist** — `ETN-SRV02 (Archive backup - Enkel op vrijdag)` (1 - USB)
- [ ] **Xcopy** — `ETN-SRV01 (Differential)` (1)

#### 4. Klant MGW
- [ ] **BackupAssist** — `MGW-SRV01 (File protection)` (1 - NAS)
- [ ] **BackupAssist** — `MGW-SRV01 (System Protection)` (1 - NAS)
- [ ] **Synology** — `MGW-NAS01` (1 - NAS2NAS)

#### 5. Klant GGL (Group GL / GL Hospitality)
- [x] **N-able** — `GGL-SRV11 + GGL-SRV14 (Files + System State)` (6 - Cloud - API)
- [ ] **AvePoint** — `M365 (Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams)` (Cloud - Enkel nog linken in CC)
- [ ] **BackupAssist** — `GGL-SRV14 + GGL-SRV11 (SQL)` (4 - GGL-NAS02)
- [ ] **Synology** — `GGL-NAS02 to GGL-NAS01` (1 - Externe NAS)
- [ ] **Veeam** — `GGL-SRV11 t/m GGL-SRV16` (1 - GGL-NAS02)

#### 6. Klant HVE (Huygen en Van Ende)
- [x] **N-able** — `HVE-SRV11 (Files + System State)` (4 - Cloud - API)
- [x] **N-able** — `HVE-SRV12 (Files + System State + MSQL)` (4 - Cloud - API)
- [x] **AvePoint** — `M365 (Exchange, OneDrive)` (Cloud)
- [ ] **Iperius** — `HVE-SRV11 + SRV12` (4 - NAS)

#### 7. Klant JM (Jacometal)
- [x] **N-able** — `JM-SRV11 + 12 + 13 + 14 (Files + System State)` (8 - Cloud - API)
- [ ] **BackupAssist** — `JM-SRV11 (File + System protection)` (1 - JM-NAS01)
- [ ] **BackupAssist** — `JM-SRV11 + 12 + 13 + 14 (System protection)` (4 - NAS)
- [ ] **BackupAssist** — `JM-SRV12 + 13 (SQL)` (2 - SQL)

#### 8. Klant JAM
- [ ] **BackupAssist** — `JAM-SRV01 (System Protect)` (1 - NAS)
- [ ] **BackupAssist** — `JAM-SRV01 (File protection)` (1 - USB)

#### 9. Klant KW
- [ ] **BackupAssist** — `Daily Backup Local NAS & Remote NAS (KW-SRV02 + 03)` (4 - NAS)
- [ ] **Veeam** — `KW-SRV01 + 02 + 03 + 04 + 05` (1 - NAS)

#### 10. Klant LP (LightPlus)
- [x] **AvePoint** — `M365` (Cloud)
- [ ] **Iperius** — `LP-LT17 (Manuele backup)` (1 - USB)

#### 11. Intern LIPA (PoC Voltooid)
- [x] **BackupAssist** — `LIPA-SRV02 (SYSTEM PROTECT eHDD)` (1 - USB DISK)
- [x] **BackupAssist** — `LIPA-SRV02 (Full Backup NAS)` (1 - NAS)
- [x] **PowerShell Robocopy** — `LIPA-SRV02 (Briljant)` (1 - Script)
- [x] **BackupNet2Access** — `LIPA-SRV02 (Net2 Access Control)` (1 - Script)
- [x] **Nakivo** — `VMware backup job` (1 - VM)
- [x] **Proxmox** — `DC-SRV002` (1 - Server)
- [x] **AvePoint** — `M365 (All)` (Cloud)
- [x] **N-able** — `lipa-server02` (Cloud - API)

#### Overige reeds actieve klanten (uit CheckCentral overzicht)
- [x] **Klant MGP (Metal Galva Plus)** — **N-able** (`dell-filiep + pluto + poseidon + zeus`)
- [x] **Klant RL (Revilax)** — **N-able** (`rl-srv02`) + **AvePoint** (`M365`)
- [x] **Klant SD (Shopping Diepenbeek)** — **AvePoint** (`M365`)
- [x] **Klant VOS (Vos N.V. / Vos Car Electronics)** — **N-able** (`vos-srv11 + vos-srv12`) + **AvePoint** (`M365`)
- [x] **Klant SHAM (Shamrock)** — **N-able** (`sham-srv01 + sham-srv03`)
- [x] **Klant VBB (VB Beton)** — **N-able** (`vbb-lt18 + vbb-srv11 + 12 + 13 + 14`)
- [x] **Klant SCH (Schoeffaerts)** — **N-able** (`schoeff-srv01`)
- [x] **Klant MR (Fintegriteit / Maes Richard)** — **N-able** (`mr-srv01`)
