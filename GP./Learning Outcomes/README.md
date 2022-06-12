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


## **6. Requirements and Design** 
      **Learning outcome:**

      You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using **multiple types of test techniques**.


## **7. Business processes** 
      **Learning outcome:** 

      You analyze and describe **simple** business processes that are **related** to your project.


## **8. Professional** 
      **Learning outcome:**

      You act in a **professional manner** during software development and learning.


