# GP Leeruitkomsten

## **1. Web application** 

    **Learning outcome:**

    You design and build **user-friendly**, **full-stack** web applications**.**

Om deze leeruitkomst aan te tonen in het groepsproject hebben we met zijn alle samen gewerkt om een full-stack web applicatie te maken voor onze stakeholders. 

De opdracht is dat we een kleinere variant moeten maken van een PIM-systeem.

**Wat is een PIM-systeem?**

In een Product Informatie Management (PIM) systeem beheert en ordent een onderneming alle relevante informatie over de producten die zij produceert of verkoopt.

De applicatie van ons groepsproject is geschreven in C# voor de back-end en vue.js voor de front-end. 


###  **PIM front-end**

Repository: <https://github.com/431433/s3-pimfrontend>

De applicatie is eerst ontworpen via schermschetsen in Adobe XD.  Deze hebben we gebruikt om eerst een demo te geven om ons beeld duidelijk te weergeven aan de stakeholders en ervoor te zorgen dat we hun opdracht goed begrijpen.


***<p>Eerste schermschets voor product te creëren</p>***
<img src="https://user-images.githubusercontent.com/77282414/172335896-efbd6490-6595-4826-aac4-0082a4f3f6e5.png" width="650">

***<p>Uiteindelijke versie voor product te creëren</p>***
<img src="https://user-images.githubusercontent.com/77282414/172337541-194c40fa-1829-4c20-b82c-561816b4dd09.png" width="650">


### **PIM back-end**

Repository: https://github.com/PepijnMuskens/ProductService & https://github.com/PepijnMuskens/ApiGateWayWocPim


Om te communiceren met de front-end maken wij gebruik van API call’s. De front-end gebruikt dan een extensie, Axios, om die API call aan te roepen en alle nodige data te laten weergeven of data te versturen via de front-end.

***<p>Axios call van de front-end</p>***
<img src="https://user-images.githubusercontent.com/77282414/172338566-e74807b2-469f-4832-85c6-482e2b9896f6.PNG" width="750">

De back-end werkt met API controllers om de API calls aan te maken, voor de beveiliging maken we ook gebruik van een gateway, waar de link ook hierboven te vinden is. De gateway is een netwerkpunt dat zorgt voor "toegang" tot een ander netwerk indien deze is toegestaan in de gateway. De gateway is dus een netwerkconfiguratie-eigenschap die aangeeft welk netwerkadres de computer mag gebruiken als hij naar een bestemming moet die niet op het lokale netwerk gelegen is.

       if (category != null)
                {
                    Category C = BsonSerializer.Deserialize<Category>(category);
                    return BsonDocument.Parse(System.Text.Json.JsonSerializer.Serialize(C)).ToString();
                }
***Voorbeeld van een klein stukje API die in onze back-end te vinden is***


## **3. Agile method** 
      **Learning outcome**

      You **choose** and implement the most suitable agile software development method for your software project.

Om deze leeruitkomst aan te tonen maken wij als groep gebruik van Agile Scrum.


Op basis van sprints is iedereen bewust van wat er aan de hand is. Op basis van de informatie uit de groepsproject dagen wordt de volgende stap gezet, waar de feedback van de opdrachtgevers en collega's centraal staan. Zo kunnen we snel ons plan van aanpak aanpassen om altijd de goede richting op te gaan, om zo uiteindelijk het ideale product op te leveren voor de opdrachtgevers.


Belangrijk is de stand-up meeting van het team. Elk teamlid beantwoord dan 3 centrale vragen:

 - Wat heb jij bereikt sinds de vorige stand-up?
 - En wat ga jij bereiken tot de volgende stand-up?
 - Wat is je probleem, wat blokkeert je? Heb je hulp nodig?

Indien een teamlid tegen een probleem aan loopt en dan ook hulp nodgi heeft of in het algemeen gaat er iets fout, maken we gebruik van structuren die bedoeld zijn om de problemen zo snel mogelijk te verhelpen. Zie de afbeelding hieronder.

