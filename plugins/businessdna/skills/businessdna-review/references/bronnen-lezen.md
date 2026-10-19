# De documenten ophalen

Deze skill leest de vijf merkdocumenten. Hij schrijft er nooit in — niet in Notion en niet
lokaal. Dat is het verschil met de vijf documentskills.

---

## Waar de documenten staan

Op twee plekken, en die kunnen uiteenlopen:

1. **Notion**, op de pagina **Business DNA**, vijf subpagina's of databaseregels
2. **Lokaal**, in `CLAUDE/Business DNA/Origineel/` — één `.md`-bestand per document

**Notion is leidend.** Daar wordt bewerkt, dus daar staat de meest recente versie. Gebruik
lokaal alleen als terugval.

Lopen ze uiteen, dan is dat zelf een bevinding (zwaarte: signaal). Vermoedelijk is er
handmatig in Notion gewerkt zonder de lokale kopie bij te werken, of andersom.

---

## De pagina vinden

1. Zoek in Notion de pagina **Business DNA**.
2. Kijk wat eronder hangt. Is het een database, kijk daarin; zijn het subpagina's, kijk daar.
3. Haal alle vijf op: Personal Brand, Ideal Client, Product Ladder, Brand Positioning,
   Tone of Voice.
4. Kijk of er onder **Tone of Voice** kanaalsubpagina's hangen (`Tone of Voice - Salespaginas`,
   `Tone of Voice - Social content`, `Tone of Voice - Social content - voorbeelden`,
   `Tone of Voice - E-mail en DM`). Zijn die er, haal ze
   dan ook op en lees ze als onderdeel van Tone of Voice. Zijn ze er niet, dan is dat geen
   bevinding: ze zijn optioneel.

Zoek nooit rechtstreeks op een documentnaam zonder eerst Business DNA te vinden. Een gebruiker
kan elders in haar workspace een pagina met dezelfde naam hebben.

Vergelijk namen hoofdletterongevoelig: in de template kan een pagina net anders geschreven
staan (bijvoorbeeld "Tone Of Voice"). Dat is dezelfde pagina. Hernoem hem niet.

Noteer per document de datum van laatste wijziging. Eén document dat veel ouder is dan de
rest, is de eerste plek om naar veroudering te kijken.

---

## Geen verbinding met Notion

Val terug op de lokale map en meld het:

> "Ik heb geen verbinding met Notion, dus ik lees je documenten uit de lokale map
> `CLAUDE/Business DNA/Origineel/`. Als je daarna nog in Notion hebt gewerkt, zie ik dat niet
> — houd daar rekening mee bij wat ik straks meld."

Staan ze lokaal ook niet, dan stopt het hier:

> "Ik kan je Business DNA nergens vinden — niet in Notion, en niet in de map
> `CLAUDE/Business DNA/Origineel/` op je bureaublad.
>
> Wil je dat ik je omgeving controleer met @businessdna-setup?"

---

## Business DNA niet gevonden

> "Ik zie nog geen Business DNA-omgeving. Er valt dan ook nog niets te controleren."

Roep `businessdna-setup` aan als de gebruiker dat wil, en stop daarna. Een review van lege
documenten heeft geen zin.

---

## Een of meer documenten ontbreken

De review draait wel, maar met minder controles. Meld vóór je begint welke wegvallen:

> "Ik mis **[naam]**. Ik kan de review wel doen, maar dan vallen deze controles weg:
>
> - [de belangrijkste kruisverbanden die dit document nodig hebben]
>
> Wil je [naam] eerst afmaken met @businessdna-[skill], of ga ik door met wat er staat?"

Welke kruisverbanden per document wegvallen:

| Ontbreekt | Vervalt |
|---|---|
| Personal Brand | 5, 6, 7, 10 |
| Ideal Client | 1, 2, 3, 4, 9 |
| Product Ladder | 1, 8, 9, 10 |
| Brand Positioning | 2, 5, 6, 8, 10 |
| Tone of Voice | 3, 4, 7 |

De interne controles van de overgebleven documenten doe je gewoon.

---

## Een document is er wel, maar is nauwelijks ingevuld

Behandel het als aanwezig en meld het als **gat**, per sectie. Een document met drie van de
acht secties ingevuld levert echte bevindingen op over de secties die er wel zijn.

Zeg wel vooraf wat je ziet:

> "Je [naam] is er, maar drie van de [aantal] secties zijn nog leeg. Ik neem mee wat er staat
> en meld de lege secties als gaten."

---

## Wat je nooit doet

- In Notion schrijven, ook geen properties zoals `Status` of `Laatst bijgewerkt`.
- Een lokaal bestand aanmaken, wijzigen of verplaatsen.
- Een ontbrekende pagina aanmaken. Dat doet `businessdna-setup`.
- `SAMENVATTING.md` lezen als bron. Dat is de verkorte versie; je controleert de originelen.
