## Inhoud
- [Web Application](#web-application)
- [Software Quality](#software-quality)
- [CI/CD](#cicd)
- [Professional](#professional)
<hr/>

# Web Application

Om deze leeruitkomst aan te tonen heb ik (tot nu toe) 1 fullstack applicatie gemaakt waar mensen nieuws van over de hele wereld kunnen lezen en commentaar op deze artikelen kan geven.

## Applicaties:

- News front-end
- News back-end

## News front-end

Repository: [News front-end](https://github.com/431433/S3-NewsFrontEnd)

### **Losse pagina,**

In mijn front-end applicatie begin je op een losse pagina die uitwisselt met verschillende componenten, op basis van wat de gebruiker wilt zien.

(Afbeelding)

### **Accounts,**

Voor het gebruik van accounts, wil ik Auth0 daarvoor gebruiken. Met deze accounts kunnen gebruikers commentaar achterlaten op artikelen.

![Auth0Login](https://user-images.githubusercontent.com/77282414/168020607-d229e649-9238-4d2e-b462-d51784e94ae5.PNG)
(comment afbeelding toevoegen)

## News back-end

Repository: [News back-end](https://github.com/431433/S3-NewsBackEnd)

### **NewsAPI,**

Om alle artikelen op te halen maak ik gebruik van de NewsAPI.

![NewsAPI](https://user-images.githubusercontent.com/77282414/168020985-ff9c9ca6-837a-4916-ad8b-fb433427ea77.PNG)


### **Interactie,**

Om de gebruikers commentaar achter te laten, maak ik gebruik van een apart lopende database. Deze houdt bij welke artikelen het commentaar hoort en van welke gebruiker deze afkomt.

(Afbeelding)


# Software Quality

Softwarekwaliteit is een abstract begrip. Zijn aanwezigheid kan moeilijk te definiëren zijn, maar zijn afwezigheid kan onmiddellijk worden gezien. Dus, in de zoektocht naar het verbeteren van de softwarekwaliteit, moeten we eerst de definitie van softwarekwaliteit begrijpen. <a href="https://en.wikipedia.org/wiki/Software_quality">Wikipedia</a> beschrijft de softwarekwaliteit als volgt:

“In de context van software-engineering meet softwarekwaliteit hoe goed de software is ontworpen (kwaliteit van ontwerp) en hoe goed de software overeenkomt met dat ontwerp (kwaliteit van conformiteit). Het wordt vaak omschreven als de ‘fitness for purpose’ van een stukje software.”

Er zijn veel variaties op de definitie van softwarekwaliteit, afhankelijk van het gezichtspunt (ontwikkelaar, eindgebruiker, management...), maar als je de bovenstaande definitie bekijkt, vraagt "fitness for purpose" zich af of de software wel doet wat die moet doen. Dat zijn de kenmerken die wij als eindgebruikers zien. De kwaliteit van het ontwerp en de kwaliteit van conformiteit met dat ontwerp zijn gerelateerd aan interne aspecten van de software, waarvan we sommige kunnen zien, zoals de navigatie van de gebruikersinterface, de plaatsing van bedieningselementen, enzovoort.

Deze gebruikersinterface heb ik doormiddel van verschillende UI ontwerpen getest. Meerdere pagina's in mijn project zijn allemaal ontworpen met andere css en andere plaatsing van bedieningselementen. Zo kon ik een klein onderzoekje doen om te kijken wat er als het beste wordt ervaren als exterene gerbuiker.
Deze kan je hier terug vinden: **LINKJE**

# CI/CD

Om deze leeruitkomst aan te tonen maak ik gebruik van meerdere .yaml bestanden, zowel in mijn eigen project als in mijn groepsproject.

### SonarCloud,

SonarCloud gebruik ik om de kwaliteit van mijn applicatie te checken.

![SonarCloud](https://user-images.githubusercontent.com/77282414/168021465-adb4986c-b33f-4071-965f-0ae1360c822e.PNG)


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

