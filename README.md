# Geautomatiseerde back-upmonitoring via CheckCentral bij Lipa ICT

> Graduaatsproef Systeem- en Netwerkbeheer - Hogeschool PXL

| | |
|---|---|
| **Student** | Lore Grymonprez |
| **Opleiding** | Graduaat Systeem- en Netwerkbeheer (SNE), Hogeschool PXL |
| **Bedrijf** | Lipa ICT |
| **Werkplekcoach** | Edwin Vanspauwen |
| **PXL-coach** | Klaas Thys |
| **Academiejaar** | 2026-2027 |
| **Titel** | CheckCentral-back-updashboard |

## Waar gaat dit over?

Bij Lipa ICT volgen we de back-ups van onze contractklanten op via een Excel-lijst. De meldingen komen binnen per mail en worden handmatig gecontroleerd. Het grootste risico is een mail die niet aankomt: als er geen melding is, valt niemand op dat een back-up niet draaide ("stille uitval"). In deze graduaatsproef zoek ik uit hoe CheckCentral dit kan oplossen met één duidelijk klantoverzicht voor support.

**Onderzoeksvraag:** hoe biedt CheckCentral support een duidelijk klantoverzicht voor back-upopvolging?

## Samenvatting (STAR)

**Situatie** - Voor 22 contractklanten lopen er circa 140 back-upchecks, verspreid over meer dan 12 systemen. De grootste zijn N-able Cove (60), BackupAssist (33), Veeam (12) en AvePoint (11). Daarnaast zijn er Iperius, Synology, Acronis en Nakivo. De opvolging gebeurt nu handmatig via Excel en de mailbox.

**Taak** - Ik zet een betrouwbare, geautomatiseerde oplossing op die laagdrempelig en onderhoudbaar is voor mijn collega's van support, zonder programmeerkennis. Het dashboard toont minimaal Success, Warning, Error en Uncategorized per klant, en meldt ook wanneer een verwachte mail ontbreekt (Missing).

**Actie** - Ik start met een gratis CheckCentral-account (Free tier) en een technische demo, en activeer daarna een Enterprise-proefperiode van 60 dagen. Ik stel een ontwerp op (naamgeving, mailflow, matching rules en tijdsvensters), bouw het gefaseerd uit per wave (eerst N-able Cove, daarna de overige back-ups) en test alle scenario's. Vanaf 21-12-2026 draai ik minstens twee weken parallel met de huidige controle. Daarna schrijf ik de handleiding, draag ik over aan support en maak ik een prijsadvies. Een Autotask-koppeling is optioneel en komt er enkel als er tijd overblijft.

**Resultaat** - Eén dashboard waarop support in één oogopslag de status van alle back-ups ziet, inclusief ontbrekende meldingen. Het resultaat is onderbouwd met een testrapport, een handleiding en een abonnementsvoorstel.

## Afbakening

- Enkel klanten met een contract (zie ADR 0005).
- Geen maatwerkscripts, enkel standaardfuncties van CheckCentral (ADR 0003).
- Gefaseerde uitrol in waves (ADR 0004).
- Eerst Free tier, dan Enterprise-proef (ADR 0006).
- Alleen support krijgt beheerdersrechten.

## Planning en deadlines

Alle datums in DD-MM-yyyy. De volledige Gantt staat in `docs/planning/`.

| Fase | Periode | Mijlpaal |
|---|---|---|
| 1. Probleemstelling, analyse en plan van aanpak | 21-09-2026 t/m 01-11-2026 | Projectvoorstel 11-10-2026, plan van aanpak 01-11-2026 |
| 2. Onderzoek en inventarisatie | 02-11-2026 t/m 15-11-2026 | Check-in 3 op 15-11-2026 |
| 3.1 Design | 16-11-2026 t/m 29-11-2026 | Ontwerpcheck en check-in 4 op 29-11-2026 |
| 3.2 Implementatie | 30-11-2026 t/m 20-12-2026 | Check-in 5 op 13-12-2026 |
| 3.3 Testen en schaduwdraaien | 14-12-2026 t/m 10-01-2027 | Parallel monitoren vanaf 21-12-2026, buffer 04-01-2027 t/m 10-01-2027 |
| 3.4 Documentatie, overdracht en prijsadvies | 14-12-2026 t/m 10-01-2027 | Gerealiseerd resultaat 10-01-2027 |
| 4 en 5. Rapporteren en reflecteren | 16-11-2026 t/m 17-01-2027 | Eindrapport 17-01-2027 |
| Presentatie en juryverdediging | 18-01-2027 t/m 31-01-2027 | Exacte datum via Blackboard (nog te bevestigen) |

