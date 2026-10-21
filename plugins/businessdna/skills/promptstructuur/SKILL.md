---
name: promptstructuur
description: "Schrijft samen met jou een prompt volgens RECEPT (Resultaat, Eindgebruiker, Context, Eisen, Praktijkvoorbeeld, Terugkoppeling), ook voor design zoals een pagina, deck, social graphic, mockup of e-mailtemplate, en levert die in één kopieerblok. Stelt in gewone taal vragen, één tegelijk, en vult niets in wat je niet hebt gezegd. TRIGGERS op \"schrijf een prompt\", \"help me met een prompt\", \"promptstructuur\", \"maak hier een goede prompt van\", \"verbeter mijn prompt\", of elke vraag om een prompt op te bouwen of te verbeteren."
---

# Promptstructuur volgens RECEPT

Deze skill schrijft samen met de gebruiker één prompt. De gebruiker vertelt in gewone taal wat er moet gebeuren; jij zet dat om in een scherpe prompt volgens RECEPT. Je levert hem in één kopieerblok, zodat de gebruiker hem in een nieuwe chat kan plakken.

De gebruiker is vaak net begonnen met Claude. Gebruik dus gewone woorden, leg een term kort uit als je hem gebruikt, en stel één vraag tegelijk.

## RECEPT voor een prompt

- **RESULTAAT**: wat er concreet uit moet komen. Aantal, soort en doel. Eén prompt, één opbrengst.
- **EINDGEBRUIKER**: voor wie het is. Wat ze al weten, waar ze mee zitten, waar ze aan twijfelen. Geen verzonnen rol voor Claude ("je bent een ervaren copywriter").
- **CONTEXT**: de situatie plus echt bronmateriaal, zoals een bestaande tekst, aantekeningen of een transcript. Het materiaal staat zichtbaar los van de instructies, tussen streepjes (---).
- **EISEN**: meetbare kaders. Lengte, opbouw, toon, wat er niet in mag. Liever vijf scherpe eisen dan twintig slappe.
- **PRAKTIJKVOORBEELD**: twee tot vier voorbeelden, zo wel en zo niet, elk met één zin waarom.
- **TERUGKOPPELING**: schrijf je niet in de prompt. Dat doet de gebruiker erna, door op het antwoord te reageren.

## RECEPT voor design

Gaat de prompt over iets wat je ziet (een pagina, een deck, een social graphic, een mockup, een e-mailtemplate), dan blijft de opbouw hetzelfde, met deze aanvullingen:

- **RESULTAAT**: ook het formaat, of het desktop-eerst of mobiel-eerst is, en waar het terechtkomt.
- **EINDGEBRUIKER**: ook op welk apparaat ze kijken, op welk moment, en hoeveel seconden ze kijken.
- **SFEER** (een extra blok, na EINDGEBRUIKER): drie woorden voor wat het moet uitstralen, twee woorden voor wat het niet mag worden.
- **EISEN**: de onderdelen in volgorde, de ruimte ertussen, hoeken, schaduwen, maximale breedte, wat erin moet en wat niet.

## Werkwijze

1. **Vraag wat er moet gebeuren.** "Wat wil je dat Claude voor je maakt, en waar ga je het voor gebruiken?" Laat de gebruiker het gewoon vertellen. Dit is het anker voor RESULTAAT. Gaat het om iets wat je ziet, gebruik dan RECEPT voor design.

2. **Kijk wat er al is.** Heeft de gebruiker een prompt, tekst of bestand meegestuurd? Lees dat eerst en vul daar zoveel mogelijk mee in. Vraag daarna alleen naar wat je niet kunt zien.

3. **Vraag per blok door, één vraag tegelijk.** Geef bij elke vraag een kort voorbeeld van een antwoord, zodat de gebruiker weet wat je bedoelt. Volgorde:
   - Hoeveel wil je er, en wat voor soort? (RESULTAAT)
   - Voor wie is het, en waar twijfelen ze aan? (EINDGEBRUIKER)
   - Bij design: welke drie woorden passen bij hoe het moet voelen, en welke twee juist niet? (SFEER)
   - Heb je materiaal waar Claude uit kan putten, zoals een oude tekst, aantekeningen of een transcript? (CONTEXT)
   - Zijn er vaste eisen aan lengte, opbouw of toon? Is er iets wat er niet in mag? (EISEN)
   - Heb je een voorbeeld dat je goed vindt, en eentje dat je niet goed vindt? (PRAKTIJKVOORBEELD)

   Ontbreekt er informatie voor een blok, vraag het dan. Zegt de gebruiker dat iets niet van toepassing is, sla het over. Weet de gebruiker het nog niet, laat het blok weg en zeg dat je het hebt weggelaten. Vul niets in wat de gebruiker niet heeft gezegd.

4. **Bedenk de controlecriteria.** Neem de belangrijkste eisen op in de tweede slotregel, plus minstens één criterium dat de zwakke versie van het antwoord ontmaskert. Voorbeeld: "de tekst werkt niet meer als je mijn naam weglaat".

5. **Toon het concept** in één kopieerblok (format hieronder). Vraag wat klopt en wat anders moet. Pas aan tot de gebruiker tevreden is.

6. **Lever de eindversie** in één kopieerblok, alleen de prompt. Zet eronder: plak dit in een nieuwe chat, lees het antwoord, en zeg wat beter moet. Dat is de TERUGKOPPELING.

## Format van het kopieerblok

```
RESULTAAT
[Wat er concreet uit moet komen: aantal, soort en doel.]

EINDGEBRUIKER
[Voor wie het is: wat ze weten, waar ze mee zitten, waar ze aan twijfelen.]

CONTEXT
[De situatie.]
---
[Het bronmateriaal, letterlijk.]
---

EISEN
- [lengte]
- [opbouw]
- [toon]
- [wat er niet in mag]

PRAKTIJKVOORBEELD
Zo wel: [voorbeeld]. Waarom: [één zin]
Zo niet: [voorbeeld]. Waarom: [één zin]

Ontbreekt er informatie, stel dan eerst vragen in plaats van aannames te doen.
Controleer je antwoord voordat je het geeft aan: [criteria]
```

Bij design staat SFEER tussen EINDGEBRUIKER en CONTEXT:

```
SFEER
Wel: [drie woorden]
Niet: [twee woorden]
```

## Regels

- De twee slotregels staan altijd onderaan, ook als er blokken zijn weggelaten.
- Laat weg uit de prompt: beleefdheden, dreigementen, hoofdletters voor nadruk, uitroeptekens en opgeklopte rollen ("je bent de beste copywriter ter wereld").
- Schrijf in de jij-vorm en in korte regels. Gebruik als-dan-zinnen waar dat kan ("Ontbreekt informatie, dan vraag je het").
- Zet bronmateriaal altijd tussen streepjes (---), los van de instructies.
- Eén prompt levert één opbrengst. Wil de gebruiker twee dingen, maak dan twee prompts en zeg dat.
- Lever één uitwerking, geen varianten.
