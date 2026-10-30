---
status: concept
aangemaakt: 2026-10-28
gepland_start: TODO
gepland_einde: TODO
---

# 7. Handleiding voor support engineers

> Doelgroep: systeembeheerders **zonder programmeerkennis**.

## 7.1 Dagelijkse opvolging
1. Open het dashboard.
2. Filter op **Error / Missing / Warning**.
3. Open de check → bekijk laatste mail & historiek.
4. Maak ticket / onderneem actie.
5. Bevestig/commentaar toevoegen in CheckCentral.

## 7.2 Statussen begrijpen
| Status | Betekenis | Wat doe ik? |
|---|---|---|

## 7.3 Een nieuwe back-upjob toevoegen
1. Verzamel: klant, systeem, jobnaam, verwacht tijdstip, voorbeeldmail.
2. Maak check aan volgens naamconventie.
3. Maak matching rule (afzender + onderwerp).
4. Stel parsing/status in.
5. Stel dead man's switch in.
6. Test met voorbeeldmail.
7. Voeg toe aan `data/` inventaris.

## 7.4 Een job aanpassen of verwijderen
…

## 7.5 Troubleshooting
| Symptoom | Mogelijke oorzaak | Oplossing |
|---|---|---|
| Mail komt niet aan als match | Onderwerp gewijzigd | Rule aanpassen |
| Onterechte Missing | Venster te krap / job verschoven | Venster aanpassen |
| Veel false positives | Tolerantie te laag | Bijstellen |

## 7.6 Contact & escalatie
…
