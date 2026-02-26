{% include top-box.html %} <!-- Kode for å inkludere boksen på toppen av siden. Se _config.yml for å gjøre endringer. -->
{% include navbar.html %} <!-- Kode for navigasjonsmeny. Se navbar.html for å gjøre endringer. -->
<!-- Gjør endringer under her -->

# Utfordring 2
## Generell informasjon
- <span style="color:OrangeRed;"> Fristen for innlevering er: </span>
- Innleveringen kan gi maks tre poeng 
- For å kvalifisere til poeng må dere ha prøvd å løse alle oppgavene. Innleveringer med blanke svar vil ikke bli evaluert.
- De ulike deloppgavene teller nødvendigvis ikke likt til totalpoeng.
- Oppgaven skal leveres inn skriftlig i Canvas.
- **NB! Filen skal ha navn med følgende struktur: [ditt kandidatnummer]sok_2008_h24_utf2.pdf (eller docx)**
- Oppgaven skal leveres som word-fil eller pdf-fil. Filer som ikke er rendret vil behandlet som blank innlevering.
- Koden skal leveres i et separat dokumentet (qmd-fil er ok) eller som appendiks til oppgaven.
- Bruk av KI skal rapporteres i en appendiks til oppgaven. Sjekk at eventuelle lenker fungerer.
- Du vil få mulighet å jobbe med oppgavene på et utfordringsseminar knyttet til temaet. Foreleseren på kurset vil være tilstede for å svare på spørsmål.

**Førberedelser og støtte:**
Kode:
-  [Hjelpe-dokument for å lage figurene R](https://uit-sok-2008-h24.github.io/assets/Utf2_kodehjelp.R)
  
Litteratur:

- Boeri og van Ours. Kapittel 2 og 3
- NOU 2021:9

[Forelesningsnotater](forelesninger.md#f_t1)

[Videoer](video.md#v_t1)

# Oppgaver

## Utfordring 2.1 - Minstelønn
I Norge har vi ikke minstelønninger, men kollektivavtalene setter i praktikken lønnsgulv på arbeidsmarkedet. Hvis vi er litt raus med begrepene kan vi tolke disse lønnsgulvene som minstelønninger. 


### 2.1.1 Teoretisk analyse

Samfunnsøkonomer er ikke enige om det å innføre et lønnsgulv er en god eller dårlig idé. Noen mener at **minstelønninger fører til økt fattigdom**, mens andre mener at **minstelønninger fører til mindre fattigdom**. Bruk grafisk analyse til å vise at begge disse påstandene kan være riktig i henhold til økonomisk teori. Vær nøye med å gjøre rede for dine antakelser og gi økonomisk intusijon. 

 - Besvarelsen skal innholde figurer som er tegnet for hånd (med fysisk eller digital penn), og figurer som er tegnet ved bruk av et program (f.eks. power-point, R-studio, Python).
 
#### 2.1.2 Empirisk analyse

1. Bruk data fra Arbeidskraftsundersøkelsen (AKU 3. kvartal 2025) til å lage én graf som viser andelen arbeidsledige i aldersgruppene: 15 - 24 år, 25 - 34 år, 35 - 44 år, 45 - 54 år, og over 55 år). 

2. Bruk t-test til å evaluere om det er en signifikant forskjell i gjennomsnittlig alder mellom arbeidsledige og sysselsatte. 

3. Hvis du ønsker (tas ikke med i vurderingen av oppgaven) kan du kjøre en regresjon der du tester om alder har en innvirkning på sannsynligheten å være arbeidsledig når vi kontrollerer for utdanning. Du kan bruke en vanlig linjer modell. I dette tilfellet blir modellen en linjer sannsynlighetsmodell. For å estimere modellen må du først lage en variabel tar verdien 1 hvis individet er arbeidsledig, og 0 hvis det er sysselsatt (bruk kun personer som deltar på arbeidsmarkedet). Du kan enten bruke alder som kategori-variabel eller som kontinuerlig variabel (alder_periode_nr). For å inkludere utdanning i analysen kan du bruke variabelen hatlevel_sikt. Denne variabelen har mange kategorier. Vi foreslår at du lager 4 kategorier: 

* hatlevel_sikt == 1 | hatlevel_sikt == 0 | hatlevel_sikt == 10 | hatlevel_sikt == 20 ~ "Lavere enn videregående",

* hatlevel_sikt == 34  | hatlevel_sikt == 35 ~ "Videregående",

* hatlevel_sikt == 45 |  hatlevel_sikt == 55 ~ "Folkhøyskole eller yrkesskole",

* hatlevel_sikt == 54 | hatlevel_sikt == 60 | hatlevel_sikt == 70 | hatlevel_sikt == 80  ~ "Universitetsutdanning"

Til sist kan du, hvis du ønsker, inkludere kjønn som forklaringsvariabel. 

**Diskutter dine empiriske observasjoner ved bruk av økonomisk teori.** 


### Utfordring 2.2 - Fagforeninger

#### 2.2.1 - Teoretisk analyse

Bruk økonomisk teori og grafisk analyse til å evaluere påstanden «Sterke fagforeninger reduserer velferden». Gjør rede for dine antakelser og gi økonomisk intusijon. 

 - Besvarelsen skal innholde figurer som er tegnet for hånd (med fysisk eller digital penn), og figurer som er tegnet ved bruk av et program (f.eks. power-point, R-studio, Python).

#### 2.2.2 - Empirisk analyse

OECD har informasjon om organisasjonsgraden i fagforeninger (union density) og arbeidsledighetsraten i ulike land. Din utfordring består i å analysere sammenhengen mellom organisasjonsgrad og arbeidsledighet for innenlandskt og utenlandskt fødte i ulike land. 

Datasettet «TUD» i R-pakken «oecd» inneholder data på organisasjonsgrad (ObsValue = organisasjonsgrad). Datasettet «MIG_NUP_RATES_GENDER» inneholder informasjon om arbeidsledighet i ulike grupper (ObsValue = arbeidsledighetsrate). Bruk data for år 2018, og for begge kjønn (GENDER = TOT). Dersom du bruker ggplot i Rstudio, kan du bruke kommandoen: «geom_smooth(method=lm, se=FALSE)» til å få fram en korrelasjonslinje.

- Bruk data for innenlandsfødte (BIRTH = NB) og utenlandsfødte (BIRTH = FB) til å lage to grafer som viser sammenhengen mellom organisasjonsgraden i fagforeninger og nivået på arbeidsledigheten i ulike land for de to gruppene. 

- Diskuter dine empiriske observasjoner ut fra økonomisk teori om forhandling mellom arbeidsmarkedets parter og medlemsbasens sammensetning.



### Innlevering
Innleveringene skal skje individuelt.

Utfodringene skal leveres i Canvas. Kode og redegjørelser for bruk av kunstig intelligens leveres som appendiks i oppgaven (enten i et separat eller i samme dokument). 

**NB: Det er utrolig viktig at du bruker følgende navn på din innlevering! "[ditt kandidatnummer]sok_2008_h24_utf4"**
Vi trenger ditt kandidatnummer for å gi en eventuell klagekommisjon tilgang til din oppgave. 
 
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
