# Business DNA

Zeven skills die samen jouw merk-DNA vastleggen in je eigen Notion, plus twee bonusskills.
Elk document is gebouwd op erkende marketingmodellen, niet op een losse vragenlijst.

## Wat zit erin

| Skill | Document | Modellen |
|---|---|---|
| `businessdna-setup` | controleert je omgeving | - |
| `businessdna-personal-brand` | Personal Brand | Golden Circle + 12 Merkarchetypen |
| `businessdna-ideal-client` | Ideal Client | Jobs To Be Done + Empathy Map |
| `businessdna-product-ladder` | Product Ladder | Value Ladder |
| `businessdna-brand-positioning` | Brand Positioning | STP + Blue Ocean (ERRC) |
| `businessdna-tone-of-voice` | Tone of Voice, plus optioneel een document per kanaal (salespagina's, social content, e-mails en DM's) | vier toon-dimensies |
| `businessdna-review` | controleert alle vijf in samenhang | - |

### Bonusskills

| Skill | Wat hij doet |
|---|---|
| `projectinstructies` | schrijft samen met jou de instructies voor een Claude-project, volgens RECEPT, als plakblok |
| `promptstructuur` | schrijft samen met jou een prompt volgens RECEPT (ook voor design), in één kopieerblok |

Je roept ze aan met "projectinstructies" of "schrijf een prompt". Ze staan los van de
merkdocumenten en werken ook als je Business DNA nog niet af hebt.

## Updates

Zet bij de marketplace automatisch synchroniseren aan. Verbeter ik de plugin, dan krijg je
de nieuwe versie vanzelf in Claude; je hoeft niets opnieuw te installeren.

## Zo werk je ermee

**Eenmalig vooraf:** download de Business DNA-template met de knop die je bij je
aankoop hebt gekregen, dupliceer hem naar je eigen Notion-workspace en koppel Notion
aan Claude via de connector. Roep daarna
`@businessdna-setup` aan; die controleert of alles klaarstaat en maakt de submappen in
je map CLAUDE.

Daarna roep je een skill aan met `@businessdna-personal-brand` of gewoon "personal
brand". Vindt een skill je omgeving niet, dan zet hij je eerst op het goede spoor.

Elke skill begint met twee vragen: maak je iets nieuws of vul je iets aan, en heb
je materiaal om aan te leveren. Wie veel materiaal heeft krijgt weinig vragen. Wie
niets heeft krijgt het volledige interview. Beide eindigen met hetzelfde document.

## Volgorde

De documenten lezen elkaar uit. Deze volgorde geeft het sterkste resultaat:

1. Personal Brand - staat op zichzelf
2. Ideal Client - staat op zichzelf
3. Product Ladder - leest Ideal Client
4. Brand Positioning - leest Personal Brand, Ideal Client en Product Ladder
5. Tone of Voice - leest alles, plus je echte contentvoorbeelden
6. Review - legt alle vijf naast elkaar en controleert of ze kloppen

Tone of Voice hoort als laatste. Een toonprofiel zonder klantbeeld en positionering
wordt generiek.

Tone of Voice vraagt eerst waarvoor je hem wilt vastleggen: algemeen, of ook specifiek per
kanaal. Kies je kanalen, dan krijg je naast het basisdocument een apart document per kanaal
waarin de vaste opbouwpatronen zijn uitgetekend. Die landen als subpagina's onder Tone of
Voice in Notion en als losse bestanden in `Origineel/`.

## Waar het landt

- **Notion:** de Business DNA-template in je eigen workspace, met de vijf documentpaginas.
  Elke skill vult ook de properties `Status` en `Laatst bijgewerkt` in, zodat je in één
  oogopslag ziet wat af is.
- **Bureaublad:** de map `CLAUDE`, die je zelf aanmaakt en als werkmap kiest.

```
CLAUDE/
├── Business DNA/
│   ├── Origineel/          het volledige document per skill, plus de kanaaldocumenten van Tone of Voice
│   ├── SAMENVATTING.md              alle vijf verkort, één kop per document
│   ├── MEMORY.md
│   └── README.md
└── Business Copybank/      jouw bronmateriaal in tekst
    ├── aanbod/
    ├── bedrijfsdocumenten/
    ├── emails/
    ├── klantgesprekken/
    ├── social posts/
    ├── transcripties/
    └── website teksten/
```

Beeldmateriaal (carrousels, brandfoto's, logo) hoort niet bij Business DNA. Claude Content
Studio maakt daar een eigen map Business Brand Guidelines voor aan.

`SAMENVATTING.md` is de korte versie: het bestand dat je in een andere AI-chat sleept als je niet je
hele merk-DNA wilt meesturen. De skills vullen hem niet tussentijds — hij wordt in één keer
opgebouwd als alle vijf de documenten compleet zijn. Je maakt hem met de prompt uit de les
De korte versie maken, en opnieuw na elke wijziging.
