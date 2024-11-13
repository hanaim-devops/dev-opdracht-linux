# Herkansing Opdracht

Maak een Linux Script maakt die als input een lijst met pig latin namen gecodeerde namen en (niet gecodeerde) onderzoeksonderwerpen omzet naar gedecodeerde namen.

Voorbeeld input
```bash
01. Tudent1say - gRPC
02. Anjay – runC
03. Illem-Alexanderway – Water management
```

Decodeert deze naar:
```bash
01. Student1 - gRPC
02. Jan – runC
03. Willem-Alexander – Water management
```

Geef het script als naam je eigen voornaam in piglatin.

Zet dit in een prive repo. En maak hierin ook een README.md aan in je repo die de gebruiker aangeeft hoe het te testen/beoordelen.

Doe dit volgens de [regels voor readme van Microsoft](https://docs.microsoft.com/en-us/azure/devops/repos/git/create-a-readme?view=azure-devops), met in ieder geval een `Intro` en een (Help your users) `Get started` kopje erin.

> "Run through the instructions as you write them in order to verify the instructions would work." - Microsoft, Vijay Machiraju et al. 14 maart 2018

>chmod + x igpay

Hint: Gebruik `sed` om met reguliere expressie en capture groups e.d. te werken.

Merk op dat je script de onderzoeksonderwerpen, nummering en tussen m-dash verder in tact laat.
Het moet uiteraard werken op een willekeurige lijst, niet alleen op deze. Maak zelf een 2e test lijst en decodeer deze eerst handmatig.
Merk uit voorgaande voorbeeld bv. op dat er ook nog wat met de hoofdletters moet gebeuren. Bewaar dit echter voor het laatste.

Graag opsplitsen in deelfuncties met logische naam. Reguliere expressie code is al moeilijk genoeg te lezen (write only code). Maar eerst iets aan de praat krijgen... Go to artikel voor 'sed' schijnt het (wat outdated ogende) artikel van Bruce Barnett te zijn.

"...sed is a marvelous utility. Unfortunately, most people never learn its real power" - Bruce Barnett

Het aangeraden artikel voor 'sed' schijnt het — wel wat outdated ogende — [artikel van Bruce Barnett](https://www.grymoire.com/Unix/Sed.html) te zijn.

Als je klaar bent vorg dan nog 2 van onderstaande features toe:

1. ook mogelijk om input te encoden via een flag `--encode` of optie `-e`.
2. De default flag is `–decode` of `-d`. Bij missende input krijg je hulp functie. 
3. Help functie met bericht
4. Help bericht ook sturen als GEEN parameters worden meegegeven
5. Extra bonus: Ook standard input accepteren via pipe of redirect: cat onderzoeksonderwerpen > igpay

```bash
Missende parameters
Gebruik: igpay [-d | --decode] [-e | --encode] [-h | --help] file
```
