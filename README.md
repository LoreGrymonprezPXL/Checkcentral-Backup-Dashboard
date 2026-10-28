# CheckCentral — Centraal back-updashboard bij Lipa ICT

> Graduaatsproef Systeem- en Netwerkbeheer · Hogeschool PXL

| | |
|---|---|
| **Student** | [Voornaam Naam] |
| **Opleiding** | Graduaat Systeem- en Netwerkbeheer (SNE), Hogeschool PXL |
| **Bedrijf** | Lipa ICT |
| **Werkplekcoach** | Edwin Vanspauwen |
| **PXL-coach** | Klaas Thys (of toegewezen coach) |
| **Academiejaar** | 2026–2027 |

## Samenvatting (STAR)

**Situatie** – Lipa ICT ontvangt dagelijks back-upmeldingen van ca. 125 actieve back-upjobs over meer dan 15 systemen/leveranciers. De opvolging gebeurde handmatig via een Excel-overzicht.

**Taak** – Een betrouwbare, geautomatiseerde oplossing opzetten die laagdrempelig en onderhoudbaar is voor collega-systeembeheerders zonder programmeerkennis.

**Actie** – [CheckCentral](https://www.checkcentral.cc) evalueren tijdens een proefperiode van 60 dagen, ca. 126 matching rules per leverancier/klant uitschrijven, dead man's switches configureren (bv. nachtvenster 01:00–06:00), alle scenario's testen (Success, Warning, Error, Missing) en overdragen aan support met handleiding.

**Resultaat** – Eén dashboard waarop support in één oogopslag de status van alle back-ups ziet; minder fouten, structurele tijdwinst.

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
│   ├── 09-gdpr-analyse.md
│   ├── 10-kostenanalyse.md
│   ├── decisions/        # Architecture/Decision Records (ADR's)
│   ├── logboek/          # Weeklogs + urenoverzicht
│   └── bronnen/          # Bronnenlijst (APA)
├── data/                 # Geanonimiseerde inventaris + rules-overzicht
├── templates/            # Sjablonen voor rule, testcase, weeklog
├── rapport/              # Eindrapport (deadline 17 jan 2027)
├── presentatie/          # Slides + demoscript (15 min + 10 min Q&A)
└── .github/              # Issue templates
```

## Planning & deadlines

| Deliverable | Gewicht | Deadline |
|---|---|---|
| Projectvoorstel | 5% | Week 1–3 |
| Plan van aanpak | 5% | **1 nov 2026** |
| Gerealiseerd resultaat | 50% | Week 11–13 |
| Rapport | 20% | **zondag 17 jan 2027** |
| Juryverdediging | 20% | Na rapport |

## Werkafspraken

- **Commits**: [Conventional Commits](https://www.conventionalcommits.org/) in het Nederlands, bv. `docs: voeg matching rules Veeam toe`, `test: voeg scenario Missing toe`.
- **Beslissingen** worden gelogd in `docs/decisions/` (ADR-formaat).
- **Weeklog** wekelijks in `docs/logboek/`; uren ook in **OnStage** ("Graduaatsproef", max. 4u/week op de werkplek).
- **Branches**: `main` = stabiel/inleverbaar, `fase/<nummer>-<naam>` voor werk per fase, merge via PR.
- **Issues/Milestones** per fase (zie `docs/02-plan-van-aanpak.md`).

## ⚠️ Privacy

Deze repo mag **geen echte klantgegevens, hostnamen, IP's, wachtwoorden of API-keys** bevatten. Gebruik pseudoniemen (`Klant-A`, `SRV-01`) en geanonimiseerde screenshots. Zie `docs/09-gdpr-analyse.md` en `.gitignore`.

## Status

- [ ] Projectvoorstel ingediend / GO
- [ ] Plan van aanpak ingediend
- [ ] Inventaris compleet
- [ ] Matching rules opgesteld
- [ ] Dead man's switches actief
- [ ] Tests uitgevoerd
- [ ] Handleiding + overdracht
- [ ] Rapport ingediend
- [ ] Presentatie klaar
