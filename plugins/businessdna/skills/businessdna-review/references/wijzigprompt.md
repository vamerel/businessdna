# De wijzigprompt

Het eindproduct van de review. Eén blok tekst dat de gebruiker plakt in haar project
**WIJZIGINGEN BUSINESS DNA** — de enige plek waar de vijf merkdocumenten aangepast worden.

---

## De eis waar alles op neerkomt

De prompt wordt gelezen in een sessie die dit gesprek niet heeft meegemaakt. Daar is geen
review, geen analyse en geen context. Alles wat nodig is om de wijziging correct door te
voeren, moet dus in de prompt zelf staan.

Toets voor je hem oplevert: **kan iemand die dit gesprek niet kent hiermee vooruit?** Staat er
"pas de kernwaarden aan zoals besproken", dan is het antwoord nee.

---

## Opbouw

Altijd in één codeblok, zodat de gebruiker hem in zijn geheel kan kopiëren.

```markdown
# Wijzigingen Business DNA — [datum]

Deze wijzigingen komen uit een review van de vijf merkdocumenten. Voer ze door in Notion en in
de lokale map `CLAUDE/Business DNA/Origineel/`. Leg elke wijziging voor voor je hem opslaat.

## 1. [Document] — [sectie]

**Nu:** [het letterlijke citaat zoals het er staat]

**Wordt:** [de nieuwe tekst, of als die nog niet vaststaat: de richting plus wat er moet
gebeuren om hem te bepalen]

**Waarom:** [de reden, in één of twee zinnen — inclusief waarmee het botste]

## 2. [Document] — [sectie]

...

---

Na het doorvoeren: draai @businessdna-review opnieuw om te controleren of er niets is
losgeraakt.
```

---

## Per wijziging drie velden

**Nu** — het letterlijke citaat. Nooit een parafrase. De sessie die dit uitvoert moet de plek
kunnen terugvinden en zeker weten dat hij de juiste tekst te pakken heeft.

Is de wijziging een toevoeging en staat er dus nog niets, schrijf dan: *"Nu: deze sectie
bevat hier nog niets."*

**Wordt** — bij voorkeur de volledige nieuwe tekst, zoals besproken en goedgekeurd tijdens de
review. Kwam die er niet uit, geef dan de richting én wat er nodig is om hem te bepalen:

> **Wordt:** een uitzonderingsregel bij het verbod op "meedenken", die vastlegt dat het woord
> wel gebruikt mag worden in citaten van klanten. De precieze formulering nog bepalen samen
> met de gebruiker.

**Waarom** — de reden uit het gesprek. Twee dingen horen erin: waarmee het botste (met
documentnaam), en wat het gevolg was. Zonder het waarom voert de volgende sessie een wijziging
door zonder te kunnen beoordelen of hij het goed doet.

---

## Volgorde

Groepeer per document, en zet de documenten in de vaste ketenvolgorde:

Personal Brand → Ideal Client → Product Ladder → Brand Positioning → Tone of Voice

Zo hoeft de uitvoerende sessie elk document maar één keer open te slaan.

Raakt één wijziging twee documenten (bij een botsing vaak het geval), zet hem dan bij het
document dat daadwerkelijk verandert, en noem het andere document in het waarom.

---

## Wat er niet in hoort

- Bevindingen waar geen besluit over genomen is. Die blijven staan; meld ze los aan de
  gebruiker, buiten de prompt.
- Jouw analyse, de controlelijst, of hoe je tot de bevinding kwam. Alleen wat er moet
  veranderen en waarom.
- Suggesties die tijdens het gesprek zijn afgewezen.
- Complimenten of samenvattingen. Het is een werkopdracht.

---

## Wat je erbij zegt

Onder het codeblok, altijd:

> "Plaats deze prompt in je project **WIJZIGINGEN BUSINESS DNA**. Dat is de enige plek waar de
> vijf documenten aangepast mogen worden — overal anders is je Business DNA alleen-lezen."

Bleven er bevindingen zonder besluit over, noem ze daar direct onder:

> "Deze heb ik er niet in gezet, omdat we er nog geen besluit over namen:
>
> - [bevinding]
> - [bevinding]
>
> Ze blijven staan zoals ze nu zijn. Wil je er alsnog naar kijken?"
