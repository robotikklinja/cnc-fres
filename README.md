# CNC Hector

## Om prosjektet 

Prosjektet er sentrert rundt utviklingen, oppbyggingen og oppgradering av den semi portable CNC fresen Hector. Hector er en CNC fres utviklet av Fabricatable Machines(FB) gruppen som består av norske utviklere og automatikere. Blant disse er Jacob Nilsson. Det spesielle med maskinene til FB er at alle delene skal kunne produseres med en tre akse CNC fres. Dette gir deg muligheten til å oppgradere og videreutvikle fresen med minimalt med remodellering. 

Hva er det vi skal gjøre med fresen.
Det som robotikk linja skal gjøre på denne fresen er å videreutvikle fresen for å støtte 6DOF. I tillegg til dette skal vi sette opp det elektriske med PSU for for stepper motorene, sjekke oppkoblingen av alle kabler og monteringen av endestopp sensorer. Du kan finne en komplett liste over arbeidsoppgaver som gjøres nedenfor.

-Jonathan

Laste ned UGS for kontroll over fres, lastes ned [her](https://winder.github.io/ugs_website/download/). Velg 2.0 Platform

## Fixing the "missing java" problem with UGS
If your computer suddenly claims that it can't find your Java installation you can help it by telling it where it is.
* First install the latest [Java](https://www.java.com) version to be absolutely sure you actually have it.
* Go to where the folder which contains the UGS program files, it's called ugsplatform. *It will be where you unpacked it, if you don't know where you put it, then it's probably in your downloads folder.* 
* Open the ugsplatform/etc subfolder
* Edit the ugsplatform.conf in your favorite text editor (notepad etc..)
* Find the line starting with #jdkhome 
* Replace it with this line: (remove the #)
```
 jdkhome="C:/Program Files (x86)/Java/jre1.8.0_221/"
```
* Double check that you have java in that folder, if it is somewhere else, adjust the path to fit.
* UGS should now work
* Do yourself a favour and create a desktop shortcut to the UGS start file **ugsplatform/bin/ugsplatform64.exe**
