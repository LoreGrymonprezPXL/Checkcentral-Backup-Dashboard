# ADR-0004: Gefaseerde uitrol in waves

- **Datum:** 2026-10-29
- **Status:** Aanvaard

## Context
De inventaris telt 71 regels (22 klanten, 12 softwaretypes). N-able Cove vormt het grootste aandeel (18 regels, tot 57 checks).

## Beslissing
- **Wave 1:** N-able Cove.
- **Wave 2:** overige leveranciers (Backup Assist, Avepoint, Synology, Iperius, Acronis, Veeam, Nakivo).
- **Later/te bepalen:** Xcopy, PowerShell/Robocopy, Proxmox, BackupNet2Access (mogelijk geen standaardmail; scripts zijn out-of-scope).

## Gevolgen
Eerst het grootste volume valideren; lessen uit Wave 1 gebruiken in Wave 2.
