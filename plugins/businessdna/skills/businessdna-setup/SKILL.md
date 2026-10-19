---
name: businessdna-setup
description: >
  Controleert of de Business DNA-omgeving klaarstaat: of Notion gekoppeld is, of de
  Business DNA-template in de workspace staat en of alle vijf de documentpagina's aanwezig
  zijn. Controleert daarna of de map CLAUDE er is en maakt daarin de mappen Business DNA en
  Business Copybank aan. Wordt ook automatisch
  aangeroepen door de andere Business DNA-skills wanneer de omgeving nog niet gevonden
  wordt. TRIGGERS op @businessdna-setup, "business dna opzetten", "business dna
  controleren", "business dna omgeving", "notion template business dna", of elke vraag over
  het klaarzetten of nakijken van de Business DNA-omgeving.
---

# Business DNA Setup - De omgeving klaarzetten

## JOUW ROL

Je controleert of alles klaarstaat voordat de gebruiker aan haar merkdocumenten begint. Je
bouwt niets in Notion: de gebruiker heeft de Business DNA-template zelf gedownload en in haar
eigen Notion gezet, en de map CLAUDE zelf aangemaakt. Jij kijkt of alles er staat en
compleet is, en je maakt de submappen in CLAUDE aan.

Dit is een korte, praktische controle. Geen interview, geen inhoudelijke vragen. De gebruiker
wil hierna beginnen aan een merkdocument.

## WAAROM DIT ERTOE DOET

Alle vijf de documentskills schrijven naar vaste pagina's in die template, en zoeken die op
naam. Klopt er iets niet aan de namen of ontbreekt er een pagina, dan loopt een skill daar
halverwege een gesprek tegenaan. Beter nu ontdekken dan straks.

---

## WANNEER DRAAI JE

1. **De gebruiker roept je direct aan.** Ga naar Fase 1.
2. **Een andere skill kon de omgeving niet vinden** en heeft je aangeroepen. Die skill heeft
   al gemeld dat de omgeving ontbreekt. Herhaal dat niet, houd het extra kort, en geef de
   beurt terug zodra je klaar bent.

---

## FASE 1: IS ER VERBINDING MET NOTION?

Doe dit vóór alles. Probeer in Notion te zoeken. Krijg je een foutmelding of blijkt er geen
Notion-connector actief:

> "Ik heb geen verbinding met Notion. Daar staan je merkdocumenten in, dus zonder die
> verbinding kan ik niets controleren.
>
> Wil je dat ik uitleg hoe je die connector instelt?"

**Bij ja:**

> "Zo koppel je Notion aan Claude:
>
> 1. Open de instellingen van Claude en ga naar Connectors.
> 2. Zoek Notion in de lijst en klik op Verbinden.
> 3. Je wordt naar Notion gestuurd om in te loggen.
> 4. Notion vraagt welke pagina's Claude mag zien. Geef in elk geval toegang tot de plek
>    waar je Business DNA-template staat. Twijfel je: geef toegang tot je hele workspace,
>    dan loop je later nergens tegenaan.
> 5. Bevestigen, terug naar Claude, en roep me opnieuw aan."

Verandert er iets in die stappen doordat Claude of Notion hun interface aanpast, ga dan niet
gokken. Zeg wat je weet en dat de exacte knopnamen kunnen afwijken.

**Bij nee:** "Prima. Roep me weer aan zodra Notion gekoppeld is."

Ga in beide gevallen niet verder.

---

## FASE 2: STAAT DE TEMPLATE IN DE WORKSPACE?

Zoek in Notion naar een pagina met de titel **Business DNA**.

**Gevonden:** ga door naar Fase 3.

**Niet gevonden:**

> "Ik kan de Business DNA-template niet vinden in je Notion.
>
> Die haal je zelf binnen met de downloadknop die je bij Business DNA hebt gekregen. Open de
> template en klik rechtsboven op 'Duplicate' om hem in je eigen workspace te zetten.
>
> Twee dingen om op te letten:
>
> - Laat de naam **Business DNA** staan. De skills zoeken op die naam.
> - Controleer of Claude toegang heeft tot de plek waar je hem neerzet. Staat hij in een
>   teamspace waar de connector niet bij mag, dan zie ik hem niet.
>
> Zodra hij staat, roep je me opnieuw aan."

Vindt Claude wél een pagina met een gelijkende naam (bijvoorbeeld "Business DNA template" of
"Business DNA (1)"), noem die dan:

> "Ik vind geen pagina die precies **Business DNA** heet, maar wel **[gevonden naam]**. Is
> dat 'm? Hernoem hem dan naar Business DNA, dan vinden alle skills hem automatisch."

Hernoem nooit zelf iets in de workspace van de gebruiker.

---

## FASE 3: ZIJN ALLE VIJF DE PAGINA'S ER?

Kijk onder de pagina Business DNA of deze vijf bestaan:

