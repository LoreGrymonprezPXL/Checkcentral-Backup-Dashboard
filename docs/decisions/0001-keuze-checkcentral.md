# ADR-0001: Keuze voor CheckCentral als SaaS back-updashboard

- **Datum:** [YYYY-MM-DD]
- **Status:** Aanvaard
- **Beslissers:** [student], Edwin Vanspauwen

## Context
Handmatige Excel-opvolging van ~125 jobs is foutgevoelig. Vereist: laagdrempelig, geen programmeerkennis, dead man's switch.

## Opties
1. Excel blijven gebruiken — geen automatisering.
2. Zelfbouw (scripts/database/server) — buiten scope, onderhoudslast.
3. CheckCentral (SaaS) — mailparsing + dead man's switch, 0,50 USD/check/maand.
4. [Ander alternatief na marktverkenning]

## Beslissing
CheckCentral, evaluatie via 60 dagen proef.

## Gevolgen
+ Snelle uitrol, weinig onderhoud · − Terugkerende kost, externe verwerking (GDPR).
