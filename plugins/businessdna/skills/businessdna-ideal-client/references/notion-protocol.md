# Notion-protocol

Geldt voor alle vijf de documentskills. Deze skill vult de pagina **Ideal Client**.

---

## Bij de start: vind de pagina

1. Zoek in Notion de pagina **Business DNA**.
2. Kijk wat eronder hangt. Is het een database, kijk daarin; zijn het subpagina's, kijk daar.
3. Zoek de pagina **Ideal Client**.

Zoek nooit rechtstreeks op "Ideal Client" zonder eerst Business DNA te vinden. Een gebruiker kan
elders in haar workspace een pagina met dezelfde naam hebben, en dan schrijf je in het
verkeerde document.

Vergelijk namen hoofdletterongevoelig: in de template kan een pagina net anders geschreven
staan (bijvoorbeeld "Tone Of Voice"). Dat is dezelfde pagina. Hernoem hem niet.

De gebruiker heeft deze structuur zelf binnengehaald door de Business DNA-template te
dupliceren. Jij maakt hem niet.

### Geen verbinding met Notion

> "Ik heb geen verbinding met Notion. Daar komt je Ideal Client-document in te staan, dus zonder
> die verbinding kan ik niet aan de slag.
>
> Wil je dat ik uitleg hoe je die connector instelt?"

Bij ja: leg de stappen uit (in de Claude-app naar Aanpassingen (Customize) > Connectors,
Notion zoeken, Verbinden, toegang geven, terugkomen). Ga daarna niet verder tot het gelukt is. Begin geen interview waarvan
de uitkomst nergens heen kan.

### Business DNA niet gevonden

> "Ik zie dat je nog geen Business DNA-omgeving hebt, die maak ik nu aan."

Roep `businessdna-setup` aan. Die controleert de verbinding, de template en de mappen. Wacht
tot hij klaar is en pak daarna je eigen draad op.

### Business DNA gevonden, maar de pagina Ideal Client niet

> "Je Business DNA staat er, maar ik vind de pagina **Ideal Client** niet. Is hij misschien
> hernoemd? De skills zoeken op die exacte naam.
>
> Zal ik hem anders aanmaken? Dan zet ik hem erbij, alleen zonder de opmaak uit je template."

Maak hem alleen aan na een expliciet ja.

---

## Stap 1: nieuw of aanvullen

Altijd de eerste vraag, vóór alles.

Staat er al inhoud op de pagina, dan stel je deze vraag via het wijzigformulier uit
`wijzigformulier.md`, samen met de materiaalvraag. Kiest de gebruiker daar **opnieuw maken**,
dan bewaar je het oude altijd eerst als kopie (optie 1 hieronder), zonder het te vragen.

> "Wil je een nieuw Ideal Client-document maken, of een bestaande aanvullen?"

**Nieuw** → kijk of er al inhoud op de pagina staat. Zo ja:

> "Je hebt al een Ideal Client-document staan, en dat overschrijven betekent dat het oude
> verdwijnt. Twee mogelijkheden:
>
> 1. Ik bewaar het oude eerst als kopie, en we bouwen een nieuw document
> 2. We overschrijven het
>
> Wat wil je?"

Bij optie 1: kopieer de pagina naar `Ideal Client (oude versie, [datum])` op dezelfde plek voordat
je begint.

**Aanvullen** → is de pagina leeg, zeg dat dan:

> "Je Ideal Client-pagina staat er, maar hij is nog leeg. Er is dus nog niets om aan te vullen.
> Zullen we hem gewoon opbouwen?"

---

## Stap 2: materiaal

De tweede vraag, altijd. Welk soort materiaal nuttig is voor dit document, staat in SKILL.md.

Vast onderdeel van de vraag:

> "Je kunt bestanden in dit gesprek slepen, tekst plakken, of me het pad naar een map geven.
> Staat er al iets in de map CLAUDE/Business Copybank op je bureaublad, dan kijk ik daar zelf.
>
> Heb je niets, dan beginnen we gewoon met vragen."

Kijk zelf in `CLAUDE/Business Copybank/` op het bureaublad. Daar staan submappen per soort:
`aanbod/`, `bedrijfsdocumenten/`, `emails/`, `klantgesprekken/`, `social posts/`,
`transcripties/` en `website teksten/`. Welke voor dit document relevant zijn, staat in
SKILL.md.

