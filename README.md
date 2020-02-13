# CNC Hector

## Om prosjektet 

Prosjektet er sentrert rundt utviklingen, oppbyggingen og oppgradering av den semi-mobile CNC-fresen, Hector. Hector er en CNC fres utviklet av Fabricatable Machines (FB) gruppen som består av norske utviklere og automatikere. Blant disse er Jacob Nilsson. Det spesielle med maskinene til FB er at alle delene skal kunne produseres med en tre-akset CNC fres. Dette gir muligheten til å oppgradere og videreutvikle fresen med minimal remodellering. 

Det som robotikklinja skal gjøre på denne fresen er å videreutvikle den for å støtte 6DOF (degrees of freedom). I tillegg til dette skal det settes opp det elektriske med PSU for for stepper motorene, sjekke oppkoblingen av alle kabler og monteringen av endestoppsensorer. Alle arbeidsoppgaver som står igjen kan man finne under "Projects" -> "Jakob sin TODO liste". Her står det også hva som er gjort ferdig og hva som er i gang.

##  Oppstart av fres med UGS og Arduino

Først må man laste ned UGS for kontroll over fres [herfra](https://winder.github.io/ugs_website/download/). Velg 2.0 Platform.

For å få kontakt med Arduinoen i UGS må du ha lastet ned Arduino drivere for PC-en. Last ned denne filen [her](https://www.arduined.eu/ch340g-converter-windows-7-driver-download/). Etter nedlastning pakk ut filen, gå inn på CH341SER og kjør "Setup.exe". Deretter åpner du UGS, og setter Baud til 115200. Trykk på connect, fresen skal nå respondere.



## Hvordan fikse "missing Java" problemet i UGS?
Hvis PC-en din plutselig sier at den ikke finner Java installasjonen din, må du fortelle den hvor installasjonen er. Dette gjøres slikt:
-	Last ned den nyeste Java versjonen.
-	Før du fortsetter, må du vite hvilken versjon du har. For å finne denne åpner du cmd og skriver `java -version`. Husk dette versjonsnummeret til etterpå.
-	Naviger til mappa som inneholder UGS programfilene. Den heter «ugsplatform» og skal ligge der du pakka ut .zip filen da du lasta ned UGS.
-	Åpne ugsplatform/etc submappa.
-	Åpne ugsplatform.conf filen. Denne kan åpnes med hvilken som helst text-editor, f. eks. Notepad.
-	Finn linja som starter med #jdkhome.
    - Erstatt den med `jdkhome="C:/Program Files (x86)/Java/jre*DIN JRE VERSJON*/"` og husk å slette #-en.
    - Min JRE versjon er 1.8.0_241, så linja skal se sånn ut: `jdkhome="C:/Program Files (x86)/Java/jre1.8.0_241/"`
-	Dette er default mappa til Java nedlastninger. Hvis du har lasta ned Java i en annen mappe, må du oppdatere path-en. 





