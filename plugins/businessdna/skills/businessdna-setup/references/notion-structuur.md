# Notion-structuur

Wat er in de Business DNA-template hoort te staan, en hoe elke skill het terugvindt.

De gebruiker maakt deze structuur niet zelf: ze downloadt de template en dupliceert hem naar
haar eigen workspace. Deze skill controleert alleen.

---

## Wat er moet staan

```
Business DNA                    (pagina)
├── Personal Brand
├── Tone of Voice
├── Ideal Client
├── Product Ladder
└── Brand Positioning
```

Onder **Tone of Voice** kunnen later optionele kanaalsubpagina's komen te hangen
(`Tone of Voice - Salespaginas`, `Tone of Voice - Social content`, `Tone of Voice - Social
content - voorbeelden`, `Tone of Voice - E-mail en DM`). Die maakt de Tone of Voice-skill zelf aan als de gebruiker daarom vraagt. Jij
controleert er niet op en maakt ze niet aan.

De vijf documenten kunnen in de template database-items zijn of gewone subpagina's. Voor het
terugvinden maakt dat niet uit: er wordt op naam gezocht, niet op vorm.

**De namen liggen vast.** Elke documentskill zoekt de pagina die exact zo heet als het
document dat hij vult. Wordt er een pagina hernoemd, dan vindt die skill hem niet meer.

---

## Hoe je zoekt

1. Zoek de pagina **Business DNA** in de workspace.
2. Kijk wat eronder hangt. Is dat een database, kijk dan daarin. Zijn het losse subpagina's,
   kijk dan daar.
3. Zoek de pagina met de naam van het document.

Zoek nooit alleen op de documentnaam zonder eerst Business DNA te vinden. Een gebruiker kan
elders in haar workspace ook een pagina "Personal Brand" hebben staan, en dan schrijf je in
het verkeerde document.

---

## Properties

De template heeft per document deze properties:

| Property | Type | Wat de skills ermee doen |
|---|---|---|
| `Naam` | titel | De documentnaam. Nooit wijzigen: de skills zoeken erop. |
| `Status` | select: `Leeg`, `In progress`, `Compleet` | Op `Compleet` zodra het volledige document erin staat. Op `In progress` als er een deel in staat. |
| `Laatst bijgewerkt` | datum | De datum waarop de skill het document heeft bijgewerkt. |

**Elke documentskill vult deze twee properties in bij het wegschrijven.** Dat is geen extraatje:
zonder die twee laat het overzicht in Notion zien dat er niets gebeurd is, terwijl de pagina vol
staat. Controleer bij deze setup of ze bestaan en meld het als er een ontbreekt.

Heten ze in de workspace van de gebruiker net anders, dan gebruiken de skills die namen.
Bestaat een property helemaal niet, dan slaan ze hem over zonder er iets over te zeggen.

Maak nooit properties aan die er niet zijn. Dat is de template van de gebruiker.

---

## Wanneer een pagina ontbreekt

Meld welke, en bied aan hem aan te maken. Doe dat alleen na een expliciet ja. Een ontbrekende
pagina betekent meestal dat er iets misging bij het dupliceren, of dat de gebruiker bewust
iets heeft weggehaald — dat weet zij, jij niet.

Maak je er een aan, zet hem dan onder Business DNA op dezelfde plek als de andere vier, met de
exacte documentnaam als titel. Verder leeg; de skill vult hem daarna.

---

## Wanneer de hele template ontbreekt

Bouw hem niet na. De template bevat opmaak, covers en toelichting die deze plugin niet kent,
en een zelfgebouwde variant ziet er anders uit dan wat de gebruiker heeft gekocht.

Verwijs terug naar het dupliceren van de template, en controleer daarna opnieuw.
