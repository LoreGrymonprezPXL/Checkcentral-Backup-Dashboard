# 🛡️ CheckCentral Back-up Automatisering Tracker

![Voortgang](https://geps.dev/progress/28) 

**Legende:**
- 🟢 **Actief in CheckCentral** (Volledig gekoppeld via API of unieke e-mailalias)
- 🟡 **Klaar voor kloon/template** (Regels bekend uit PoC: BackupAssist & AvePoint)
- 🔴 **Nog te analyseren / koppelen** (Voorbeeldmail nodig of manuele check)

---

### 📈 Voortgang per Softwarepakket
| Software | Methode | Status | Voortgang (Groepen/Taken) |
| :--- | :--- | :--- | :--- |
| **N-able Cove** | Direct Integration (API) | 🟢 93% | 13 / 14 klantgroepen actief (32 checks) |
| **Lipa Intern (Diverse)** | E-mail / PoC | 🟢 100% | 8 / 8 taken actief |
| **BackupAssist** | E-mail (Kloonbaar) | 🟡 6% | 1 / 14 klantgroepen actief |
| **AvePoint (M365)** | E-mail (Kloonbaar) | 🟡 9% | 1 / 11 klantgroepen actief |
| **Synology** | E-mail | 🔴 0% | 0 / 7 klantgroepen actief |
| **Iperius** | E-mail | 🔴 0% | 0 / 4 klantgroepen actief |
| **Veeam** | E-mail | 🔴 0% | 0 / 3 klantgroepen actief |
| **Acronis** | E-mail | 🔴 0% | 0 / 1 klantgroep actief |

---

### 📋 Detailoverzicht per Klant

#### 1. Bouwpunt Droogmans
- [x] 🟢 **N-able** — `bd-rds_nacao + bd-app_q8igr + bd-mgmt_6bv5k + bd-dc_40heu + BD-QLIK + BD-ORGANI` (Cloud - API)
- [ ] 🟡 **Backup Assist** — `BD-RDS + BD-APP + BD-MGMT + BD-DC` (4 - NAS)
- [ ] 🔴 **Iperius** — `BD-RDS file backup + BD-NGINX VM backup` (2 - NAS)

#### 2. Calomat
- [x] 🟢 **N-able** — `ca-plenion_uo80p (Files + System State)` (2 - Cloud - API)
- [ ] 🟡 **Backup Assist** — `CA-Plenion (System Protection)` (1 - CA-NAS01)
- [ ] 🟡 **AvePoint** — `M365 Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams` (7 - Cloud)
- [ ] 🔴 **Synology Hyper Backup** — `Network Backup NAS2NAS (CA-NAS01 to CA-DS213J)` (1 - CA-DS213J)

#### 3. ETN Eric Banden
- [x] 🟢 **N-able** — `ETN-SRV02 (Data)` (Cloud - API)
- [x] 🟢 **N-able** — `ETN-SRV01 (Data)` (Cloud - API)
- [ ] 🟡 **Backup Assist** — `ETN-SRV02 (Archive backup - Enkel op vrijdag)` (1 - USB)
- [ ] 🔴 **Xcopy** — `ETN-SRV01 (adsolut Differential)` (1)

#### 4. Garage Wouters
- [ ] 🟡 **Backup Assist** — `MGW-SRV01 (file protection)` (1 - NAS)
- [ ] 🟡 **Backup Assist** — `MGW-SRV01 (System Protection)` (1 - NAS)
- [ ] 🔴 **Synology** — `MGW-NAS01` (1 - NAS2NAS)

#### 5. GroupGL
- [x] 🟢 **N-able** — `GGL-SRV11 + GGL-SRV14 (Files + System State)` (6 - Cloud - API, *let op: enkel SRV14 zat in API-import, SRV11 nakijken*)
- [ ] 🟡 **Backup Assist** — `GGL-SRV14 + GGL-SRV11 (SQL)` (4 - GGL-NAS02)
- [ ] 🟡 **AvePoint** — `M365 Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams` (7 - Cloud)
- [ ] 🔴 **Synology** — `GGL-NAS02 to GGL-NAS01` (1 - GGL-NAS01 bij Lipa)
- [ ] 🔴 **Veeam** — `GGL-SRV11+GGL-SRV12+GGL-SRV13-GGL-SRV14-SERVER2-NTSERVER` (1 - GGL-NAS02)

#### 6. Huygen en van Ende
- [x] 🟢 **N-able** — `HVE-SRV11 (Files + System State)` (4 - Cloud - API)
- [x] 🟢 **N-able** — `HVE-SRV12 (Files + System State + MSQL)` (4 - Cloud - API)
- [ ] 🟡 **AvePoint** — `Exchange, OneDrive` (2 - Cloud)
- [ ] 🔴 **Iperius** — `HVE-SRV11 + SRV12` (4 - NAS)

#### 7. Jacometal
- [x] 🟢 **N-able** — `JM-SRV11 + 12 + 13 + 14 (Files + System State)` (8 - Cloud - API)
- [ ] 🟡 **Backup Assist** — `JM-SRV11 (File + System protection)` (1 - JM-NAS01)
- [ ] 🟡 **Backup Assist** — `JM-SRV11 + 12 + 13 + 14 (System protection)` (4 - NAS)
- [ ] 🟡 **Backup Assist** — `JM-SRV12 + 13 (SQL)` (2 - SQL)

#### 8. Jamart
- [ ] 🟡 **Backup Assist** — `JAMART-SRV01 (System Protect)` (1 - NAS)
- [ ] 🟡 **Backup Assist** — `JAMART-SRV01 (File protection)` (1 - USB)

#### 9. Kringwinkel
- [ ] 🟡 **Backup Assist** — `Daily Backup Local NAS & Remote NAS (KW-SRV02 + 03)` (4 - NAS)
- [ ] 🔴 **Veeam** — `KW-SRV01 + 02 + 03 + 04 + 05` (1 - NAS)

#### 10. Lightplus
- [ ] 🟡 **AvePoint** — `M365` (2 - Cloud)
- [ ] 🔴 **Iperius** — `LP-LT17 - Manuele backup` (1 - USB)

#### 11. Lipa Office (Intern - PoC Voltooid)
- [x] 🟢 **Backup Assist** — `Lipa-Server02 (SYSTEM PROTECT)` (1 - USB DISK)
- [x] 🟢 **Backup Assist** — `Lipa-Server02 (Full Backup)` (1 - NAS)
- [x] 🟢 **Powershell robocopy** — `Lipa-Server05 (briljant)` (1 - LIPA-SERVER02 Backups)
- [x] 🟢 **Nakivo** — `Lipa-Server01 & Lipa-Server05` (1 - Nakivo Server)
- [x] 🟢 **BackupNet2Access** — `LIPA-SERVER02` (1 - LIPA-SERVER02 Backups)
- [x] 🟢 **N-able** — `lipa-server02_5fsuv (Data)` (2 - Cloud - API)
- [x] 🟢 **Proxmox** — `DC-SRV002` (1 - NAS)
- [x] 🟢 **AvePoint** — `M365` (5 - Cloud)

#### 12. Maes Richard (Fintegriteit)
- [x] 🟢 **N-able** — `mr-srv01_fwvqt (Files + System State)` (2 - Cloud - API)
- [ ] 🟡 **AvePoint** — `M365` (5 - Cloud)

#### 13. Metal Galva Plus
- [x] 🟢 **N-able** — `Pluto, Poseidon, Zeus` (7 - Cloud - API)
- [x] 🟢 **N-able** — `DELL-Filiep` (2 - Cloud - API)
- [ ] 🟡 **AvePoint** — `M365` (Cloud)

#### 14. Movie One
- [ ] 🔴 **Synology** — `funcitynas Network backup` (1 - DC NAS Lipa)

#### 15. Notaris Jageneau
- [ ] 🟡 **Backup Assist** — `NJ-SRV01 (Data)` (1 - NAS1)
- [ ] 🟡 **Backup Assist** — `NJ-SRV01 (SQL)` (1 - SQL)
- [ ] 🔴 **Synology** — `NJ-SRV01 Backup naar remote NAS bij Lipa` (1 - NAS2NAS)
- [ ] 🔴 **Veeam** — `NJ-SRV02 to NJ-SRV01` (1 - Local)

#### 16. Revilax
- [ ] 🔴 **N-able** — `rl-srv02_me3fg (Data)` (Cloud — *Let op: stond nog niet tussen de 32 API-checks!*)
- [ ] 🟡 **Backup Assist** — `RL-SRV02 Backup naar NAS` (1 - NAS)
- [ ] 🟡 **AvePoint** — `M365 Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams` (7 - Cloud)

#### 17. Schoeffaerts
- [x] 🟢 **N-able** — `schoeff-srv01_pspce` (2 - Cloud - API)
- [ ] 🟡 **AvePoint** — `M365 Groups, Public Folder, Project, Exchange, SharePoint, OneDrive, Teams` (7 - Cloud)

#### 18. Shamrock
- [x] 🟢 **N-able** — `SHAM-SRV01_evnxe (Data)` + `sham-srv03_u16i0` (2 - Cloud - API)
- [ ] 🟡 **Backup Assist** — `SHAM-SRV01 + SRV02 + SRV03 (System Protection)` (3 - NAS)
- [ ] 🟡 **Backup Assist** — `SHAM-SRV02` (1 - SHAM-SRV01)

#### 19. Shopping Diepenbeek
- [ ] 🟡 **AvePoint** — `M365` (2 - Cloud)

#### 20. VBBeton
- [x] 🟢 **N-able** — `VBB-SRV11 + 12 + 13 + 14` (9 - Cloud - API)
- [x] 🟢 **N-able** — `vbb-lt18_1s2ov` (1 - Cloud - API)
- [ ] 🔴 **Iperius** — `VBB-SRV11, 12, 13` (1 - NAS01)

#### 21. Vitalis huisartsen
- [ ] 🔴 **Synology** — `Acronis + Synology (Network backup)` (1 - NAS01 to NAS02)
- [ ] 🔴 **Acronis** — `PC-BUREEL` (1 - PCs2NAS)
- [ ] 🔴 **Acronis** — `VIT-LT04 (vroeger LAPTOP-PAUL)` (1 - PCs2NAS)
- [ ] 🔴 **Acronis** — `VIT-LT03 (vroeger LAPTOP-FRANK)` (1 - PCs2NAS)
- [ ] 🔴 **Acronis** — `PC-Wendy` (1 - PCs2NAS)

#### 22. VOS
- [x] 🟢 **N-able** — `vos-srv11 + 12` (2 - Cloud - API)
- [ ] 🟡 **Backup Assist** — `vos-srv11 + 12` (1 - NAS)
- [ ] 🟡 **AvePoint** — `M365 Groups, Exchange, SharePoint, OneDrive, Teams` (5 - Cloud)
