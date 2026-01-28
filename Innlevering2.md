{% include top-box.html %} <!-- Kode for å inkludere boksen på toppen av siden. Se _config.yml for å gjøre endringer. -->
{% include navbar.html %} <!-- Kode for navigasjonsmeny. Se navbar.html for å gjøre endringer. -->
<!-- Gjør endringer under her -->

# Utfordring 1
## Generell informasjon
- Innleveringen skal skje individuelt
- **Fristen for innlevering er:**
- Innleveringen kan gi maks tre poeng 
- For å kvalifisere til poeng må dere ha prøvd å løse alle oppgavene. Innleveringer med blanke svar vil ikke bli evaluert.
- De ulike deloppgavene teller nødvendigvis ikke likt til totalpoeng.
- Oppgaven skal leveres inn skriftlig i Canvas.
- **NB! Filen skal ha navn med følgende struktur: kandidatnrstudent1_utf1.pdf (eller docx)**
- Oppgaven skal leveres som word-fil eller pdf-fil. Filer som ikke er rendret vil behandlet som blank innlevering.
- Koden skal leveres i et separat dokumentet (qmd-fil er ok) eller som appendiks til oppgaven.
- Husk KI-erklæring.
- Du vil få mulighet å jobbe med oppgavene på et utfordringsseminar knyttet til temaet. Foreleseren på kurset vil være tilstede for å svare på spørsmål. 

## Førberedelser og støtte

For å gjennomføre utfodring 1 må du hente data fra Arbeidskraftsundersøkelsen (AKU) 3. kvartal 2025 på [Surveybanken](https://sikt.no/surveybanken). Du har fått tilgang til datamaterialet fra Sikt. For å bruke datamaterialet må du lage deg en bruker på Sikt og signere avtalen som du finner under "Min forskning". Når du har signert avtalen vil du kunne laste ned data.  

**NB: Du må følge avtalen i din bruk av data. Dette betyr at du ikke får laste opp datamaterialet til KI-verktøy eller dele det med andre mennesker. Du er selv ansvarlig for bruken av data**. Spør oss gjerne hvis du lurer på hva du har lov og ikke lov å gjøre med data.

Litteratur:

- Barr. Kapittel 3, 4 og 9-11
- Boeri og van Ours. Kapittel 1 og 7

[Forelesningsnotater](forelesninger.md#f_t1)

[Videoer](video.md#v_t1)

## Oppgaver
### Utfordring 1.1
Hvert kvartal samler Statistisk sentralbyrå (SSB) inn informasjon om arbeidskraften via Arbeidskraftsundersøkelsen (AKU). AKU 3. kvartal 2025 inneholder svar fra 14841 personer. Din utfordring består i å bruke data fra AKU 3. kvartal 2025 til å bruke økonomisk teori til å analysere menn og kvinners arbeidstimer og deltakelse i arbeidsstyrken. 

**A.** Tegn to figurer som viser hvordan valget av fritid og konsum henger sammen med individets preferanser. Grafene skal vise optimalt valg for 1) kvinner og 2) menn. Gå ut ifra at menn og kvinner har lik timelønn, men at kvinner av en eller annen grunn verdsetter tid med familien ("fritid") mer enn menn. Analyser forskjeller i menn og kvinners optimale valg av arbeid og fritid. Gå ut ifra at markedet er perfekt og at menn og kvinner kan velge arbeidstimer fritt.

**NB: Oppgaven skal innholde figurer tegnet for hånd, og figurer tegnet "digitalt" (ved bruk av tegningsverktøy eller script)**

**B.** Lag to grafer med empiriske data:

Graf 1: Fordeling av arbeidstimer for menn og kvinner som har arbeid (er sysselsatte). Bruk variabelen "hwactual" for å måle antall arbeidstimer (noter at denne variabelen er målt i antall arbeidstimer x 10). Bruk variabelen "ilostat" for å identifisere personer som er sysselsatt. Bruk variabelen "sex" for å identifisere menn og kvinner. Bruk variabelen "alder_periode_nr" til å dele inn deltakerne i tre aldersgrupper: 1) "Under 30 år", 2) "30 - 49 år", 3) "Eldre enn 50" og lag grafen slik at den viser fordelingen av arbeidstimer for disse tre gruppene (bruk f.eks "facet_wrap()"funksjonen i R-studio).  

