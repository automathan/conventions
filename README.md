# Conventions 

[🇳🇴](#norsk) [🇬🇧](#english)


## Norsk
Denne listen er kompilert for bruk hos Cogito NTNU, kontribuer gjerne om du har noen rettelser eller tilføyninger.
_Merk at dette er retningslinjer, og med det så finnes det alltid unntak. Derfor bør de ansees som gjeldende dersom ikke annet er spesifisert._

### Navngivning
- Klasser skal ha et beskrivende navn i ubestemt entall.
- Klasser navngis med substantiv, funksjoner med verb.
- Ikke bruk forkortelser i navn på klasser og funksjoner. _Typiske unntak: RSA, gcd_
- Følg programmeringsspråkets standard for forbokstavs-konvensjoner for klasser, funksjoner og variabler med forskjellige tilgangsmodifikatorer.
- Dersom et konsept har flere annerkjente navn, velg ett og hold deg til det.
- Ikke bland inn informasjon om en funksjons utviklingstilstand i navnet. _Eksempel: funksjonA\_temp, WIPKlasseBv2_
- Ved sammensatte navn, være konsistent i rekkefølgen på beskrivende ord. _Eksempel: ikke ha både QuickSort og SearchBinary, men heller QuickSort og BinarySearch_
- Prøv å unngå veldig lange og sære navn. Hvis du ikke kommer unna kan det være et tegn på at prosjektet har et designproblem.

### Kode
- Konstanter burde deklareres som konstanter, med riktig navngivning og passende skop. Unntak er spesielle tall som _0, 1, 2, -1, 0xff_ og liknende (i riktig kontekst, vel å merke).
- Følg DRY-prinsippet (Don't Repeat Yourself). Dersom du føler at du skriver noe som er tilnærmet identisk til noe du har skrevet før, vurder å lage f.eks. en _utility_-funksjon som gjør det. Dette reduserer selvfølgelig antall linjer, men hovedfordelen er heller at når man ikke trenger å skrive koden på nytt, så kan man heller ikke gjøre dumme slurvefeil.

### Git
- Ikke commit utkommentert kode, med mindre du vet at det helt sikkert kommer til å bli avkommentert til en senere tid.
- Prøv å unngå at flere én commit inneholder løsningen på mange helt forskjellige problemer, eller en samling nye funsksjoner uten noen sterk sammenheng.
- Skriv commit-meldinger. Ikke skriv dagbok, skriv heller ikke _shit3fixedfinal_, med mindre det beskriver presist hva du har gjort.

## English
This list is compiled for use at Cogito NTNU, feel free to contribute if you have any corrections or additions in mind. 
_Note that these are just guidelines, which means that there are always exceptions. Therefore they should rather be treated as default unless anything else is specified.


### Naming
- Classes should be named with a descriptive _singular_ noun.
- While functions should be named as verbs.
- Do not use abbreviations in class and function names. _Some valid exceptions: RSA, gcd_
- Follow the capitalization conventions specified by the programming language standard for classes, functions and variables with different access level modifiers.
- If a concept has several accepted names, choose one and stick to it.
- Names should not contain any traces of development information. _Example: functionA\_temp, WIPClassBv2_
- In the case of multi-word names, make sure the ordering of descriptive words is consistent through the project. _Example: avoid having QuickSort and SearchBinary when you can have QuickSort and BinarySearch_
- Try your best to avoid long and weird names. If you cannot get around this, you might want to reconsider the overall design of your program.

### Code
- Constants should be declared as constants, with a proper name and scope. Exceptions are special numbers such as _0, 1, 2, -1, 0xff_ og liknende (given the right context).
- Respect the DRY-principle (Don't Repeat Yourself). If you feel that you are repeating yourself, consider making a _utility_ function that you can replace all occurences of similar code segments with. While reducing the overall line count, the main advantage is that you reduce the possibility for error.

### Git
- Do not commit code that is commented out, unless you know for sure that it will be uncommented at some point in the future.
- Try to avoid grouping a bunch of unrelated segments of code into the same commit.
- Use commit messages. It is not your diary, but you should neither write _shit3fixedfinal_, unless that describes exactly what you have done.
