# Notion-protocol

Geldt voor alle vijf de documentskills. Deze skill vult de pagina **Tone of Voice**, en bij
een kanaalkeuze ook de subpagina's daaronder.

---

## Bij de start: vind de pagina

1. Zoek in Notion de pagina **Business DNA**.
2. Kijk wat eronder hangt. Is het een database, kijk daarin; zijn het subpagina's, kijk daar.
3. Zoek de pagina **Tone of Voice**.

Zoek nooit rechtstreeks op "Tone of Voice" zonder eerst Business DNA te vinden. Een gebruiker kan
elders in haar workspace een pagina met dezelfde naam hebben, en dan schrijf je in het
verkeerde document.

Vergelijk namen hoofdletterongevoelig: in de template kan een pagina net anders geschreven
staan (bijvoorbeeld "Tone Of Voice"). Dat is dezelfde pagina. Hernoem hem niet.

De gebruiker heeft deze structuur zelf binnengehaald door de Business DNA-template te
dupliceren. Jij maakt hem niet.

Kijk meteen ook of er al kanaalpagina's onder Tone of Voice hangen (zie "Waar de
kanaalmodules landen"). Dan weet je bij de reikwijdtevraag al wat er staat.

### Geen verbinding met Notion

> "Ik heb geen verbinding met Notion. Daar komt je Tone of Voice-document in te staan, dus zonder
> die verbinding kan ik niet aan de slag.
>
> Wil je dat ik uitleg hoe je die connector instelt?"

Bij ja: leg de stappen uit (Claude-instellingen → Connectors → Notion → verbinden → toegang
geven → terugkomen). Ga daarna niet verder tot het gelukt is. Begin geen interview waarvan
de uitkomst nergens heen kan.

### Business DNA niet gevonden

> "Ik zie dat je nog geen Business DNA-omgeving hebt, die maak ik nu aan."

Roep `businessdna-setup` aan. Die controleert de verbinding, de template en de mappen. Wacht
tot hij klaar is en pak daarna je eigen draad op.

### Business DNA gevonden, maar de pagina Tone of Voice niet

> "Je Business DNA staat er, maar ik vind de pagina **Tone of Voice** niet. Is hij misschien
> hernoemd? De skills zoeken op die exacte naam.
>
> Zal ik hem anders aanmaken? Dan zet ik hem erbij, alleen zonder de opmaak uit je template."

Maak hem alleen aan na een expliciet ja.

---

## Stap 0: de reikwijdte

Dit is de allereerste vraag van de skill, nog vóór nieuw-of-aanvullen. De vraag zelf en hoe je
hem stelt, staan in `vragen.md` onder "Vooraf: de reikwijdte".

Wat de uitkomst bepaalt:

| Keuze | Wat je maakt | Waar het landt |
|---|---|---|
| Algemeen | alleen het basisdocument | de pagina **Tone of Voice** |
| Algemeen plus kanalen | het basisdocument én één document per gekozen kanaal | de pagina **Tone of Voice**, plus een subpagina per kanaal |

Het basisdocument maak je altijd, ook als de gebruiker alleen om kanalen vraagt.

Staan er al kanaalpagina's die de gebruiker nu niet kiest, laat ze dan met rust. Noem ze één
keer, en ga verder:

> "Er staat al een document voor je e-mails en DM's. Dat laat ik zoals het is."

---

## Stap 1: nieuw of aanvullen

De tweede vraag, direct na de reikwijdte.

> "Wil je een nieuw Tone of Voice-document maken, of een bestaande aanvullen?"

Werkt de gebruiker met kanalen, dan geldt het antwoord voor alles wat je in deze ronde
aanraakt. Is het beeld gemengd — de basis staat er wel, een kanaalpagina nog niet — zeg dat
dan:

> "Je basisdocument staat er al, de kanaaldocumenten nog niet. Ik vul de basis dus aan en de
> kanalen bouw ik nieuw op. Goed zo?"

**Nieuw** → kijk of er al inhoud op de pagina staat. Zo ja:

> "Je hebt al een Tone of Voice-document staan, en dat overschrijven betekent dat het oude
> verdwijnt. Twee mogelijkheden:
>
> 1. Ik bewaar het oude eerst als kopie, en we bouwen een nieuw document
> 2. We overschrijven het
>
> Wat wil je?"

Bij optie 1: kopieer de pagina naar `Tone of Voice (oude versie, [datum])` op dezelfde plek voordat
je begint. Kanaalpagina's die je vervangt, kopieer je op dezelfde manier.

**Aanvullen** → is de pagina leeg, zeg dat dan:

> "Je Tone of Voice-pagina staat er, maar hij is nog leeg. Er is dus nog niets om aan te vullen.
> Zullen we hem gewoon opbouwen?"

---

## Stap 2: materiaal

De derde vraag, altijd. Welk soort materiaal nuttig is voor dit document, staat in SKILL.md;
wat je per gekozen kanaal minstens nodig hebt, staat in `vragen.md` onder "Vooraf: voorbeelden
en templates".

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

Schrijf tijdens het interview niets weg. Goedkeuring gaat per sectie en per module, in het
gesprek. Pas als alles is goedgekeurd, ga je schrijven.

Houd de goedgekeurde secties en modules bij in het gesprek en gebruik ze als input voor de
volgende.

---

## Waar de kanaalmodules landen

Elke module is een eigen document en krijgt een eigen **subpagina onder Tone of Voice**, met
deze namen:

| Module | Paginanaam | Bestandsnaam |
|---|---|---|
| Salespagina's | `Tone of Voice - Salespaginas` | `Tone of Voice - Salespaginas.md` |
| Social content | `Tone of Voice - Social content` | `Tone of Voice - Social content.md` |
| Social content, voorbeelden | `Tone of Voice - Social content - voorbeelden` | `Tone of Voice - Social content - voorbeelden.md` |
| E-mails en DM's | `Tone of Voice - E-mail en DM` | `Tone of Voice - E-mail en DM.md` |