<img src="https://user-images.githubusercontent.com/77282414/172338984-03596553-85a6-4cdf-bb91-7f92a40a17c0.svg" width="750">


Na alle team overleggen of sprint oplevering hebben we in de discord omgeving onze eigen server opgezet, hierdoor kunnen we zelfs als we online werken makkelijk contact houden met elkaar en kunnen we belangerijke documentatie delen met elkaar.

<img src="https://user-images.githubusercontent.com/77282414/172339240-6f1f849a-a73f-409e-8e8a-70078a0975fc.PNG" width="150">



## **5. Cultural differences and ethics** 

      **Learning outcome:**

      You **recognize** and **take into account** cultural differences between project stakeholders and ethical aspects in software development.


Cultuur omvat religie, eten, wat we dragen, hoe we het dragen, onze taal, huwelijk, muziek en is over de hele wereld anders. <a href="https://carla.umn.edu/culture/definitions.html" >Het Center for Advanced Research on Language Acquisition<a/> gaat een stap verder en definieert cultuur als gedeelde gedragspatronen en interacties, cognitieve constructies en begrip die worden geleerd door socialisatie. Cultuur kan dus worden gezien als de groei van een groepsidentiteit die wordt gestimuleerd door sociale patronen die uniek zijn voor de groep.
   
Binnen onze eigen groep hebben we deze culturele verschillen getest doormiddel van een presentatie die met ons is gedeeld via school. In deze presentatie staan vragen gefomuleerd over verschillende aspecten die je misschien tegen kan komen in het leven, bedoeld om onderling discussies te stimuleren.
    
Onze antwoorden:
   ```
      Bas: A, B, C, True, A
      Jenson: A, B, C, True, A
      Pepijn: A, A, C, True, B
      Coen: A, B, C, True, A
      Marijn: C, A, C, False, A
   ```
Er wordt gezegd dat medewerkers vaak meer overeenkomsten hebben dan verschillen, maar die verschillen kunnen soms groter zijn dan de overeenkomsten. Hoewel deze verschillende verschillen een levendiger omgeving kunnen creëren, kunnen ze ook leiden tot meer dan een paar problemen als gevolg van cultuurclash. Gelukkig desondanks dat we sommige vragen verschillend antwoorden, waren we bereid om elkaars andere perspectieve aan te horen en begrepen hun andere zicht op het probleem ook. 
In het begin waren de culturele verschillen wel groter, dit was niks negatiefs, maar het was wel op te merken. Dit werd veroorzaakt door een groepsgenoot die Engels sprak, qua gedrag en  cognitieve constructies waren en weinig verschillen. Het verschil werd dan ook alleen opgemerkt in de taal.


## **6. Requirements and Design** 
      **Learning outcome:**

      You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using **multiple types of test techniques**.
      
Documentatie: <a href="https://github.com/431433/S3-portfolio/tree/main/GP./Documentation">linkje<a/>

Na ons eerste overleg met de opdrachtgever waren we aan de slag gegaan om requirements op te stellen, op deze manier konden we het bestaansrecht van het project doorlopend blijven toetsen door deze altijd te bespreken. Zie het als een vorm van procesbewaking. Hierdoor was het altijd duidelijk wat we moesten doen en hoe de opdrachtgever het ook voor zich zag.


Voor het uiterlijk van de applicatie hebben we zoals eerder vermeld in dit document gebruik van schermschetsen gemaakt in Adobe XD. 
Dit helpt me niet alleen om te verwoorden hoe we van plan zijn een probleem aan te pakken, maar door hardop op papier te denken, kan iedereen - ikzelf, mijn team en de opdrachtgever - zien hoe ideeën beginnen, evolueren en uiteindelijk tot de oplossing waar we hebben allemaal naar toe gewerkt vorm krijgt.


<img src="https://user-images.githubusercontent.com/77282414/173248764-38eb3638-acdc-423d-82a6-c4aef91dbb43.png" width="500">

