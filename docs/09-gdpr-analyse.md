---
status: concept
aangemaakt: 2026-10-28
gepland_start: TODO
gepland_einde: TODO
---

# 9. GDPR-toetsing

> Geen juridisch advies. Doel: een onderbouwde risicoanalyse, bevestigd door de verantwoordelijke binnen Lipa ICT.

## 9.1 Vraag
Mogen back-upmeldingen extern (SaaS, leverancier Binary Fortress, Canada) verwerkt worden?

## 9.2 Beoordeling
De GDPR is van toepassing op elke organisatie in de EU die persoonsgegevens verwerkt. Het risico is hier laag omdat back-upmeldingen vooral technische statusinformatie bevatten (jobnamen, servernamen, tijdstippen, foutcodes).

## 9.3 Aandachtspunten
| Gegeven in melding | Persoonsgegeven? | Maatregel |
|---|---|---|
| Klantnaam / servernaam | Zelden | Toegestaan, nodig voor het doel |
| Gebruikersnamen of e-mailadressen (bv. in Avepoint-rapporten) | Ja | Per leverancier controleren; indien mogelijk uitsluiten |
| Bestandsnamen/paden in foutmeldingen | Mogelijk | Controleren in mailanalyse |

Verder nakijken: verwerkersovereenkomst, locatie van verwerking, bewaartermijn (Free 1 maand, Enterprise 6 maanden historiek).

## 9.4 Conclusie
Risico laag. Bevestiging verantwoordelijke Lipa ICT: ____ · Datum: ____
