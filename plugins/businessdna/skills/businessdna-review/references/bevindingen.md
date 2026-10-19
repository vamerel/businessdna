# Bevindingen: zwaartes, formaat en advies

---

## De drie zwaartes

Zwaarte bepaalt wat de gebruiker ermee moet, niet hoe erg het is. Noem de zwaarte altijd bij
de bevinding, zodat duidelijk is wat moet en wat mag.

**Botsing** — twee documenten zeggen iets dat niet allebei waar kan zijn. Dit moet opgelost
worden. Zolang het blijft staan, krijgt elke skill die beide documenten uitleest
tegenstrijdige instructies.

**Gat** — iets ontbreekt, of het staat er wel maar stuurt niets. Dit mag blijven staan, maar
dan is dat een keuze. Een gat kost geen fouten, wel bruikbaarheid.

**Signaal** — het klopt misschien nog, maar zou verouderd of onbedoeld kunnen zijn. Dit kun je
niet zelf vaststellen; je vraagt het na. De gebruiker beslist of het iets is.

Twijfel je tussen botsing en gat: botst het met een ander document, dan is het een botsing.
Staat het op zichzelf, dan is het een gat.

---

## Het formaat per bevinding

Vier onderdelen, altijd in deze volgorde.

```markdown
### [Zwaarte] — [document] ↔ [document]

**Wat:** [wat je ziet, met het letterlijke citaat uit beide documenten, met vermelding van de
sectie]

**Waarom het uitmaakt:** [welk gevolg dit heeft voor wat er straks mee geschreven wordt]

**Mijn advies:** [wat jij zou doen, en waarom]

**Vraag:** [wat wil zij hiermee] → `@businessdna-[skill]`
```

Bij een bevinding binnen één document vervalt de tweede documentnaam in de kop.

### Uitgewerkt voorbeeld

```markdown
### Botsing — Tone of Voice ↔ Ideal Client

**Wat:** "meedenken" staat in Tone of Voice bij de verboden woorden. In Ideal Client komt het
letterlijk voor in twee klanttaalcitaten: *"ik wil iemand die meedenkt"* en *"niemand die
echt meedenkt met mijn situatie"*.

**Waarom het uitmaakt:** elke schrijfskill leest beide documenten. Nu krijgt hij de opdracht
een woord te vermijden dat volgens hetzelfde merk de taal van je klant is. In de praktijk
betekent dat: je verkoopteksten gaan langs je klant heen precies op het punt waar zij het
duidelijkst zegt wat ze wil.

**Mijn advies:** het verbod slaat waarschijnlijk op je eigen teksten, niet op het weergeven
van je klant. Ik zou de uitzondering toevoegen in plaats van het verbod te schrappen — je had
een reden om het woord te wantrouwen, en die reden geldt nog steeds voor je eigen zinnen.

**Vraag:** wil je "meedenken" uit de verbodenlijst halen, of er de uitzondering bij zetten dat
het wel mag in klantcitaten? → `@businessdna-tone-of-voice`
```

---

## Het citaat is niet optioneel

Zonder letterlijk citaat is een bevinding een mening. Vergelijk:

Mening:

> "Je positionering en je product ladder sluiten niet goed op elkaar aan."

Bevinding:

> "Je positioneringsstatement zegt *'toegankelijk voor wie net begint'*, en je laagste trede is
> een traject van €1.800."

De gebruiker moet elke bevinding zelf kunnen natrekken zonder de documenten erbij te pakken.
Vermeld daarom altijd document én sectie.

---

## Hoe je adviseert

Elke bevinding krijgt een advies. Een review die alleen problemen oplevert, verschuift al het
denkwerk naar de gebruiker — en dat is precies wat ze aan jou uitbesteedde.

**Wel:**

- Zeg wat je zou doen, in één of twee zinnen, met de reden erbij.
- Zitten er meerdere kanten aan, geef dan beide kanten en dan je voorkeur. Niet alleen je
  voorkeur.
- Baseer je advies op wat er in de documenten staat, niet op wat gebruikelijk is in de markt.
- Is de oplossing evident, zeg dat dan gewoon: "hier lijkt me weinig twijfel over".

**Niet:**

- Adviseren over het merk zelf. Of een prijs verstandig is, of een doelgroep kansrijk is, of
  een positionering slim is — daar ga jij niet over. Je toetst of de documenten kloppen en
  bruikbaar zijn.
- Een advies verpakken als besluit. De gebruiker kiest.
- Je advies herhalen als ze iets anders kiest. Neem haar keuze over en ga door.
- Adviseren zonder reden. "Ik zou het weghalen" is geen advies.

---

## Volgorde en tempo

Botsingen één voor één. Ze vragen een keuze, en keuzes stapelen slecht.

Gaten en signalen mogen gegroepeerd per document, met per stuk nog steeds een vraag.

Meer dan zes bevindingen: bied actief aan te splitsen. Bijvoorbeeld eerst de botsingen
afhandelen, de wijzigprompt daarvoor maken, en de gaten in een tweede ronde. Beter twee
afgeronde rondes dan één lijst die half blijft liggen.

---

## Wat je bijhoudt

Per besproken bevinding leg je het besluit vast:

- Welk document en welke sectie
- Wat er nu staat (letterlijk)
- Wat het moet worden, of welke kant het op moet
- Waarom — de reden uit het gesprek, niet uit jouw analyse

Dat laatste is wat de wijzigprompt bruikbaar maakt in een sessie die dit gesprek niet heeft
meegemaakt.

Bevindingen zonder besluit gaan niet mee in de prompt. Meld aan het eind welke dat waren, zodat
de gebruiker weet wat er blijft staan.
