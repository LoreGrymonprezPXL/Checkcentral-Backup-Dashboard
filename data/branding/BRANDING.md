# Huisstijl (Lipa ICT)

Bron: Lipa Brandbook, bewaard in `assets/LipaBrandBook.png`. De waarden hieronder zijn daaruit overgenomen. Bij twijfel geldt het brandbook.

## Kleuren

### Hoofdkleuren

| Naam | HEX | RGB | CMYK |
| --- | --- | --- | --- |
| Lipa Blauw | `#52C3F1` | 82, 195, 241 | 62, 0, 0, 0 |
| Lipa Grijs | `#838383` | 131, 131, 131 | 48, 38, 38, 19 |

### Secundaire kleuren

| Naam | HEX | RGB |
| --- | --- | --- |
| Oranje | `#EA640A` | 234, 100, 10 |
| Paars | `#A185A4` | 161, 133, 164 |
| Turquoise | `#25A0A8` | 37, 160, 168 |
| Groen | `#92B63D` | 146, 182, 61 |

### Afgeleide hulpkleuren (niet in het brandbook)

Deze heb ik zelf afgeleid voor leesbaarheid en grafieken. Ze zijn geen officiële Lipa-kleuren.

| Gebruik | HEX | Opmerking |
| --- | --- | --- |
| Tekst (donkergrijs) | `#4D4D4D` | Lipa Grijs op wit haalt ongeveer 3,9:1 contrast, onvoldoende voor lopende tekst. Lipa Blauw op wit haalt ongeveer 2,1:1. Gebruik beide dus voor titels, vlakken en grafieken, niet voor kleine tekst. |
| Tinten (50%) | `#A8E1F8` blauw, `#C1C1C1` grijs, `#F4B184` oranje, `#D0C2D1` paars, `#92CFD3` turquoise, `#C8DA9E` groen | Voor grafieken met meer dan zes categorieën |
| Foutstatus (rood) | `#D32F2F` | Het palet bevat geen rood. Gebruik dit enkel voor een mislukte back-up |

## Lettertypes

- **Muli Light** voor titels
- **Open Sans** voor lopende tekst

Beide zijn gratis bij Google Fonts. Fallback: Arial of Calibri.

## Statuskleuren in het dashboard

| Status | Kleur |
| --- | --- |
| Geslaagd | Groen `#92B63D` |
| Waarschuwing | Oranje `#EA640A` |
| Mislukt | Rood `#D32F2F` (hulpkleur) |
| Ontbrekend | Paars `#A185A4` |
| Neutraal / geen data | Lipa Grijs `#838383` |

Gebruik naast kleur ook altijd een label of icoon, zodat de status ook leesbaar is voor kleurenblinden.

## Mermaid-thema voor GitHub

Plak dit bovenaan elk Mermaid-pie-diagram:

```
%%{init: {"theme":"base","themeVariables":{"fontFamily":"Open Sans, Arial, sans-serif","pieTitleTextColor":"#4D4D4D","pieSectionTextColor":"#333333","pieLegendTextColor":"#4D4D4D","pieStrokeColor":"#FFFFFF","pie1":"#52C3F1","pie2":"#838383","pie3":"#EA640A","pie4":"#A185A4","pie5":"#25A0A8","pie6":"#92B63D","pie7":"#A8E1F8","pie8":"#C1C1C1","pie9":"#F4B184","pie10":"#D0C2D1","pie11":"#92CFD3","pie12":"#C8DA9E","pie13":"#4D4D4D"}}}%%
```

De kleuren volgen de volgorde van de data: de eerste regel krijgt `pie1`, de tweede `pie2`, enzovoort.

## Waar pas je dit toe

| Onderdeel | Toepassing |
| --- | --- |
| Projectvoorstel en eindverslag | Houd de template van de school aan. Gebruik de kleuren enkel in eigen figuren en tabelkoppen. |
| Handleiding voor collega's | Titels in Muli Light en Lipa Blauw, tekst in Open Sans en `#4D4D4D`, waarschuwingen in oranje. |
| Presentatie voor de verdediging | Witte achtergrond, Lipa Blauw voor titels en accenten, Lipa Grijs voor ondersteunende tekst, oranje voor het belangrijkste punt per dia. |
| Diagrammen en grafieken in de repo | Mermaid-thema hierboven. |
| CheckCentral-dashboard | Controleer tijdens de proefperiode welke aanpassingen CheckCentral toelaat (logo, kleuren). Ga er niet van uit dat dit kan. |
| Projectlogo | De mascotte in `assets/CheckCentral_Mascot_Logo_Storyboard.png` gebruikt dezelfde kleuren. Gebruik die enkel als projectlogo, niet als het officiële CheckCentral-logo. |
