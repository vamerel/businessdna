---
name: projectinstructies
description: "Schrijft samen met jou de projectinstructies voor een Claude-project, opgebouwd volgens RECEPT (Resultaat, Eindgebruiker, Context, Eisen, Praktijkvoorbeeld, Terugkoppeling), en levert ze als kant-en-klaar plakblok. Stelt in gewone taal vragen, één tegelijk, en vult niets in wat je niet hebt gezegd. TRIGGERS op \"ik wil projectinstructies opzetten\", \"projectinstructies\", \"schrijf de instructies voor dit project\", \"help me met mijn project instellen\", of elke vraag om instructies voor een Claude-project te maken of te verbeteren."
---

# Projectinstructies volgens RECEPT

Deze skill schrijft samen met de gebruiker de instructies voor één Claude-project. De gebruiker vertelt in gewone taal wat het project is; jij zet dat om in scherpe instructies volgens RECEPT. Je levert ze als plakblok, want het instructieveld van een project kun je niet zelf invullen.

De gebruiker is vaak net begonnen met Claude. Gebruik dus gewone woorden, leg een term kort uit als je hem gebruikt, en stel nooit meer dan één vraag tegelijk.

## RECEPT voor een project

- **RESULTAAT**: wat er in dit project concreet uitkomt. Het soort output en waar het voor dient. Eén project, één duidelijk doel.
- **EINDGEBRUIKER**: voor wie de output is. Wat ze al weten, waar ze mee zitten, waar ze aan twijfelen. Werkt de gebruiker in dit project alleen voor zichzelf, dan is de gebruiker de eindgebruiker. Geen verzonnen rol voor Claude ("je bent een ervaren copywriter").
- **CONTEXT**: de situatie plus het materiaal waar Claude uit put: een gekoppelde map, bestanden, voorbeelden, merkdocumenten. Bij welke taak leest Claude welk bestand.
- **EISEN**: meetbare kaders. Vorm, lengte, opbouw, toon, wat er niet in mag. Liever vijf scherpe eisen dan twintig slappe. Wil de gebruiker toch een rol, dan staat die hier als één regel.
- **PRAKTIJKVOORBEELD**: twee tot vier voorbeelden, zo wel en zo niet, elk met één zin waarom.
- **TERUGKOPPELING**: schrijf je niet als blok. Het zit in de werkafspraken: wat de gebruiker vaker verbetert, wordt een vaste regel.

## Werkwijze

1. **Vraag naar het doel.** "Wat is dit project, en wat ga je hier vooral doen?" Laat de gebruiker het gewoon vertellen. Dit is het anker voor RESULTAAT.

2. **Kijk wat er al is.** Is er een map aan het project gekoppeld, of zijn er bestanden toegevoegd? Bekijk die eerst en vul CONTEXT daar zoveel mogelijk mee in. Vraag daarna alleen naar wat je niet kunt zien.

3. **Vraag per blok door, één vraag tegelijk.** Geef bij elke vraag een kort voorbeeld van een antwoord, zodat de gebruiker weet wat je bedoelt. Volgorde:
   - Voor wie is wat hier uitkomt? (EINDGEBRUIKER)
   - Zijn er vaste eisen aan vorm, lengte of toon? Is er iets wat er nooit in mag? (EISEN)
   - Heb je een voorbeeld van output die je goed vindt, en eentje die je niet goed vindt? (PRAKTIJKVOORBEELD)
   - Mag Claude in dit project bestanden maken of aanpassen? Zo ja, waar? (voor de werkafspraken)

   Zegt de gebruiker dat iets niet van toepassing is, sla het over. Weet de gebruiker het nog niet, laat het blok weg en zeg dat je het hebt weggelaten. Vul nooit iets in wat de gebruiker niet heeft gezegd.

4. **Bedenk de controlecriteria.** Neem de belangrijkste eisen op in de tweede slotregel, plus minstens één criterium dat de zwakke versie van de output ontmaskert. Voorbeeld: "de tekst werkt niet meer als je mijn naam weglaat".

5. **Toon het concept** in één kopieerblok (format hieronder). Vraag wat klopt en wat anders moet. Pas aan tot de gebruiker tevreden is.

6. **Lever de eindversie** in één kopieerblok, alleen de instructies. Zet eronder hoe ze het plakken: open het project, ga naar de instructies (Instructions) van het project, plak het blok en sla op.

## Format van het plakblok

```
RESULTAAT
[Wat er in dit project uitkomt: soort output en waar het voor dient.]

EINDGEBRUIKER
[Voor wie de output is: wat ze weten, waar ze mee zitten, waar ze aan twijfelen.]

CONTEXT
[De situatie. Welke map, bestanden of voorbeelden Claude gebruikt, en bij welke taak.]

EISEN
- [vorm en opbouw]
- [lengte]
- [toon]
- [wat er niet in mag]

PRAKTIJKVOORBEELD
Zo wel: [voorbeeld]. Waarom: [één zin]
Zo niet: [voorbeeld]. Waarom: [één zin]

WERKAFSPRAKEN
- [waar Claude bestanden opslaat, als dat mag]
- Bestaat een bestand al, dan werk je dat bestand bij in plaats van een nieuwe versie ernaast te zetten.
- Verbeter ik je op iets dat vaker terugkomt, stel dan voor om het als vaste regel toe te voegen aan deze instructies.
- Iets verwijderen doe je pas na mijn ja.

Ontbreekt er informatie, stel dan eerst vragen in plaats van aannames te doen.
Controleer je antwoord voordat je het geeft aan: [criteria]
```

## Regels

- De twee slotregels staan altijd onderaan, ook als er blokken zijn weggelaten.
- Laat weg uit de instructies: beleefdheden, dreigementen, hoofdletters voor nadruk, uitroeptekens en algemene regels die niets veranderen ("wees behulpzaam", "wees professioneel").
- Schrijf in de jij-vorm en in korte regels. Gebruik als-dan-zinnen waar dat kan ("Ontbreekt informatie, dan vraag je het").
- Werkt het project met een gekoppelde map, noem die map in CONTEXT en zet in WERKAFSPRAKEN waar output komt.
- Lever één uitwerking, geen varianten.
