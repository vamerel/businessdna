# Het wijzigformulier

Staat er al een Tone of Voice-document in Notion, dan begin je niet met losse vragen maar met
één formulier in de chat. Daarin kiest de gebruiker in één keer wat ze wil: aanpassen of
opnieuw maken, welke onderdelen het betreft, wat er anders moet, en ze kan meteen bestanden
toevoegen. Dat is sneller en overzichtelijker dan vier vragen na elkaar.

---

## Wanneer

1. Vind eerst de pagina, zoals in `notion-protocol.md` onder "Bij de start". Zeg nog niets.
2. Kijk welke documenten er al inhoud hebben: de basis, en de subpagina's per kanaal.
3. **Heeft de basis inhoud**, toon dan het formulier. Het vervangt de reikwijdtevraag (Fase 1),
   de vraag nieuw of aanvullen (Fase 2) en de materiaalvraag (Fase 3) in één keer.
4. **Is de pagina leeg**, dan is er niets te wijzigen. Geen formulier; begin gewoon bij Fase 1.

Het maakt niet uit hoe de gebruiker het zegt: "ik wil mijn tone of voice wijzigen",
"aanpassen", "bijwerken", "aanvullen", "opnieuw doen", of alleen "@businessdna-tone-of-voice".
Staat er een document, dan komt het formulier.

Heeft de gebruiker in haar eerste bericht al gezegd om welk onderdeel het gaat, of al
bestanden meegestuurd, toon het formulier dan toch. Het is één overzicht om te bevestigen,
en je hoeft niet te gokken wat ze nog meer wil.

---

## Hoe je het toont

Toon het formulier met `show_widget`: de tool waarmee Claude een interactief blok in de chat
zet (de visualize-tool). Lees eerst de instructies met `read_me`, met de module `elicitation`.
Zie je `show_widget` niet meteen in je lijst met tools, zoek hem dan eerst op (bijvoorbeeld met
tool search op "show_widget" of "visualize"). Pas als hij dan ook niet bestaat, kan het formulier
niet.

