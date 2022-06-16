## Inhoud
- [Web Application](#web-application)
- [Software Quality](#software-quality)
- [CI/CD](#cicd)
- [Professional](#professional)
<hr/>

# Web Application

Om deze leeruitkomst aan te tonen heb ik 1 fullstack applicatie gemaakt waar mensen nieuws van over de hele wereld kunnen lezen en commentaar op deze artikelen kan geven samen met een cijfer.

## News front-end

Repository: [News front-end](https://github.com/431433/S3-NewsFrontEnd)

### **Losse pagina,**

In mijn front-end applicatie begin je op een losse pagina die uitwisselt met verschillende componenten, via vue-router, op basis van wat de gebruiker wilt zien. De gebruiker kan dan kiezen uit: Top stories, War, Sports, Covid-19 of de gebruiker zoekt het onderwerp waarin hij geïnteresseerd is.
![Screenshot 2022-06-13 at 21-29-57 s3-newsfrontend](https://user-images.githubusercontent.com/77282414/174152745-4332db85-e8a7-498c-99ea-11b305c3c29b.png)


### **Accounts,**

Voor accounts heb ik een extentie gebruikt, Auth0. Auth0 is een flexibele drop-in-oplossing om authenticatie- en autorisatieservices om aan mijn applicatie toe te voegen. Ik heb zo het risico vermijden die gepaard gaan met het bouwen van mijn eigen oplossing voor het verifiëren en autoriseren van gebruikers.

<img src="https://user-images.githubusercontent.com/77282414/168020607-d229e649-9238-4d2e-b462-d51784e94ae5.PNG" height="300">

### **Comments,**

Mensen kunnen er ook voor kiezen om een mening achter te laten op het artikelen, deze functionaliteit heb ik wel alleen nog toegevoegd aan oorlogs artikelen, maar zou zo makkelijk kunnen worden geïmplementeerd om bij alle artikelen te werken.

![review](https://user-images.githubusercontent.com/77282414/174154007-72e83658-d79d-4ad6-a68c-740404819eab.PNG)

## News back-end

Repository: [News back-end](https://github.com/431433/S3-NewsBackEnd)

### **NewsAPI,**

Om alle artikelen op te halen maak ik gebruik van de NewsAPI.

![NewsAPI](https://user-images.githubusercontent.com/77282414/168020985-ff9c9ca6-837a-4916-ad8b-fb433427ea77.PNG)


### **Interactie,**

Om de gebruikers commentaar achter te laten, maak ik gebruik van een apart lopende database. Deze houdt bij welke artikelen het commentaar hoort en welke cijfers erbij horen. Voor de database gebruik ik een MySQL database. MySQL is een vrij toegankelijk SQL-relationele databasebeheersysteem dat ontwikkeld is en ondersteund wordt door Oracle. In een relationele database zijn je gegevens onderverdeeld in verschillende van elkaar afgescheiden opslagruimtes, tabellen, in plaats van alles bij elkaar te gooien in één grote opslagloods.
In deze database sla ik de titel, cijfer en mening op die achter gelaten zijn bij een artikelen. 

![mysql](https://user-images.githubusercontent.com/77282414/174154889-75408622-9170-4819-aa99-88f67187ad83.PNG)

In de back-end heb ik zelf API calls staan die ervoor zorgen dat ik met de front-end kan communiceren. Er kunnen zo meningen worden opgeslagen en opgehaald. Ook wordt het gemiddelde cijfer berekend van alle meningen samen. Zo kan ik aan de bovenkant van de review pagina een gemiddeld cijfer weergeven, hiermee kan de gebruiker al een eerste impressie krijgen.

![grade](https://user-images.githubusercontent.com/77282414/174155656-ee737234-56ca-4906-8235-ffe66711ffc6.PNG)

# Software Quality

Softwarekwaliteit is een abstract begrip. Zijn aanwezigheid kan moeilijk te definiëren zijn, maar zijn afwezigheid kan onmiddellijk worden gezien. Dus, in de zoektocht naar het verbeteren van de softwarekwaliteit, moeten we eerst de definitie van softwarekwaliteit begrijpen. <a href="https://en.wikipedia.org/wiki/Software_quality">Wikipedia</a> beschrijft de softwarekwaliteit als volgt:

“In de context van software-engineering meet softwarekwaliteit hoe goed de software is ontworpen (kwaliteit van ontwerp) en hoe goed de software overeenkomt met dat ontwerp (kwaliteit van conformiteit). Het wordt vaak omschreven als de ‘fitness for purpose’ van een stukje software.”

Er zijn veel variaties op de definitie van softwarekwaliteit, afhankelijk van het gezichtspunt (ontwikkelaar, eindgebruiker, management...), maar als je de bovenstaande definitie bekijkt, vraagt "fitness for purpose" zich af of de software wel doet wat die moet doen. Dat zijn de kenmerken die wij als eindgebruikers zien. De kwaliteit van het ontwerp en de kwaliteit van conformiteit met dat ontwerp zijn gerelateerd aan interne aspecten van de software, waarvan we sommige kunnen zien, zoals de navigatie van de gebruikersinterface, de plaatsing van bedieningselementen, enzovoort.

Deze gebruikersinterface heb ik doormiddel van verschillende UI ontwerpen getest. Meerdere pagina's in mijn project zijn allemaal ontworpen met andere css en andere plaatsing van bedieningselementen. Zo kon ik een klein onderzoekje doen om te kijken wat er als het beste wordt ervaren als exterene gerbuiker.
Deze kan je hier terug vinden: <a href="https://git.fhict.nl/I431433/s3-portfolio/-/blob/main/Research/UIResearch.pdf"> linkje <a/>
  
Ik heb in de back-end ook nog een aantal unit testen gemaakt, in dit geval voor mijn zelf gemaakt API calls, om zo te checken of alles wel naar behoren werkt. Daarnaast zijn al mijn query's beveiligd met de methodes waar ik over heb geleerd tijdens mijn security onderzoek.
Unit testen is een type softwaretest waarbij individuele eenheden of componenten van een software worden getest. Het doel is om te valideren dat elke eenheid van de softwarecode presteert zoals verwacht. Unit Testing wordt gedaan tijdens de ontwikkeling (coderingsfase) van een applicatie door de ontwikkelaars. Unit Tests isoleren een deel van de code en verifiëren de juistheid ervan. Een eenheid kan een individuele functie, methode, procedure, module of object zijn.
  
In mijn geval heb ik het creëren van reviews, ophalen van specifieke artikelen en de bijhorende reviews en het berekenen van het gemiddelde cijfer getest.
Al deze tests worden gedaan met de hulp van een MockDal.
  
![tests](https://user-images.githubusercontent.com/77282414/174157642-93ebdecc-34ea-499e-99f7-965f59a98dcc.PNG)
  
Bij het schrijven van tests voor je applicatie is het vaak wenselijk om de database niet te raken. Entity Framework stelt je in staat om dit te bereiken door een context te creëren - met gedrag gedefinieerd door uw tests - die gebruik maakt van in-memory data. 
  Door bij het aanroepen van de Data Acces Layer een nieuwe database mee te geven, voorkom ik perongeluk mijn eigen database, MySQL, te gebruiken en mogelijk belangerijke data aanpas of verwijder.
  
![wissel](https://user-images.githubusercontent.com/77282414/174158482-74a7afe9-171a-4234-b2e0-d7365376d356.PNG)

  Het uitwisselen van databasen heb ik door middel van het Entity Framework kunnen doen, als oefening heb ik dan ook meteen 5 lagen gemaakt in mijn back-end, de test laag niet mee geteld dan.
  
![lagen](https://user-images.githubusercontent.com/77282414/174158606-7a95c85b-ec4f-494e-b03b-c3fc9419823b.PNG)

# CI/CD

Om deze leeruitkomst aan te tonen maak ik gebruik van meerdere .yaml bestanden, zowel in mijn eigen project als in mijn groepsproject.

### SonarCloud,

SonarCloud gebruik ik om de kwaliteit van mijn applicatie te checken. SonarCloud is een cloudgebaseerde code-analyseservice die is ontworpen om problemen met de codekwaliteit in 25 verschillende programmeertalen te detecteren, waarbij continu de onderhoudbaarheid, betrouwbaarheid en veiligheid van uw code wordt gegarandeerd.

<img src="https://user-images.githubusercontent.com/77282414/168021465-adb4986c-b33f-4071-965f-0ae1360c822e.PNG" width="500">
**Code quality in het begin van het project**
<img src="https://user-images.githubusercontent.com/77282414/174159531-b59fd4c9-305b-4b74-a268-214075e20804.PNG" width="500">
**Laatste code quality voor de oplevering**
  
  
  Voor de CD wordt zowel mijn front-end als mijn back-end deployed op Azure.\
  <a href="https://blue-stone-0b5834e03.1.azurestaticapps.net/">Front-end</a>\
  <a href="https://newsbackend.azurewebsites.net/">Back-end</a>
  
Microsoft Azure, vaak Azure genoemd, is een cloudcomputingservice die wordt beheerd door Microsoft voor applicatiebeheer via door Microsoft beheerde datacenters. Het biedt software as a service (SaaS), platform as a service (PaaS) en infrastructuur as a service (IaaS) en ondersteunt veel verschillende programmeertalen, tools en frameworks, waaronder zowel Microsoft-specifieke als software en systemen van derden.
  
Via een .yaml bestand kan ik bij elke push naar de master branch automatisch configureren dat de nieuwe versie van de applicatie wordt geupload naar Azure.
YAML is een taal voor gegevensserialisatie die vaak wordt gebruikt voor het schrijven van configuratiebestanden. Afhankelijk van wie je het vraagt, staat YAML voor yet another markup language of YAML is geen opmaaktaal , waarmee wordt benadrukt dat YAML voor gegevens is, niet voor documenten.
  Hieronder kan je als voorbeeld zien de workflow die ik in GitHub Actions gebruik om mijn front-end te deployen.
  
 ```yaml
  name: Azure Static Web Apps CI/CD

on:
  push:
    branches:
      - master
  pull_request:
    types: [opened, synchronize, reopened, closed]
    branches:
      - master

jobs:
  build_and_deploy_job:
    if: github.event_name == 'push' || (github.event_name == 'pull_request' && github.event.action != 'closed')
    runs-on: ubuntu-latest
    name: Build and Deploy Job
    steps:
      - uses: actions/checkout@v2
        with:
          submodules: true
      - name: Build And Deploy
        id: builddeploy
        uses: Azure/static-web-apps-deploy@v1
        with:
          azure_static_web_apps_api_token: ${{ secrets.AZURE_STATIC_WEB_APPS_API_TOKEN_BLUE_STONE_0B5834E03 }}
          repo_token: ${{ secrets.GITHUB_TOKEN }} # Used for Github integrations (i.e. PR comments)
          action: "upload"
          app_location: "/" # App source code path
          api_location: "" # Api source code path - optional
          output_location: "dist" # Built app content directory - optional
          ###### End of Repository/Build Configurations ######

  close_pull_request_job:
    if: github.event_name == 'pull_request' && github.event.action == 'closed'
    runs-on: ubuntu-latest
    name: Close Pull Request Job
    steps:
      - name: Close Pull Request
        id: closepullrequest
        uses: Azure/static-web-apps-deploy@v1
        with:
          azure_static_web_apps_api_token: ${{ secrets.AZURE_STATIC_WEB_APPS_API_TOKEN_BLUE_STONE_0B5834E03 }}
          action: "close"
  ```

# Professional

### **Git workflow,**

Om mijn project zo soepel mogelijk te laten lopen, werk in met verschillende branches om mogelijke &#39;merge conflicts&#39; te voorkomen.

**Branches:**

- Master
- Hot Fix
- Release
- Development
- Feature

![GitBranching_3](https://user-images.githubusercontent.com/77282414/168022124-7be833fe-fa9d-4e9f-8496-4d698a69a0b8.png)
  
  
  

