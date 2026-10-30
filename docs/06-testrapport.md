---
status: concept
aangemaakt: 2026-10-28
gepland_start: TODO
gepland_einde: TODO
---

# 6. Testrapport

## 6.1 Testdoelen
Valideren dat alle vier statussen correct gedetecteerd en gemeld worden.

## 6.2 Testscenario's
| ID | Scenario | Voorbereiding | Verwacht resultaat | Werkelijk resultaat | OK? |
|---|---|---|---|---|---|
| T01 | Success | Voorbeeldmail succes | Check = Success | | |
| T02 | Warning | Voorbeeldmail warning | Check = Warning + alert | | |
| T03 | Error | Voorbeeldmail failed | Check = Error + alert | | |
| T04 | Missing | Geen mail in venster 01:00–06:00 | Check = Missing + alert | | |
| T05 | Unmatched mail | Onbekend formaat | Landt in unmatched, geen foutieve match | | |
| T06 | Herstel | Success na Error | Status herstelt | | |
| T07 | Meerdere mails per run | Dubbele meldingen | Correcte eindstatus | | |

Template: [`templates/testcase.md`](../templates/testcase.md)

## 6.3 Gebruikersvalidatie
Feedback van support engineers (naam, datum, opmerkingen, aanpassingen).

## 6.4 Conclusie & bijsturing
…
