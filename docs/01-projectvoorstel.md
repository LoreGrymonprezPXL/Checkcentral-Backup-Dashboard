---
status: concept
aangemaakt: 2026-10-28
gepland_start: TODO
gepland_einde: TODO
---

# 1. Projectvoorstel

> Weging: 5%. Bij **NO GO** → herwerking binnen 1 week. Een onvoldoende = geen deelname.

## 1.1 Context
Lipa ICT beheert ca. **125 actieve back-upjobs** verspreid over **15+ systemen/leveranciers**. Meldingen komen per e-mail binnen en worden handmatig bijgehouden in een Excel-overzicht.

## 1.2 Probleemstelling
- Handmatige opvolging is tijdrovend en foutgevoelig.
- Ontbrekende meldingen (job draaide niet) vallen pas laat of niet op.
- Excel is moeilijk onderhoudbaar en geeft geen realtime overzicht.

## 1.3 Doelstelling
Een gecentraliseerd, geautomatiseerd dashboard waarop support in één oogopslag de status van alle back-ups ziet, onderhoudbaar zonder programmeerkennis.

## 1.4 Onderzoeksvraag
*Hoe kan Lipa ICT met CheckCentral de opvolging van back-upmeldingen centraliseren en automatiseren, zodat fouten en ontbrekende meldingen betrouwbaar gedetecteerd worden?*

Deelvragen:
1. Welke leveranciers/mailformaten komen voor en hoe parsen we ze?
2. Hoe configureren we dead man's switches per job?
3. Voldoet externe verwerking van meldingen aan GDPR/interne richtlijnen?
4. Wat zijn de kosten ten opzichte van de huidige werkwijze?
5. Is de oplossing onderhoudbaar voor non-developers?

## 1.5 Scope
**In scope:** implementatie voor ~130 checks · parsing & matching rules · dead man's switch · documentatie & overdracht · GDPR-toetsing.
**Out of scope:** eigen software/webapps · SQL-databases/extra servers · zware maatwerkscripts (Python/Office) — enkel ingebouwde CheckCentral-parsing.

## 1.6 Stakeholders
| Rol | Persoon | Belang |
|---|---|---|
| Werkplekcoach / opdrachtgever | Edwin Vanspauwen | Werkende, onderhoudbare oplossing |
| PXL-coach | Klaas Thys | Academische kwaliteit |
| Eindgebruikers | Support engineers Lipa ICT | Dagelijks gebruik |

## 1.7 Kosten
0,50 USD/check/maand × ~130 = **±65 USD/maand** excl. btw, na 60 dagen gratis proef. Zie `10-kostenanalyse.md`.

## 1.8 Risico's (kort)
Zie risicoregister in `02-plan-van-aanpak.md`.

## 1.9 Feedback & status
| Datum | Feedback coach | Status (GO/NO GO) |
|---|---|---|
| | | |