Negeer bestanden die met `internal_` beginnen.

---

## Tijdens het werk: niets naar Notion

Schrijf tijdens het interview niets weg. Goedkeuring gaat per sectie, in het gesprek. Pas
als alle secties zijn goedgekeurd, ga je schrijven.

Houd de goedgekeurde secties bij in het gesprek en gebruik ze als input voor de volgende.

---

## Aan het eind: wegschrijven naar twee plekken

Nadat de gebruiker het volledige document heeft goedgekeurd. Doe beide stappen, niet alleen de
eerste.

### 1. Naar Notion: de pagina én de properties

Zet het volledige document op de pagina **Ideal Client**, met een H2 per sectie.

**Vul daarna altijd de properties in.** Dit wordt het vaakst vergeten en is precies waar de
gebruiker later op stuurt: haar overzicht laat anders zien dat er niets gebeurd is.

| Property | Waarde |
|---|---|
| `Status` | `Compleet` als het volledige document erin staat. Staat er een deel in en gaan jullie later verder, dan `In progress`. Nog niets: laat `Leeg` staan. |
| `Laatst bijgewerkt` | De datum van vandaag, als datum (YYYY-MM-DD). Ook bij een kleine aanvulling. |

Zoek de datum van vandaag op, gok hem niet.

Heten de properties in de template van de gebruiker net anders (`Bijgewerkt`, `Status
document`), gebruik dan die namen. Bestaat een property helemaal niet, sla hem dan over
zonder er iets over te zeggen. Maak nooit zelf properties aan: het is de template van de
gebruiker.

Deze stap geldt voor alle vijf de documentskills, ook wanneer je maar één sectie hebt
bijgewerkt.

### 2. Naar het bureaublad: het volledige document

Schrijf hetzelfde document als Markdown naar
`CLAUDE/Business DNA/Origineel/Ideal Client.md`.

De map `Origineel/` hoort ín `CLAUDE/Business DNA/`, nooit ernaast en nooit direct onder
`CLAUDE/`. Bestaat hij niet, maak hem daar aan.

Bestaat het bestand al, hernoem het oude naar `Ideal Client (vervangen [datum]).md` voordat je het
nieuwe wegschrijft. Overschrijf nooit zonder de oude te bewaren.

Lukt het wegschrijven niet, dan is dat geen blokkade — Notion is de hoofdopslag. Meld het en
ga door.

### SAMENVATTING.md raak je niet aan

`CLAUDE/Business DNA/SAMENVATTING.md` is de verkorte versie van alle vijf de documenten samen. Die
wordt **niet** per skill bijgewerkt. Hij wordt in één keer opgebouwd als alle vijf de
documenten compleet zijn, buiten deze skills om. Schrijf er dus niets in, noem hem niet in
je terugkoppeling, en beloof er niets over.

### 3. Rapporteer met links

> "Je Ideal Client-document is klaar en staat op twee plekken:
>
> - In Notion: [de echte URL van de pagina] — status op Compleet, bijgewerkt vandaag
> - Volledig op je bureaublad: CLAUDE/Business DNA/Origineel/Ideal Client.md"

---

## Notion is de bron, de bestanden zijn een export

Twee kopieën betekenen dat ze uit elkaar kunnen lopen. Werk daarom altijd volgens deze regel:

- **Schrijven doe je naar allebei.**
- **Lezen doe je uitsluitend uit Notion.**

Werkt de gebruiker haar document later bij, dan doet ze dat in Notion. De bestanden op het
bureaublad zijn een momentopname: handig om in een andere AI-chat te slepen en handig als
back-up, maar nooit de plek waar je iets vandaan haalt. Zo maakt het niet uit dat een bestand
op een dag achterloopt.

---

## Als het wegschrijven mislukt

Laat het werk nooit verdampen. Zet het volledige document in je antwoord in het gesprek:

> "Het wegschrijven naar Notion lukte niet: [reden]. Hier is je volledige document, zodat je
> het niet kwijt bent. Zeg het als ik het opnieuw moet proberen."