Social content levert twee documenten op: de module zelf, en een apart document met de vijf
stijlvoorbeelden. Beide hangen **direct onder Tone of Voice**, naast elkaar, niet het ene onder
het andere. Het voorbeeldendocument maak je alleen bij de keuze social content, en altijd
samen met de module.

Bestaat de subpagina al, gebruik hem. Bestaat hij niet, dan maak je hem aan — daar heb je geen
aparte toestemming voor nodig, want de gebruiker heeft er bij de reikwijdtevraag al om
gevraagd. Zeg wel wat je gaat aanmaken voordat je het doet.

Zet boven aan elke kanaalpagina één regel die naar de basis verwijst:

> *Deze module hoort bij het basisdocument Tone of Voice en legt alleen vast wat op dit kanaal
> anders is. Lees ze samen.*

Op de pagina **Tone of Voice - Social content - voorbeelden** staat in plaats daarvan:

> *Dit zijn de vijf posts die het best laten zien hoe ik op social klink. Ze horen bij Tone of
> Voice en Tone of Voice - Social content. Lees ze samen.*

Zet omgekeerd onder aan het basisdocument een lijstje met de kanaaldocumenten die erbij horen,
met links.

---

## Aan het eind: wegschrijven naar twee plekken

Nadat de gebruiker het volledige document heeft goedgekeurd — bij kanalen: nadat zij de basis
én elke module heeft goedgekeurd. Doe beide stappen, niet alleen de eerste.

### 1. Naar Notion: de pagina's én de properties

Zet het basisdocument op de pagina **Tone of Voice**, met een H2 per sectie. Zet elke module
op haar eigen subpagina, ook met een H2 per onderdeel.

**Vul daarna altijd de properties in.** Dit wordt het vaakst vergeten en is precies waar de
gebruiker later op stuurt: haar overzicht laat anders zien dat er niets gebeurd is.

| Property | Waarde |
|---|---|
| `Status` | `Compleet` als alles wat in deze ronde is afgesproken erin staat — de basis én elke gekozen module. Ontbreekt er nog een module, dan `In progress`. Nog niets: laat `Leeg` staan. |
| `Laatst bijgewerkt` | De datum van vandaag, als datum (YYYY-MM-DD). Ook bij een kleine aanvulling. |

Zoek de datum van vandaag op, gok hem niet.

De properties zitten op de pagina **Tone of Voice** uit de template. De subpagina's die jij
aanmaakt hebben ze niet; maak ze daar ook niet aan.

Heten de properties in de template van de gebruiker net anders (`Bijgewerkt`, `Status
document`), gebruik dan die namen. Bestaat een property helemaal niet, sla hem dan over
zonder er iets over te zeggen. Maak nooit zelf properties aan: het is de template van de
gebruiker.

Deze stap geldt voor alle vijf de documentskills, ook wanneer je maar één sectie hebt
bijgewerkt.

### 2. Naar het bureaublad: alle documenten

Schrijf elk document als Markdown naar `CLAUDE/Business DNA/Origineel/`, met de bestandsnamen
uit de tabel hierboven. Het basisdocument blijft `Tone of Voice.md`.

De map `Origineel/` hoort ín `CLAUDE/Business DNA/`, nooit ernaast en nooit direct onder
`CLAUDE/`. Bestaat hij niet, maak hem daar aan.

Bestaat een bestand al, hernoem het oude naar `[naam] (vervangen [datum]).md` voordat je het
nieuwe wegschrijft. Overschrijf nooit zonder de oude te bewaren.

Lukt het wegschrijven niet, dan is dat geen blokkade — Notion is de hoofdopslag. Meld het en
ga door.

### SAMENVATTING.md raak je niet aan

`CLAUDE/Business DNA/SAMENVATTING.md` is de verkorte versie van alle vijf de documenten samen. Die
wordt **niet** per skill bijgewerkt. Hij wordt in één keer opgebouwd als alle vijf de
documenten compleet zijn, buiten deze skills om. Schrijf er dus niets in, noem hem niet in
je terugkoppeling, en beloof er niets over.

### 3. Rapporteer met links

Noem elk document apart, met de echte link. Bij alleen een basisdocument:

> "Je Tone of Voice-document is klaar en staat op twee plekken:
>
> - In Notion: [de echte URL van de pagina] — status op Compleet, bijgewerkt vandaag
> - Volledig op je bureaublad: CLAUDE/Business DNA/Origineel/Tone of Voice.md"

Bij kanalen erbij:

> "Je Tone of Voice staat klaar, in [aantal] documenten:
>
> - **Basis** — [URL] — CLAUDE/Business DNA/Origineel/Tone of Voice.md
> - **Salespagina's** — [URL] — CLAUDE/Business DNA/Origineel/Tone of Voice - Salespaginas.md
> - **Social content** — [URL] — CLAUDE/Business DNA/Origineel/Tone of Voice - Social content.md
> - **Social content, voorbeelden** — [URL] — CLAUDE/Business DNA/Origineel/Tone of Voice - Social content - voorbeelden.md
>
> De status op je Tone of Voice-pagina staat op Compleet, bijgewerkt vandaag.
>
> Geef je dit aan een AI-tool, geef dan altijd de basis mee plus het kanaal waarvoor je
> schrijft. Alleen een kanaaldocument is niet genoeg."

Is een module niet af, zeg dat hier ook, met wat je nodig hebt om hem af te maken.

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

Gaat het om meerdere documenten en lukt er één niet, schrijf de rest dan gewoon weg en zet
alleen het mislukte document in het gesprek.
