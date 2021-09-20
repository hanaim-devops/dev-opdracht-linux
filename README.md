# Dev Opdracht Linux

## User stories bij bash opdracht Linux

Auteur: Bart van der Wal
*Datum: 8 september 2022*
*Edited 20-9-2022 voor de 2023 editie*

### Must

> - **US-1** [ ] Als docent wil ik dat een DevOps student een Linux bash script schrijft zodat deze laat zien over basis Linux vaardigheden te beschikken
> - **US-2A** [ ] Als docent wil ik dat student het script Nederlandstalige hulp en optienamen geeft zodat student een voorproefje krijgt van deze DDD-conventie
> - **US-2B** [ ] Als gebruiker wil ik dat het script zelf uitlegt wat het doet/kan als je geen parameters meegeeft (of evt `--help`) zodat ik geen externe documentatie hoef te krijgen/lezen
> - **US-3** [ ] Als docent wil ik dat minstens 4 'should' user stories  implementeert zodat 'niet alles belangrijk is' en er verschillende uitwerkingen van deze uitwerking en de student wel bepaalde minimale inspanning moet leveren
> - **US-4A** [ ] Als docent wil ik dat de student het script de naam `<student-naam>.sh` of `student-naam>-script.sh`<sup>*</sup> geeft zodat ik snel kan zien wiens script van wie is als ik alle gemaakt scripts bij elkaar in een folder zetten bij het nakijken
> - **US-4B** [ ] Als docent wil ik dat de student het gemaakte script in een zelf aangemaakte privé repo zet, en deze een eigen, korte maar duidelijke en volledige [README](https://docs.microsoft.com/en-us/azure/devops/repos/git/create-a-readme) geeft, inclusief een kopje met  de afgevinkte user stories uit deze lijst, zodat de repo zelfbeschrijvend is, de beoordelaar beschreven stappen domweg kan uitvoeren om het script te executeren, en de zonder README wellicht verborgen/impliciete dependencies kan terughalen zoals het gebruikte Linux distributie, versienummer en shell type

<sup>*</sup>Je mag de extensie `.sh` ook weglaten als je dit [logischer vindt](https://stackoverflow.com/questions/27813563/what-is-the-bash-file-extension) (dit lijkt dus wel de consensus in Unix/Linux wereld).

## Should

> - **US-5A** [ ] Als gebruiker wil ik dat het script het aantal subfolders van de [home](https://nl.wikipedia.org/wiki/Homedirectory) folder toont, zodat ik een beeld krijg hoe uitgebreid dit is
> - **US-5B** [ ] Als gebruiker wil ik dat het script ook de naam van huidige gebruiker laat zien, zodat ik deze kan veriferen
> - **US-6A** [ ] Als gebruiker wil ik dat het script het aantal bestanden in de huidige folder laat zien, zodat ik idee krijg hoe groot deze is
> - **US-6B** [ ] Als gebruiker wil ik dat het script hierbij ook de huidige folder naam laat zien, zodat ik deze kan verifieren
> - **US-7A** [ ] Als gebruiker wil ik dat het script de huidige hostname laat zien
> - **US-7B** [ ] Als gebruiken wil ik dat het script hierbij ook het ip adres van het systeem laat zien
> - **US-8A** [ ] Als docent wil ik dat je geimplementeerde features los van elkaar kunt kiezen via command line opties met logische én semantische namen
> - **US-8B** [ ] Als gebruiker wil ik dat het script output van alle geimplementeerde user stories laat zien via een '--alles' optie

## Could/Wannahaves

> - **US-9** [ ] Als docent wil ik dat als de student zelf logische/leuke extra features weet bedenkt hij/zij deze toevoegt voor bonuspunten/kudo's, maar dan ook in de hulp functie, de README zet en deze userstorylijst zet en inclusief `zodat` deel, zodat student nog eens kan oefenen met user story schrijven en het concept van [continuous documentation](https://thenewstack.io/continuous-documentation-in-a-ci-cd-world/) of welllicht zelfs [README driven development](https://rathes.me/blog/en/readme-driven-development/)
