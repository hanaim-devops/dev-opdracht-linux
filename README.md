# Dev Opdracht Linux - Bash opdracht Linux

- *Auteur*: Bart van der Wal
- *Datum*: 8 september 2022
- *Laatste edit*: 19-4-2024 voor de 2024 editie, opdracht vanaf nu in duo's, extra opdrachten

De user stories hieronder vertellen op zich het hele verhaal over het te schrijven script. Verdeel de user stories gelijkmatig over de twee studenten en volg de ['werkwijze week-opdrachten'](https://minordevops.nl/week-opdrachten.html) met het aanmaken van planbord/issues voor de taken en het committen op de issues.

- Gebruik als linter [shell check](https://www.exasol.com/resource/ghost-in-the-shell-busters-your-guide-to-using-shellcheck-for-top-quality-scripts/) voor - Linting/kwaliteitssuggesties voor je bash script. Deze heeft ook een [VS Code extensie](https://marketplace.visualstudio.com/items?itemName=timonwong.shellcheck).
- Lever deze opdracht (ivm accreditatie) in via upload naar iSAS, en zet deze in een zip in een aparte folder `dev-opdracht-linux` direct in de root van de zip (naast andere Dev BP's, zoals de blog die je later schrijft).

### MUST User Stories

- [ ] **US-1** Als docent wil ik dat een DevOps student aan een Linux bash script schrijft zodat deze laat zien over basis Linux vaardigheden te beschikken
- [ ] **US-2** Als docent wil ik dat het een echt 'CLI programma' wordt, dus die [command line opties](https://en.wikipedia.org/wiki/Command-line_interface#Command-line_option) van de gebruiker accepteert zodat iemand het gemaakte script in eigen bash scripts kan hergebruiken (compositie) (laat he script dus dus NIET een dialoog met je gebruiker aangaan, hoogstens als uitbreiding) )
- [ ] **US-3** Als docent wil ik dat studenten het script Nederlandstalige optie- en flagnamen geeft (bv. `-h` en `--hostnaam`) zodat de student een voorproefje krijgt van deze DDD-conventie
- [ ] **US-4** Als gebruiker wil ik dat het script zelf uitlegt wat het doet/kan als je geen parameters meegeeft (of evt `--help`) zodat ik geen externe documentatie hoef te krijgen/lezen
- [ ] **US-5** Als docent wil ik dat elk van studenten minstens 6 user stories implementeert (dus als duo samen 12), met 3 SHOULD, 2 COULDs en 1 WannaHave zodat 'niet alles belangrijk is' en er verschillende uitwerkingen komeng en de student tegelijkertijd een bepaalde minimale inspanning moet leveren
- [ ] **US-6** Als docent wil ik dat de student het script de naam `<student-naam-1-student-naam-2>` geeft, of `student-naam-1-student-naam-2>-script`<sup>*</sup> geeft zodat ik snel kan zien wiens script van wie is als ik alle gemaakt scripts bij elkaar in een folder zet bij het nakijken
- [ ] **US-7** Als docent wil ik dat het script de output van alle geimplementeerde user stories laat zien via een '--alles' optie, zodat ik tijdens het beoordelen alle output kan verifieren
- [ ] **US-8** Als docent wil ik dat je geimplementeerde features los van elkaar kunt kiezen via command line opties met logische én semantische namen zodat dit script weer te gebruiken is in een ander script (compositie)
- [ ] **US-9** Als docent wil ik dat elke student de volgende standaarden aanhoudt, zodat de repo vindbaar is en zelfbeschrijvend is, en de beoordelaar de in README.md beschreven stappen domweg kan uitvoeren om het script te executeren/testen
      - **US-9a** het gemaakte script staat in een zelf aangemaakte privé repo
      - **US-9b** heeft een eigen, korte maar duidelijke en volledige [README volgens dez Microsoft standaard](https://docs.microsoft.com/en-us/azure/devops/repos/git/create-a-readme) 
      - **US-9c** deze `README.md` bevat een kopje `User Stories` met hierin de afgevinkte user stories uit deze lijst met 'markdown checkboxes' (GitHub flavoured markdown feature)
      - **US-9d** je scant op linting issues uit het script met shellcheck en refactort code smells (kijk ook naar 'warning's, 'info' of 'style' meldingen)

<sup>*</sup>Je mag ook een extensie `.sh` geven als je dit [handiger vindt](https://stackoverflow.com/questions/27813563/what-is-the-bash-file-extension). Hoewel sommigen een `.sh` extensie logischer vinden, is inmiddels het weglaten ervan de consensus in de Unix/Linux wereld.

## SHOULD User Stories

- [ ] **US-10** Als gebruiker wil ik dat het script het aantal subfolders van de [home](https://nl.wikipedia.org/wiki/Homedirectory) folder toont, zodat ik een beeld krijg hoe 'gevuld' de home folder is
- [ ] **US-11** Als gebruiker wil ik dat het script de naam van huidige gebruiker laat zien, zodat ik deze kan verifiëren
- [ ] **US-12** Als gebruiker wil ik dat het script het aantal bestanden in de huidige folder laat zien, zodat ik een idee krijg hoe groot deze is
- [ ] **US-13** Als gebruiker wil ik dat het script de huidige folder naam laat zien, zodat ik deze kan verifieren
- [ ] **US-14** Als gebruiker wil ik dat het script de huidige hostname laat zien, zodat ik deze kan verifieren
- [ ] **US-15** Als gebruiker wil ik dat het script hierbij ook het (lokale!) IP adres van het systeem laat zien zodat ik deze kan verifieren
- [ ] **US-16** Als docent wil ik dat als de student ook wat COULD of WannaHave features inmplementeert zoals in US-5 beschreven, waarbij de student in plaats van de wannahave  ook zelf een logische/leuke extra features kan bedenken en maken, mits je deze ook in de hulp functie zet én de userstory-lijst in de README zet inclusief `zodat` deel, zodat de student kan oefenen met een user story schrijven en het concept van [Continuous Documentation](https://thenewstack.io/continuous-documentation-in-a-ci-cd-world/) en welllicht zelfs [README driven development](https://rathes.me/blog/en/readme-driven-development/)

## COULD User Stories

- [ ] **US-17** Als gebruiker wil ik dat het script de totale schijfruimte en beschikbare schijfruimte van het huidige systeem toont met --schijfruimte, zodat ik inzicht krijg in de opslagcapaciteit.
- [ ] **US-18** Als gebruiker wil ik dat het script met de optie `--bestandsrechten` de toegangsrechten van alle bestanden in de huidige directory weergeeft, zodat ik de beveiligingsstatus kan controleren.
- [ ] **US-19** Als gebruiker wil ik dat het script via de optie `--procescontrole` een lijst van de top 5 processen qua geheugengebruik toont, zodat ik inzicht krijg in resourcegebruik.

## WANNAhave User Stories

- [ ] **US-20** Als gebruiker wil ik dat het script met `--netwerkinfo` basis netwerkinformatie toont, zoals de naam van het netwerk en de gebruikte bandbreedte, zodat ik mijn netwerkverbinding kan monitoren.
- [ ] **US-21** Als gebruiker wil ik dat het script met de optie `--hardwareinfo` beknopte informatie geeft over de CPU en het geheugen, inclusief type en snelheid, zodat ik weet wat de machine aankan.
- [ ] **US-22** Als gebruiker wil ik dat het script een interactieve kaart van de directorystructuur toont met `--kaart`, zodat ik visueel kan navigeren door mijn bestanden.
