# Conventions

[🇳🇴](#norsk) [🇬🇧](#english)

## Norsk
Denne listen er kompilert for bruk hos Cogito NTNU, kontribuer gjerne om du har noen rettelser eller tilføyninger.
_Merk at dette er retningslinjer, og med det så finnes det alltid unntak. Derfor bør de ansees som gjeldende dersom ikke annet er spesifisert._

### Navngivning
- Alle variabler, funksjoner, klasser, kommentarer etc. skal skrives på engelsk.
- Klasser skal ha et beskrivende navn i ubestemt entall.
- Klasser navngis med substantiv, funksjoner med verb.
- Ikke bruk forkortelser i navn på klasser og funksjoner. _Typiske unntak: RSA, gcd_
- Følg programmeringsspråkets standard for forbokstavs-konvensjoner for klasser, funksjoner og variabler med forskjellige tilgangsmodifikatorer.
- Dersom et konsept har flere annerkjente navn, velg ett og hold deg til det.
- Ikke bland inn informasjon om en funksjons utviklingstilstand i navnet. _Eksempel: funksjonA\_temp, WIPKlasseBv2_
- Ved sammensatte navn, være konsistent i rekkefølgen på beskrivende ord. _Eksempel: ikke ha både QuickSort og SearchBinary, men heller QuickSort og BinarySearch_
- Prøv å unngå veldig lange og sære navn. Hvis du ikke kommer unna kan det være et tegn på at prosjektet har et designproblem.
- La filtypene tale for seg. _Eksempel: script.py istedet for python_script.py_
- Prøv å reservere korte og mye brukte variabelnavn eksklusivt til lokale variabler med relativt lite skop. _Eksempel: x, y, i, j, max, temp, tmp..._

### Kode
- Konstanter burde deklareres som konstanter, med riktig navngivning og passende skop. Unntak er spesielle tall som _0, 1, 2, -1, 0xff_ og liknende (i riktig kontekst, vel å merke).
- Følg DRY-prinsippet (Don't Repeat Yourself). Dersom du føler at du skriver noe som er tilnærmet identisk til noe du har skrevet før, vurder å lage f.eks. en _utility_-funksjon som gjør det. Dette reduserer selvfølgelig antall linjer, men hovedfordelen er heller at når man ikke trenger å skrive koden på nytt, så kan man heller ikke gjøre dumme slurvefeil.
- Maks linjelengde er 100 tegn.
- Følg programmeringsspråkets konvensjon for indentering.

### Kommentering
- Forklar koden, ikke forklar programmering. Anta at leseren har en grunnleggende forståelse av språket.
- Kommentaren skal komme før det den kommenterer (linjemessig).
- Korte kommentarer på samme linje som koden brukes der det passer seg, men pass på så ikke koden tar mye plass i bredden.
- Kommenter variabler når de skal deklareres _dersom_ navnet på variabelen ikke forklarer seg selv tilstrekkelig.
- Dersom kommentarene blir mistenkelig lange, vurder en omskrivning av koden du kommenterer. Hvis noe ikke kan forklares over relativt få setninger kan det indikere kryptisk kode.
- Når en kommentar kommer før en funksjon eller klasse, skal den typisk forklare _hva_ funksjonen eller klassen gjør, noen ganger kan man også føye kort på _hvordan_ den gjør det. Trengs det derimot en grundig forklaring på _hvordan_ det gjøres, vurder å kommentere mellom linjene inne i funksjonskroppen.
- Prøv å være generell hvis mulig, ikke anta at leseren kjenner til resten av prosjektet inn og ut. Dersom du referer til andre særegne komponenter i prosjektet, sørg for at også disse er grundig kommentert og dokumentert, slik at leseren alltids har muligheten til å forstå det helhetlige bildet.

### Tester
- Navn på tester burde følge et konsistent format som gjør det klart hvilken funksjonalitet som testes.
- Enhetstester burde begrenses til å teste spesifikk funksjonalitet, og burde ikke
  inneholde logikk.

### Git
- Ikke commit utkommentert kode, med mindre du vet at det helt sikkert kommer til å bli avkommentert til en senere tid.
- Prøv å unngå at flere én commit inneholder løsningen på mange helt forskjellige problemer, eller en samling nye funsksjoner uten noen sterk sammenheng.
- Skriv commit-meldinger. Ikke skriv dagbok, skriv heller ikke _shit3fixedfinal_, med mindre det beskriver presist hva du har gjort.
- Commit message subjects should be written in the imperative mood.
  A trick for writing commit subjects are "If this commit is applied, it will X", where X is
  your commit message subject. Example: "Add tests for DateTime time-zone conversion".
- Commit-meldinger bør skrives i imperativ modus, og på engelsk. Et triks for å skrive commit-meldinger er å skrive i formatet "If this commit is applied, it will X", der X er
  commit-meldingen. Eksempel: "Add tests for DateTime time-zone conversion".
- All kode skal gå gjennom _code-review_ før det blir merget. Følg konvensjonen om
  pull-requests.

## English
This list is compiled for use at Cogito NTNU, feel free to contribute if you have any corrections or additions in mind.
Note that these are just guidelines, which means that there are always exceptions. Therefore they should rather be treated as default unless anything else is specified.

### Naming
- All variables, functions, classes, comments, etc. should be written in English.
- Classes should be named with a descriptive _singular_ noun.
- While functions should be named as verbs.
- Do not use abbreviations in class and function names. _Some valid exceptions: RSA, gcd_
- Follow the capitalization conventions specified by the programming language standard for classes, functions and variables with different access level modifiers.
- If a concept has several accepted names, choose one and stick to it.
- Names should not contain any traces of development information. _Example: functionA\_temp, WIPClassBv2_
- In the case of multi-word names, make sure the ordering of descriptive words is consistent through the project. _Example: avoid having QuickSort and SearchBinary when you can have QuickSort and BinarySearch_
- Try your best to avoid long and weird names. If you cannot get around this, you might want to reconsider the overall design of your program.
- Let the file extensions do their job. _Example: use script.py instead of python_script.py_
- Try to reserve short and commong variable names exclusively for local variables with limited scopes. _Example: x, y, i, j, max, temp, tmp..._

### Code
- Constants should be declared as constants, with a proper name and scope. Exceptions are special numbers such as _0, 1, 2, -1, 0xff_ (given the right context).
- Respect the DRY-principle (Don't Repeat Yourself). If you feel that you are repeating yourself, consider making a _utility_ function that you can replace all occurences of similar code segments with. While reducing the overall line count, the main advantage is that you reduce the possibility for error.
- Maximum linewidth is 100 characters.
- Follow the indentation conventions specified by the given programming language.

### Commenting
- Explain the code, not programming in itself. Assume that the reader has a general familiarity with the language.
- The comment should precede whatever it is commenting (line-wise).
- Short comments on the same line as the code can be utilized when appropriate, but beware of wide lines.
- Comment a varible when you declare it _if_ the name is not completely self-explanatory.
- If the comments are getting suspiciously long, consider a rewrite of the code iself. If you cannot explain it in relatively few sentences it might indicate cryptic code.
- If a comment precedes a function or a class, it should typically explain _what_ the function or the class does, occasionally one can also add a note on _how_ it's done as well. Should you however need an excessive explanation of _how_ it is done, consider comments between the lines inside the function body.
- If possible, try to be general in your comments, do not assume that the reader knows every detail about the rest of the project. Should you refer to other distinctive components in the project, make sure those are also properly commented and documented so that the reader is allowed the insight they need to proceed.

### Tests
- Unit tests shold follow a consistent naming conventions which easily communicates
  its purpose.
- Unit tests should be restricted to test specific functionality, and should not
  contain logic.

### Git
- Do not commit code that is commented out, unless you know for sure that it will be uncommented at some point in the future.
- Try to avoid grouping a bunch of unrelated segments of code into the same commit.
- Use commit messages. It is not your diary, but you should neither write _shit3fixedfinal_, unless that describes exactly what you have done.
- Commit message subjects should be written in the imperative mood.
  A trick for writing commit subjects are "If this commit is applied, it will X", where X is
  your commit message subject. Example: "Add tests for DateTime time-zone conversion".
- All code should pass _code-review_ before merging. Follow the conventions
  for pull-requests.