Gebruik hiervoor **niet** het vraagvenster met keuzeknoppen (AskUserQuestion, of "Wat wil je
aanpassen?" met genummerde opties). Daarin kiest de gebruiker maar één ding tegelijk en kan ze
geen bestanden toevoegen. Dat is precies wat dit formulier oplost.

Zet er één korte zin boven, bijvoorbeeld:

> "Je Tone of Voice staat er al. Vink hieronder aan wat je wilt, dan gaan we meteen aan de
> slag."

Neem de HTML hieronder over. De twee SVG-iconen (bovenaan en bij het uploadvak) neem je
letterlijk over, teken met de hand niets na. Verander de teksten niet zonder reden: kopers
krijgen dit formulier zo te zien.

```html
<form class="elicit">
  <div class="elicit-header">
    <svg viewBox="0 0 20 20" fill="currentColor"><path d="M11.586 2a1.5 1.5 0 0 1 1.06.44l2.914 2.914a1.5 1.5 0 0 1 .44 1.06V16.5a1.5 1.5 0 0 1-1.5 1.5h-9a1.5 1.5 0 0 1-1.492-1.347L4 16.5v-13A1.5 1.5 0 0 1 5.5 2zM5.5 3a.5.5 0 0 0-.5.5v13a.5.5 0 0 0 .5.5h9a.5.5 0 0 0 .5-.5V7h-2.5A1.5 1.5 0 0 1 11 5.5V3zm7.04 10.304a.5.5 0 0 1 .92.392c-.295.69-.871 1.304-1.66 1.304-.487 0-.892-.234-1.2-.574-.309.34-.713.574-1.2.574-.486 0-.892-.233-1.2-.574-.31.34-.714.574-1.2.574a.5.5 0 0 1 0-1c.212 0 .52-.18.74-.696l.034-.067a.5.5 0 0 1 .886.067c.221.516.528.696.74.696.213 0 .52-.18.74-.696l.035-.067a.5.5 0 0 1 .885.067c.22.516.527.696.74.696s.519-.18.74-.696m0-4a.5.5 0 0 1 .92.392c-.295.69-.871 1.304-1.66 1.304-.487 0-.892-.234-1.2-.574-.309.34-.713.574-1.2.574-.486 0-.892-.233-1.2-.574-.31.34-.714.574-1.2.574a.5.5 0 0 1 0-1c.212 0 .52-.18.74-.696l.034-.067a.5.5 0 0 1 .886.067c.221.516.528.696.74.696.213 0 .52-.18.74-.696l.035-.067a.5.5 0 0 1 .885.067c.22.516.527.696.74.696s.519-.18.74-.696M12 5.5a.5.5 0 0 0 .5.5h2.293L12 3.207z"/></svg>
    <span>Tone of Voice wijzigen</span>
  </div>
  <div class="elicit-body">
    <div class="elicit-group">
      <label class="elicit-question">Wat wil je doen met je Tone of Voice?</label>
      <div class="elicit-pills" data-name="actie" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Aanpassen" style="border-radius:12px; padding:14px 16px; display:flex; gap:12px; align-items:flex-start; text-align:left; min-width:200px; box-shadow:0 1px 2px rgba(0,0,0,0.04)">
          <i class="ti ti-pencil" style="font-size:20px" aria-hidden="true"></i>
          <span><span style="font-size:13px; font-weight:500">Aanpassen</span><br><span style="font-size:11px; color:var(--text-muted)">Bestaande tekst bijwerken</span></span>
        </button>
        <button type="button" class="elicit-pill" data-value="Opnieuw maken" style="border-radius:12px; padding:14px 16px; display:flex; gap:12px; align-items:flex-start; text-align:left; min-width:200px; box-shadow:0 1px 2px rgba(0,0,0,0.04)">
          <i class="ti ti-refresh" style="font-size:20px" aria-hidden="true"></i>
          <span><span style="font-size:13px; font-weight:500">Opnieuw maken</span><br><span style="font-size:11px; color:var(--text-muted)">Vanaf nul, oude versie blijft bewaard</span></span>
        </button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Welke onderdelen gaat het om? Je mag er meer aanvinken.</label>
      <div class="elicit-pills" data-name="onderdelen" data-multi="true">
        <button type="button" class="elicit-pill" data-value="Algemeen (basis)" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)">
          <i class="ti ti-message-circle" style="font-size:18px" aria-hidden="true"></i>
          <span><span style="font-size:13px; font-weight:500">Algemeen</span><br><span style="font-size:11px; color:var(--text-muted)">Je basisstem</span></span>
        </button>
        <button type="button" class="elicit-pill" data-value="Social content" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)">
          <i class="ti ti-brand-instagram" style="font-size:18px" aria-hidden="true"></i>
          <span><span style="font-size:13px; font-weight:500">Social media</span><br><span style="font-size:11px; color:var(--text-muted)">Incl. stijlvoorbeelden</span></span>
        </button>
        <button type="button" class="elicit-pill" data-value="Salespaginas" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)">
          <i class="ti ti-file-text" style="font-size:18px" aria-hidden="true"></i>
          <span><span style="font-size:13px; font-weight:500">Salespagina's</span><br><span style="font-size:11px; color:var(--text-muted)">Verkoopteksten</span></span>
        </button>
        <button type="button" class="elicit-pill" data-value="E-mail en DM" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)">
          <i class="ti ti-mail" style="font-size:18px" aria-hidden="true"></i>
          <span><span style="font-size:13px; font-weight:500">E-mails en DM's</span><br><span style="font-size:11px; color:var(--text-muted)">Nieuwsbrief, berichten</span></span>
        </button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Wat wil je anders? Vertel het in je eigen woorden.</label>
      <textarea class="elicit-textarea" data-name="toelichting" placeholder="Mijn posts klinken nog te formeel, ik wil dat het luchtiger wordt en meer zoals ik praat"></textarea>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Heb je voorbeelden die ik mag gebruiken? Denk aan teksten die wel of juist niet als jou klinken.</label>
      <div class="elicit-files" data-name="voorbeelden">
        <label class="elicit-dropzone">
          <svg viewBox="0 0 20 20" fill="currentColor"><path d="M16.5 13a.5.5 0 0 1 .5.5v2a1.5 1.5 0 0 1-1.5 1.5h-11A1.5 1.5 0 0 1 3 15.5v-2a.5.5 0 0 1 1 0v2a.5.5 0 0 0 .5.5h11a.5.5 0 0 0 .5-.5v-2a.5.5 0 0 1 .5-.5M10 3a.5.5 0 0 1 .374.168l4 4.5.059.082a.5.5 0 0 1-.732.65l-.075-.068L10.5 4.814V13.5a.5.5 0 0 1-1 0V4.814L6.374 8.332a.5.5 0 0 1-.748-.664l4-4.5.08-.071A.5.5 0 0 1 10 3"/></svg>
          <span>Kies bestanden</span>
          <input type="file" multiple>
        </label>
      </div>
      <textarea class="elicit-textarea" data-name="voorbeelden_text" placeholder="of plak hier een tekst of een link naar een post"></textarea>
    </div>
  </div>
  <div class="elicit-footer">
    <button type="button" class="elicit-skip">Liever in de chat</button>
    <button type="button" class="elicit-submit">Ga verder</button>
  </div>
</form>
```

---

## Wat je met de antwoorden doet

De antwoorden komen als één bericht binnen. Zet ze zo om:

| Antwoord | Wat je doet |
|---|---|
| **Aanpassen** | De route "aanvullen": je loopt alleen de aangevinkte onderdelen langs. Per onderdeel laat je eerst zien wat er nu staat, en werk je bij met de toelichting en het nieuwe materiaal. Wat niet is aangevinkt, blijft zoals het is. |
| **Opnieuw maken** | De route "nieuw" voor de aangevinkte onderdelen. Bewaar het oude eerst als kopie, zoals in `notion-protocol.md` onder "Nieuw" staat, zonder dat opnieuw te vragen: het formulier belooft dat de oude versie bewaard blijft. |
| **Onderdelen** | Dit is de reikwijdte uit Fase 1. Algemeen is de basis, de andere drie zijn de kanaalmodules. Social media omvat ook het document met de vijf stijlvoorbeelden. |
| **Toelichting** | Je startpunt per onderdeel. Wat ze hier schrijft, hoef je niet nog eens te vragen. |
| **Bestanden en geplakte tekst** | Dit is het materiaal uit Fase 3. Bestanden staan als bijlage in het gesprek; lees ze zoals elk ander aangeleverd bestand. Kijk daarnaast zelf in `CLAUDE/Business Copybank/`, zoals altijd. |

Daarna vervolg je de skill vanaf Fase 4, met deze keuzes als vaststaand. Vraag ze niet
opnieuw.

**Ontbreekt er iets in het antwoord**, vraag dan alleen dat ene in tekst:

- Geen actie gekozen: "Wil je het aanpassen of opnieuw maken?"
- Geen onderdeel aangevinkt bij aanpassen: "Om welk onderdeel gaat het: algemeen, social
  media, salespagina's of e-mails en DM's?"
- Geen toelichting bij aanpassen: begin bij het eerste aangevinkte onderdeel, laat zien wat er
  staat en vraag wat er anders moet.
- Geen materiaal: geen probleem bij een kleine aanpassing. Bij opnieuw maken geldt wat in
  Fase 3 staat: voor dit document zijn echte teksten nodig.

**Social content niet aangevinkt, en er is nog geen social-document**, geef dan één keer de
waarschuwing uit Fase 1 over de caption-skill. Zegt ze nee, kom er niet op terug.

**Kiest ze een kanaal dat nog geen eigen document heeft**, dan is dat kanaal nieuw, ook als ze
"aanpassen" koos. Zeg dat in één zin en bouw het op.

**Bij het voorleggen in Fase 8** (na aanpassen): laat de gewijzigde documenten en secties
volledig zien en noem de rest bij naam als ongewijzigd. Weggeschreven wordt altijd het
volledige document, zoals in `notion-protocol.md` staat.

---

## Als het formulier niet kan

**"Liever in de chat"** — ga door met de gewone volgorde: Fase 1, Fase 2 en Fase 3, elke vraag
apart.

**Bestaat `show_widget` niet**, ook niet na zoeken, stel dan dezelfde vragen in één bericht,
als tekst. Ook dan niet via het vraagvenster met keuzeknoppen:

> "Je Tone of Voice staat er al. Vertel me in één keer:
>
> 1. Wil je hem **aanpassen** of **opnieuw maken**? (Opnieuw maken: de oude versie blijft
>    bewaard.)
> 2. Om welke onderdelen gaat het? **Algemeen**, **social media**, **salespagina's**,
>    **e-mails en DM's**. Meer mag.
> 3. Wat wil je anders?
> 4. Heb je voorbeelden? Sleep ze in dit gesprek of plak ze hieronder."

Noem nooit dat er een formulier had moeten komen. De gebruiker merkt alleen dat het in één
keer gaat.