Graf 2: Andel menn og kvinner som deltar i arbeidsstyrken. Bruk variabelen "ilostat" for å identifisere personer i arbeidsstyrken. Bruk variabelen "sex" for å identifisere menn og kvinner. NB: Her trenger du ikke å dele opp deltakerne i ulike aldersgrupper.  

Diskutter i hvilken grad dine teoretiske prediksjoner ser ut å være forenlig med det du ser i data.

### Utfordring 1.2
Dette [datasettet](https://github.com/uit-sok-2303-V2026/uit-sok-2303-V2026.github.io/blob/main/assets/women.csv) inneholder informasjon om generøsiteten av foreldrepermisjonsordninger og mødres yrkesdeltakelse i 24 OECD land i 2021. For å gjøre ulike lands rettigheter sammenlignbare presenteres permisjonsordningenes gunstighet ved hjelp av «full rate equivalent» (tot_full_rate = uker med 100% støtte), hvilket tilsvarer foreldrepermisjonens varighet i uker multiplisert med utbetalingssats i prosent av gjennomsnittlig inntekt. 

Bruk datasettet til å lage to diagrammer som viser sammenhengen mellom lengde på betalt foreldrepermisjon og yrkesdeltakelse blant kvinner. I det ene diagrammet skal du bruke data som beskriver sysselsetting blant kvinner med barn i alderen 0-2 år (fem_emp_rate_0_2), og det andre skal du bruke data på kvinner med barn i alderen 6-14 år (fem_emp_rate_6_14). 

Diskuter, basert på disse diagrammene og økonomisk teori, følgende påstand: *«Gunstige permisjonsordninger ved fødsel sikrer høy yrkesdeltakelse blant kvinner på lang sikt»*.

Forklar hvorfor høy yrkesdeltakelse blant norske kvinner og høye barnetall er viktig for at den norske velferdsmodellen skal være økonomisk bærekraftig.

### Utfordring 1.3
I en situasjon med økende kostnader i helsetjenesten og strammere offentlige budsjetter blir høyere egenandeler ofte diskutert som et virkemiddel for å påvirke etterspørselen etter helsetjenester og redusere atferdsrisiko (moral hazard). I denne oppgaven skal du analysere utviklingen i bruken av fastlegetjenester i Norge og drøfte hvordan egenandeler kan påvirke forbruket av helsetjenester.

**A.** Lag en figur som viser utviklingen i antall fastlegekonsultasjoner per innbygger i perioden 2012–2024 ved hjelp av SSB-tabell 10141. Beskriv utviklingen du observerer. Analyser hvilke diagnosegrupper som ser ut til å bidra mest til endringene i det totale antallet fastlegekonsultasjoner over tid.

**B.** Bruk økonomisk teori om atferdsrisiko fra forelesninger og pensum til å forklare hvordan økte egenandeler påvirker etterspørselen etter helsetjenester. Illustrer forklaringen grafisk ved hjelp av tilbuds- og etterspørselsdiagrammer eller andre relevante figurer. Vis også, ved hjelp av figurer, hvordan en økning i egenandelen kan påvirke forbruket forskjellig på tvers av ulike diagnosegrupper (for eksempel akutte vs. mindre alvorlige tilstander).

**C.** Bruk økonomisk teori til å diskutere fordelingseffekter av økte egenandeler. Hvem rammes relativt sett hardest, og hvorfor? Drøft hvordan høyere egenandeler kan påvirke arbeidsevne og yrkesdeltakelse i befolkningen, både på kort og lang sikt.



### Evaluering av utfordringer
Utfordringene blir bedømt i henhold til regelen i Tabell 1. Det vil være mulig å få halve og hele poeng på utfordringene. Hver innlevering kan gi maks tre poeng.

**NB: Hver utfordring består av flere deloppgaver. Alle deloppgavene må besvares. Hvis minst én av deloppgavene ikke er besvart, eller er besvart svært ufullstendig eller feilaktig, er det fullt mulig å få null poeng på innleveringen.**

**Tabell 1.** Regel for poengsetting av innleveringsoppgaver
<table>
  <tr>
    <th>Poeng</th>
    <th>Beskrivelse</th>
  </tr>
  <tr>
    <td>3</td>
    <td>
      <ul>
        <li>Oppgaven inneholder korrekte eller veldig nært korrekte løsninger på alle deloppgaver.</li>
        <li>Dersom det er feil og mangler, er disse små og uviktige.</li>
        <li>Oppgaven er veldig godt skrevet og strukturert, og det er veldig enkelt å lese oppgaven og forstå innholdet.</li>
        <li>Du viser at du har veldig god forståelse for hva du har gjort.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>2</td>
    <td>
      <ul>
        <li>Oppgaven inneholder løsninger på alle deloppgaver, og de fleste løsningene er korrekte eller veldig nært korrekte.</li>
        <li>Det er noen feil i noen løsninger, men disse er ikke fundamentale (vitner ikke om store mangler i forståelse).</li>
        <li>Oppgaven er godt skrevet og strukturert, og det er enkelt å lese oppgaven og forstå innholdet.</li>
        <li>Du viser at du har god forståelse for hva du har gjort i de fleste oppgavene. Det er ikke tegn på at du har alvorlige mangler i forståelse.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>1</td>
    <td>
      <ul>
        <li>Oppgaven inneholder løsninger på alle deloppgaver, men...</li>
        <li>Noen av løsningene har feil som vitner om alvorlig mangel i forståelse, eller...</li>
        <li>Det er vanskelig å lese og forstå hva du har gjort.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>0</td>
    <td>
      <ul>
        <li>Oppgaven mangler løsninger på noen oppgaver, eller...</li>
        <li>Flere av løsningene vitner om alvorlige mangler i forståelse.</li>
        <li>Det går ikke an å følge hva studentene gjør og hvorfor, eller...</li>
        <li>Kode og/eller bruk av KI blir ikke gjort rede for.</li>
      </ul>
    </td>
  </tr>
</table>

### Plagiat og juks

Det er tillatt å arbeide med oppgavene sammen med andre, men hver gruppe skal produsere sin egen tekst, figurer, koder og så videre. Det er ikke lov å levere inn tekster som er produsert av KI. Vi bruker URKUND for å sjekke for plagiering. 

### Bruk av kunstig intelligens (KI)
Hver innlevering **skal** inneholde en deklarasjon om bruk av KI. Deklarasjonen skal settes inn i et appendiks til oppgaven. **Du må ha med deklarasjonen selv om du ikke har brukt KI**. Dersom dere bruker kunstig intelligens for å løse oppgaven skal dere oppgi hvilken KI dere brukte. Dere er selve ansvarlige for de tekster leverer inn. 

### Tips og triks for hvordan du skriver en god besvarelse

#### Generelle tips

1. Skriv kortfattet og tydelig
2. Gå gjennom språket. Oppgaven skal skrives på godt akademisk språk, ikke i taleform.
3. Ha samme inndeling på ditt svar som det er i oppgaven.
4. Det er lov å bruke bilder på håndtegnede grafer og ligninger men jeg anbefaler å prøve å lage både ligninger og grafer digitalt. Hvis du bruker håndtegnede grafer eller ligninger, se til at både grafen i seg selv, og bildet av grafen er svært tydelig. Hvis jeg ikke kan se hva grafen viser kan jeg ikke gi poeng. 
5. Definere dine symboler hvis du bruker andre symboler enn de vi bruker under kurset.
6. Referere i teksten til de symboler som du analyserer, og beskriv dem i ord. F eks, en økning i arbeidstilbudet ($L^s$) fører til at…
7. Forklare dine ligninger og utledninger. Det er viktig at det går å følge dine utledninger og beregninger. 
8. Gi alltid samfunnsøkonomisk forklaring til dine svar. Det å skrive "Kurven skifter og vi går fra A til B" er ikke tilstrekkelig. Du skal forklare mekanismene i samfunnsøkonomiske termer, f eks.; "Hvis innvandringen øker vil dette føre til at mengden arbeidere som er villige til å jobbe til en gitt timelønn øker, arbeidstilbudet ($L^s$) øker. Ved likevektslønna $w_0$ finnes det nå arbeidere som ønsker jobb men som ikke har jobb. Dette fører til en press ned på lønna. Når lønna synker finnes det flere bedrifter som er villige å ansette. Sysselsettingen øker. Den nye likevektslønna gis av $w_1$. Sysselsettingen i den nye likvekten gis av $L_1$" 

#### Format
Du velger selv i hvilket format du ønsker å lage oppgaven. Det er lov å bruke Word, eller andre standard ordbehandlingsprogrammer. Dersom du ønsker å skrive oppgaven i Quarto finner du støtte til dette [her](https://quarto.org/).

#### Ligninger
Det er mulig å skrive ligninger i Quarto og de fleste ordbehandlingsprogrammer.  

#### Figurer og grafer
Det går an å lage figurer ved bruk av en rekke verktøy, f.eks RStudio og Python. Det er lov å tegne figurer i ved bruk av f.eks Word eller Power-point. Vår erfaring er at Power-point er bedre enn Word. Når du har laget en graf i Power-point kan du enten lagre denne som et bilde ved å høyre-klikke på den, eller kopiere den direkte og lime inn den som et bilde (lime inn spesial) i Word.

#### Tabeller
Det går an å lage tabeller ved bruk av en rekke verktøy, f.eks. Excel, Python og R. Det går å kopiere tabeller fra Excel og R og lime inn i Word. Hvis du er flink i f eks LaTeX så går det å skrive kode i R som lager TeX filer. 

#### Referanser
Hvis du bruker materiale utenfor pensum skal du bruke referanser, både i teksten, og i en referanseliste. Referanser i tekst skal inneholde etternavn på forfatter og år. Hvis det er flere enn to forfatter er det lov å bruke «et al». Det finnes to forskjellige måten å skrive referanser i tekst. Iblant henviser vi til en studie i teksten, f eks at Acemoglu et al (2001) fant at land en signifikant lenke mellom kolonial historie og nåværende økonomisk vekst. Et annet måte er å skrive at det ser ut å va en lenke mellom kolonial historie og nåværende økonomisk vekst (Acemoglu et al, 2001). Lengst ned i dokumentet skriver du en referanseliste. I Tabell 2 her nede ser du hvordan du refererer til ulike typer av skrevet materiale. 
 
**Tabell 2.** Referanser

| Type                             | Referanse |
|----------------------------------|-----------|
| Vitenskapelige artikler og working-papers | Acemoglu, D., Johnson, S., and Robinsom, J. (2001). The Colonial Origins of Comparative Development: An Empirical Investigation. *American Economic Review*, 91(5), pp. 1369-1401 |
| Bøker                            | Lucas, R. E. (1976). Econometric Policy Evaluation: A Critique, in Brunner, K., and Metzer, A (eds), *The Phillips Curve and Labor Markets*, Carnegie Rochester Conference Series, New York, North Holland, pp. 19-46 |
| Artikler i aviser                | Weisman, J. (2015). Deal Reached on Fast-Track Authority for Obama on Trade Accord. *The New York Times*, p.A1 |
| Artikler fra Internett           | Messer, L. (2015). 'Fancy Nancy' Optioned by Disney Junior. [online] ABC News. Available at: [http://abcnews.go.com/Entertainment/fancy-nancy-optioned-disney-junior-2017/story?id=29942496#.VRWbWJwmbs0.twitter](http://abcnews.go.com/Entertainment/fancy-nancy-optioned-disney-junior-2017/story?id=29942496#.VRWbWJwmbs0.twitter) (Accessed 31 Mar. 2015)|