| Deliverable | Gewicht | Deadline |
|---|---|---|
| Projectvoorstel | 5% | 11-10-2026 |
| Plan van aanpak | 5% | 01-11-2026 |
| Gerealiseerd resultaat | 50% | 10-01-2027 |
| Rapport | 20% | 17-01-2027 |
| Juryverdediging | 20% | Na het rapport |

## Repo-structuur

```
├── docs/
│   ├── 01-projectvoorstel.md
│   ├── 02-plan-van-aanpak.md
│   ├── 03-onderzoek-inventaris.md
│   ├── 04-ontwerp-matching-rules.md
│   ├── 05-realisatie.md
│   ├── 06-testrapport.md
│   ├── 07-handleiding-support.md
│   ├── 08-overdracht.md
│   ├── 09-kostenanalyse.md
│   ├── bijlagen/         # Plan van aanpak (docx + pdf)
│   ├── planning/         # Gantt (csv, json, pdf, svg) + mijlpalen
│   ├── decisions/        # Decision records (ADR's)
│   ├── logboek/          # Weeklogs + urenregistratie
│   └── bronnen/          # Bronnenlijst (APA)
├── data/                 # Geanonimiseerde inventaris + matching rules (csv)
├── assets/branding/      # Mascotte, Lipa brandbook, BRANDING.md
├── templates/            # Sjablonen voor rule, testcase en weeklog
├── rapport/              # Eindrapport (deadline 17-01-2027)
└── presentatie/          # Slides + demoscript (15 min + 10 min Q&A)
```

## Werkafspraken

- **Commits:** [Conventional Commits](https://www.conventionalcommits.org/) in het Nederlands, bv. `docs: voeg matching rules Veeam toe` of `test: voeg scenario Missing toe`.
- **Beslissingen** log ik in `docs/decisions/` (ADR-formaat, met datum).
- **Weeklog** schrijf ik wekelijks in `docs/logboek/`. Mijn uren registreer ik ook in OnStage ("Graduaatsproef", max. 4u/week op de werkplek).
- **Branches:** `main` is stabiel en inleverbaar, voor werk per fase gebruik ik `fase/<nummer>-<naam>` en merge ik via PR.
- **Issues en milestones** maak ik per fase aan (zie `docs/02-plan-van-aanpak.md`).
- **Datums** schrijf ik overal als DD-MM-yyyy.

## Privacy

Deze repo bevat **geen echte klantgegevens, hostnamen, IP's, wachtwoorden of API-keys**. Ik werk met pseudoniemen (`Klant-A`, `SRV-01`) en geanonimiseerde screenshots. Voor ik het conceptrapport laat nalezen, controleer ik zelf nog eens of alle klantnamen geanonimiseerd zijn.

## Status

- [x] Projectvoorstel ingediend en GO (11-10-2026)
- [ ] Plan van aanpak ingediend (01-11-2026)
- [ ] Inventaris compleet (15-11-2026)
- [ ] Ontwerp besproken met werkplekcoach (29-11-2026)
- [ ] Matching rules en tijdsvensters ingesteld
- [ ] N-able Cove gekoppeld (begin december 2026)
- [ ] Overige back-ups gekoppeld (voor de kerstvakantie)
- [ ] Parallel monitoren gestart (21-12-2026)
- [ ] Tests uitgevoerd, testrapport klaar (10-01-2027)
- [ ] Handleiding, overdracht en prijsadvies (10-01-2027)
- [ ] Rapport en reflectie ingediend (17-01-2027)
- [ ] Presentatie en demo klaar