Het delen van schetsen, zowel intern als extern, maakt samenwerking en creativiteit binnen het  team mogelijk, wat leidt tot een gedeeld begrip en afstemming van begin tot eind. Hierdoor kunnen we geen miscommunicatie oplopen met de opdrachtgever en kunnen we makkelijk feedback krijgen om mogelijke verbeteringen toe te voegen. Door het gebruik van de Adobe XD feature, prototyping, konden we ook Black Box Testing gebruiken om de structuur en ontwerp optimaal te testen.


<img src="https://user-images.githubusercontent.com/77282414/173249170-6aa650cf-d25f-490b-bafd-ce2cde13553a.PNG" width="250">


Om onze website ook mee te testen heb ik de website door een performance testing website gehaald. (https://gtmetrix.com/reports/kind-sky-062238903.1.azurestaticapps.net/mYJSRQvH/)
Performance Testing is een softwaretest proces dat wordt gebruikt voor het testen van de snelheid, responstijd, stabiliteit, betrouwbaarheid, schaalbaarheid en resourcegebruik van een softwaretoepassing onder een bepaalde werkdruk. Het belangrijkste doel van een performance is het identificeren en elimineren van de prestatieknelpunten in de softwaretoepassing.


Om merge-conflict te voorkomen werkten we ook met verschillende branches, op deze manier konden we eerst elkaar codes checken en testen voordat deze automatisch werd deployed via de master branch naar Azure.

<img src="https://user-images.githubusercontent.com/77282414/173251063-a283d762-1a96-4929-a0f5-1285c0e213df.PNG" width="750">


## **7. Business processes** 
      **Learning outcome:** 

      You analyze and describe **simple** business processes that are **related** to your project.


Business process reengineering (BPR) is gericht op het verbeteren van de efficiëntie en effectiviteit van de processen die binnen en tussen organisaties bestaan.


<img src="https://user-images.githubusercontent.com/77282414/173250075-004a74d8-941f-4d71-9440-62330efd53b2.png" width="300">



## **8. Professional** 
      **Learning outcome:**

      You act in a **professional manner** during software development and learning.

Dit semester hebben we voor het eerst echt de Agile Scrum manier van werken gevolgd, we hielden dagelijkse stand-ups op groepsproject dagen, sprintreview, sprintretrospectief etc. In het begin verliep het houden van de dagelijkse stand-ups wel stroef maar na kort overleg met een van onze docenten (Marc) kwam hij met het idee om het persoonlijker te maken maar wel concreet te zijn met de stand-ups. Zo konden we elkaar beter leren kennen en vonden we het minder moeilijk om het te zeggen als iets niet lukt. Hierdoor konden we samen mogelijk tot een oplossing komen.


Dit semester werkten we in sprints van 3/4 weken, na elke sprint was er contact met de opdrachtgever voor een korte oplevering/update van het project en de bijhorende stand van zaken. Ik mailde dan altijd onze opdrachtgever om een vergadering in te plannen. Na zo'n oplevering/update hielden we in discord de dag erna een retrospective om alles na te bespreken en het netjes bij te houden in feedpulse.

In discord hielden we ook altijd contact over opkomende vergaderingen of eventuele vertragingen die we ervaren met het OV of files, hier hadden we dan ook een apart 'kanaal' voor die we 'meetings'noemde, zo waren er ook kanalen voor notities of off-topic vragen. Op deze manier konden we makkelijk overzicht houden en makkelijk documentatie terug vinden.

In het begin merkte ik wel dat ik minder makkelijk communiceerde met mijn groepje, we overlegten een plan van aanpak met elkaar en daar bleef het meestal bij. Pas na ongeveer 5 weken ging de communicatie soepeler naar mijn gevoel en kon ik ook vragen stellen over mijn indivuele project, we waren niet meer genoodzaakt om puur en alleen te praten over het groepsproject en verder niks. Richting het einde van dit semester was de communicatie voor mij perfect, ik durfte gesprekken te starten en kon mijn mening geven als ik het niet ergens mee eens was, of als ik dacht dat er een betere manier was.
