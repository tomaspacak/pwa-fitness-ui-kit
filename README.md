# My workout - fitness PWA aplikace
Tento projekt obsahuje návrh a podklady pro tvorbu **fitness aplikace**, která umožňuje uživatelům vytvářet vlastní tréninkové plány a sledovat jejich progress. Cílem bylo připravit podklady pro následnou realizaci jako **PWA (Progressive Web App)**.

## Obsah
- [Katalog cviků](#-katalog-cviků)
- [Design a uživatelské rozhraní](#-design-a-uživatelské-rozhraní)
- [Statická šablona](#-statická-šablona)

---

## Katalog cviků
Tato kapitola slouží jako průvodce katalogem cviků, který ma sloužit jako podklad pro vytvoření databáze cviků pro fitness aplikaci. Tabulka je rozdělena do několika sloupců, které obsahují potřebné informace o jednotlivých cvicích. Sloupce Kategorie I a Kategorie II by měly být implementovány jako atribut v databázovém modelu, aby uživatelé mohly snadno filtrovat cviky podle jejich preferencí. Níže je popsán účel a obsah každého sloupce:

| Sloupec               | Popis |
|-----------------------|-------|
| **Jméno cviku**       | Oficiální název cviku |
| **ID**                | Jedinečný identifikátor cviku v databázi |
| **Kategorie I**       | Rozdělení cviků na cviky s vlastní vahou a cviky s vybavením |
| **Kategorie II**      | Zaměření na svalovou skupinu (Nohy, Hrudník, Záda, Ramena, Břicho) |
| **Popis**             | Stručný popis cviku|
| **Náročnost**         | Obtížnost cviku (začátečník, středně pokročilý, pokročilý) |
| **Primární svaly**    | Hlavní svalové skupiny aktivované během cviku |
| **Sekundární svaly**  | Sekundární svalové skupiny, které cvik také zapojuje |
| **Jak na to**         | Podrobnější popis správného provedení cviku |

---

## Design a uživatelské rozhraní
**Barevná paleta**
 - Pozadí: #353535
 - Gradient: lineární rovnoměrně barvy #FE0000 s barvou #0381F5
 - Primární: #2A2A2A
 - Seknudární: #404040

**Ikony**: ve složce icons jsou uloženy veškeré potřebné ikony ve formátu SVG.

### Homepage
V dolní části se nachází menu, přes které se lze dostat do tří základních částí aplikace - přehled vytvořených plánů (homepage), sestavení nového tréninkového plánu a moje data.
Na homepage je zobrazen přehled všech vytvořených plánů uživatelem (v případě, že se nevejdou na obrazovku, tak je potřeba vertikálně skrolovat). Pro spuštění plánu je potřeba na něj kliknout.

![homepage](https://github.com/pslib-cz/2023-l4-web-mockupapp-tomaspacak/blob/main/img/homepage.png)

#### Spuštěný plán
Nahoře se nacházejí stopky, které měří uplynulý čas při cvičení. Lze je pozastavit pomocí tlačítka pauza dole, stejným tlačítkem se opět spustí. Pod názvem plánu a stopkami se nachází seznam cviků. Vedle každého cviku se nachází ikona, na kterou uživatel klikne, když je s cvikem hotov. Ve chvíli kdy jsou zakliknuta veškerá cvičení, tak je plán ukončen pomocí jediného tlačítka dole, poté je uživatel přesměrován na homepage. Plán lze i předčasně ukončit pomocí tlačítka vedle tlačítka pauza, po té je uživatel automaticky přesměrován na homepage.

![spuštěný plán](https://github.com/pslib-cz/2023-l4-web-mockupapp-tomaspacak/blob/main/img/spusteny_plan.png)

### Nový plán
V této části je možné vytvořit nový plán, který se po uložení zobrazí na homepage.
![tvorba nového plánu](https://github.com/pslib-cz/2023-l4-web-mockupapp-tomaspacak/blob/main/img/novy_plan.png)

### Moje data
Zde si uživatel zapisuje svoji váhu, obvod pasu, procentuální míru tuku a svalů. Zároveň je zde vidět celkový čas strávený cvičením.

![moje data](https://github.com/pslib-cz/2023-l4-web-mockupapp-tomaspacak/blob/main/img/moje_data.png)

---
## Statická šablona
[Statická šablona](https://pslib-cz.github.io/2023-l4-web-mockupapp-tomaspacak/index.html)