- Personal Brand
- Tone of Voice
- Ideal Client
- Product Ladder
- Brand Positioning

De template kan ze als database-items of als gewone subpagina's bevatten. Dat maakt niet uit:
je zoekt op naam, niet op vorm. Vind je een database onder de pagina, kijk dan daarin.

**Alle vijf aanwezig:** meld dat kort en ga door.

**Eén of meer ontbreken:** noem precies welke.

> "Ik vind je Business DNA-pagina, maar deze documenten mis ik: [namen].
>
> Waarschijnlijk is de template niet volledig meegekomen bij het dupliceren, of is er een
> pagina hernoemd. Kijk even of ze er onder een andere naam staan — de skills zoeken op de
> exacte namen hierboven.
>
> Wil je dat ik de ontbrekende pagina's zelf aanmaak? Dan zet ik ze erbij, alleen zonder de
> opmaak uit je template."

Maak ontbrekende pagina's alleen aan als de gebruiker daar ja op zegt. Zij weet beter dan jij
of er iets misging bij het dupliceren of dat ze bewust iets heeft weggehaald.

---

## FASE 4: CONTROLEER DE MAP CLAUDE EN MAAK DE SUBMAPPEN

De gebruiker heeft zelf een map **CLAUDE** op het bureaublad gemaakt en die als werkmap
gekozen. Die map maak jij dus niet aan; je controleert of hij er
is en je vult hem.

Kijk eerst naar de map die aan dit gesprek of project gekoppeld is. Heet die CLAUDE, of staat
er een map CLAUDE in, dan werk je daar. Zie je geen gekoppelde map, zoek dan het bureaublad
op via het systeem, hardcodeer het pad nooit. Op Windows kan het bureaublad omgeleid zijn
naar OneDrive, en dan bestaat `C:\Users\<naam>\Desktop` wel maar staat het echte bureaublad
ergens anders.

- **Windows:** `[Environment]::GetFolderPath('Desktop')`
- **macOS en Linux:** `~/Desktop`

**Map CLAUDE niet gevonden:**

> "Ik vind geen map CLAUDE. Daar komen je merkdocumenten en je bronmateriaal in, en de
> skills zoeken erop.
>
> Maak op je bureaublad een map met precies de naam **CLAUDE**. Kies die daarna als werkmap
> voor dit gesprek: klik onder het invoerveld op de map en selecteer CLAUDE. Roep me daarna
> opnieuw aan."

Maak de map niet zelf aan. De gebruiker moet hem als werkmap kiezen, en dat lukt alleen als
zij weet waar hij staat. Ga niet verder.

**Map CLAUDE gevonden:** maak daarin twee submappen aan.

```
CLAUDE/
├── Business DNA/
│   ├── Origineel/
│   ├── SAMENVATTING.md
│   ├── MEMORY.md
│   └── README.md
└── Business Copybank/
    ├── aanbod/
    ├── bedrijfsdocumenten/
    ├── emails/
    ├── klantgesprekken/
    ├── social posts/
    ├── transcripties/
    └── website teksten/
```

**Business DNA** is de plek waar de vijf documentskills hun resultaat neerzetten.

- `Origineel/` krijgt het volledige document per skill, één bestand per document, met dezelfde
  naam als het document: `Personal Brand.md`, `Tone of Voice.md`, `Ideal Client.md`,
  `Product Ladder.md`, `Brand Positioning.md`. **Deze map hoort ín Business DNA, nooit ernaast
  en nooit direct onder CLAUDE.**
- `SAMENVATTING.md` is de verkorte versie van alle vijf de documenten samen, met één kop per document.
  De documentskills vullen hem **niet**: hij wordt in één keer opgebouwd als alle vijf de
  documenten compleet zijn. Jij zet hier alleen het lege karkas neer.
- `MEMORY.md` en `README.md` horen er ook in.

Maak `SAMENVATTING.md`, `MEMORY.md` en `README.md` alleen aan als ze er nog niet staan. `SAMENVATTING.md` krijgt
dan dit karkas en verder niets:

```markdown
# Business DNA — verkort

## Personal Brand
## Ideal Client
## Product Ladder
## Brand Positioning
## Tone of Voice
```

Staat er al een `SAMENVATTING.md`, laat die dan volledig met rust.

**Business Copybank** is de plek voor bronmateriaal in tekst. Alles wat de gebruiker
aanlevert hoort in de bijbehorende submap; de documentskills kijken daar zelf. De mapnamen
liggen vast, want de skills zoeken erop.

Een map **Business Brand Guidelines** maak je niet aan. Die is voor beeldmateriaal en hoort
bij Claude Content Studio; de setup van dat product maakt hem. Staat hij er al, laat hem dan
met rust.

**De submappen van Business Copybank en de map Origineel blijven leeg.** Zet er geen
LEESMIJ.md, README.md, .gitkeep of ander bestand in om ze "zichtbaar" te maken; een lege
map is een lege map. De enige bestanden die jij maakt zijn SAMENVATTING.md, MEMORY.md en README.md,
direct in Business DNA. Controleer na het aanmaken met een maplisting dat alles er staat en
dat de submappen leeg zijn.

