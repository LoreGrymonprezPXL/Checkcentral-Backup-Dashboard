# CheckCentral graduaatsproef: overzicht back-ups

Kleuren en lettertypes: zie [BRANDING.md](BRANDING.md).

> Aanpassen? Wijzig gewoon het getal achter de dubbele punt. GitHub tekent de grafiek automatisch opnieuw.

## 1. Aantal checks per back-upsoftware

Klanten onder betaald back-upcontract, met de hand geteld (totaal: 140).

```mermaid
%%{init: {"theme":"base","themeVariables":{"fontFamily":"Open Sans, Arial, sans-serif","pieTitleTextColor":"#4D4D4D","pieSectionTextColor":"#333333","pieLegendTextColor":"#4D4D4D","pieStrokeColor":"#FFFFFF","pie1":"#52C3F1","pie2":"#838383","pie3":"#EA640A","pie4":"#A185A4","pie5":"#25A0A8","pie6":"#92B63D","pie7":"#A8E1F8","pie8":"#C1C1C1","pie9":"#F4B184","pie10":"#D0C2D1","pie11":"#92CFD3","pie12":"#C8DA9E","pie13":"#4D4D4D"}}}%%
pie showData
    title Checks per back-upsoftware (totaal 140)
    "N-able" : 60
    "Backup Assist" : 33
    "Veeam" : 12
    "Avepoint" : 11
    "Iperius" : 8
    "Synology" : 5
    "Acronis" : 4
    "Nakivo" : 2
    "Synology Hyper Backup" : 1
    "BackupNet2Access" : 1
    "Powershell" : 1
    "Proxmox" : 1
    "Xcopy" : 1
```

## 2. Fasering: eerst de makkelijke checks

Logica: begin met de grootste groepen met één uniform mailformaat. Zo is er snel veel gedekt. Eindig met de uitzonderingen die mogelijk geen standaardmail sturen.

| Fase | Software | Checks | Waarom |
| --- | --- | --- | --- |
| 1 | N-able, Avepoint | 71 | Groot volume, uniform mailformaat. Eén rule dekt veel checks |
| 2 | Backup Assist, Veeam, Iperius, Acronis | 57 | Vaste mailstructuur, maar meer variatie per klant |
| 3 | Synology, Nakivo, Hyper Backup, BackupNet2Access, Powershell, Proxmox, Xcopy | 12 | Weinig checks per systeem en mogelijk geen standaardmail. Hier is het meeste testwerk |

```mermaid
%%{init: {"theme":"base","themeVariables":{"fontFamily":"Open Sans, Arial, sans-serif","pieTitleTextColor":"#4D4D4D","pieSectionTextColor":"#333333","pieLegendTextColor":"#4D4D4D","pieStrokeColor":"#FFFFFF","pie1":"#92B63D","pie2":"#52C3F1","pie3":"#EA640A"}}}%%
pie showData
    title Checks per fase (totaal 140)
    "Fase 1: N-able + Avepoint" : 71
    "Fase 2: Backup Assist + Veeam + Iperius + Acronis" : 57
    "Fase 3: overige systemen" : 12
```

## 3. Prijs op CheckCentral

| Scenario | Checks | Per maand | Per maand bij jaarbetaling (-10%) |
| --- | --- | --- | --- |
| Huidig aantal | 140 | 70 USD | 63 USD |
| Met buffer | 280 | 140 USD | 126 USD |

- Standaardcheck: 0,50 USD per check per maand.
- Kwantumkorting begint pas vanaf 400 checks, dus geen korting in beide scenario's.
- Betalingskorting: 5% bij kwartaalbetaling, 10% bij jaarbetaling.
- Prijzen exclusief btw.