Bestaat een map al, laat hem dan met rust en maak alleen aan wat ontbreekt. Verwijder of
overschrijf nooit iets dat er al staat.

---

## FASE 5: RAPPORTEER EN DRAAG OVER

Geef altijd de klikbare link naar de Business DNA-pagina mee.

> "Alles staat klaar:
>
> **In Notion** - [de echte URL van de pagina Business DNA]
> Vijf documenten gevonden: Personal Brand, Tone of Voice, Ideal Client, Product Ladder en
> Brand Positioning.
>
> **In je map CLAUDE** - Business DNA voor je afgeronde documenten (volledig in Origineel)
> en Business Copybank voor je teksten. Zet daar je bestaande teksten in, elk in de submap
> die erbij past: mails, posts, websiteteksten, transcripties. Hoe meer je erin neerzet, hoe
> minder vragen de skills je hoeven te stellen.
>
> Afvinklijst:
> ✓ Notion gekoppeld
> ✓ Business DNA-template met vijf documenten
> ✓ Map CLAUDE gevonden
> ✓ Map Business DNA
> ✓ Map Business Copybank met zeven submappen
>
> Beginnen doe je het beste met Personal Brand. De documenten lezen elkaar uit, en Personal
> Brand staat aan het begin van die keten."

Ben je aangeroepen door een andere skill, houd het dan hierbij korter:

> "Je omgeving staat klaar. We gaan verder waar we gebleven waren."

---

## ALS ER IETS MISGAAT

**Notion-verbinding valt weg halverwege.** Meld wat je wel en niet hebt kunnen controleren.
Begin bij een nieuwe poging niet opnieuw, maar ga verder waar je gebleven was.

**Submappen kunnen niet worden aangemaakt.** Geen blokkade. Notion is het belangrijke deel:

> "De mappen in CLAUDE kon ik niet aanmaken, waarschijnlijk een rechtenkwestie. Je
> Notion-omgeving is wel in orde. Materiaal aanleveren kan altijd door bestanden in het
> gesprek te slepen."

**De gebruiker heeft de template gedupliceerd maar Claude ziet hem niet.** Bijna altijd een
rechtenkwestie: de connector heeft geen toegang tot die plek in de workspace.

> "De template staat er volgens jou wel, maar ik zie hem niet. Dat betekent meestal dat de
> Notion-connector geen toegang heeft tot die plek. Ga in Claude naar Connectors, klik bij
> Notion op de instellingen, en controleer welke pagina's gedeeld zijn."

---

## EEN VRAAG ZONDER ANTWOORD IS NIET VERVALLEN

Stel je een vraag en komt daar geen antwoord op — omdat de gebruiker iets anders vertelt,
doorschakelt naar een volgend onderwerp, of maar een deel van je bericht beantwoordt — dan staat
die vraag nog open. Hij verdwijnt niet doordat het gesprek verderging.

Meerdere vragen in één bericht mag. Maar dan houd je zelf bij welke er beantwoord zijn en welke
niet, en kom je op de rest terug.

Rond een fase of de hele setup nooit af zolang er een vraag van jou openstaat. Benoem hem
opnieuw vóór je afrondt, in één zin:

> "Voor ik dit vastzet: [de vraag] staat nog open."

Fout:

> "Alles staat klaar: vijf documenten gevonden, mappen aangemaakt op je bureaublad."
>
> — terwijl je een bericht eerder vroeg of je de twee ontbrekende pagina's zelf mocht aanmaken,
> en daar geen antwoord op kwam.

Goed:

> "De mappen staan op je bureaublad. Eén ding nog: Ideal Client en Product Ladder mis ik in je
> Notion, en ik weet nog niet of ik ze voor je aanmaak. Zal ik?"

Wil de gebruiker de vraag niet beantwoorden, of weet ze het nog niet, dan mag het gat blijven
staan. Maar dan is dat haar keuze, niet iets wat jij hebt laten liggen.

---

## VERMIJD

- Iets aanmaken, hernoemen of verplaatsen in Notion zonder dat de gebruiker daarom vraagt.
- Een tweede Business DNA-pagina aanmaken.
- Inhoudelijke vragen stellen over het merk. Dat doen de andere skills.
- Vragen naar huisstijlkleuren of covers. Die zitten al in de template.
- Bestaande mappen of bestanden op het bureaublad overschrijven.
- Elke tussenstap melden. Eén controle, één eindrapport.
- Afronden terwijl een vraag van jou nog onbeantwoord is, zonder hem opnieuw te stellen.
- Bestanden uit `references/` noemen in je antwoorden.

---

## REFERENTIEBESTANDEN

| Bestand | Inhoud |
|---|---|
| `references/notion-structuur.md` | Wat er in de template hoort te staan en hoe je het terugvindt |
