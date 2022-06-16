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


Dit semester was de eerste keer dat ik heb gewerkt met een full stack applicatie. Het begin hiervan was dan ook voor mij persoonlijk heel moeilijk, ik kwam niet makkelijk opgang om de verbinding te leggen. Qua de nieuwe programmeer taal, Vue, te leren ging dat wel veel soepeler en kreeg ik makkelijk onder de knie en kon zo ook makkelijk een mooie front-end neerzetten gebaseerd op onze schermschetsen. 
In de toekomst moet het opzetten van een full stack project veel makkelijker verlopen met de kennis die ik heb opgedaan dit semester. Het ontwerpen heb ik vorig semester al voor een groot deel in gespecialiseerd omdat dit mij erg aantrok, ik heb toen ook geleerd om met Adobe XD te werken. Dit semester heb ik echter geleerd hoe je een soort interactieve presentatie van kan maken, zo dat je makkelijk kan laten zien welke knop je naar welke pagina brengt. Dit heeft uiteindelijk ook geholpen met het presenteren van de schermschetsen aan de opdrachtgever.


## **3. Agile method** 
      **Learning outcome**

      You **choose** and implement the most suitable agile software development method for your software project.

Om deze leeruitkomst aan te tonen maken wij als groep gebruik van Agile Scrum.


Op basis van sprints is iedereen bewust van wat er aan de hand is. Op basis van de informatie uit de groepsproject dagen wordt de volgende stap gezet, waar de feedback van de opdrachtgevers en collega's centraal staan. Zo kunnen we snel ons plan van aanpak aanpassen om altijd de goede richting op te gaan, om zo uiteindelijk het ideale product op te leveren voor de opdrachtgevers.


Belangrijk is de stand-up meeting van het team. Elk teamlid beantwoord dan 3 centrale vragen:

 - Wat heb jij bereikt sinds de vorige stand-up?
 - En wat ga jij bereiken tot de volgende stand-up?
 - Wat is je probleem, wat blokkeert je? Heb je hulp nodig?

Indien een teamlid tegen een probleem aan loopt en dan ook hulp nodig heeft of in het algemeen als er iets fout gaat, maken we gebruik van structuren die bedoeld zijn om de problemen zo snel mogelijk te verhelpen. Zie de afbeelding hieronder.

<img src="https://user-images.githubusercontent.com/77282414/172338984-03596553-85a6-4cdf-bb91-7f92a40a17c0.svg" width="750">


Na alle team overleggen of sprint oplevering hebben we in de discord omgeving onze eigen server opgezet, hierdoor kunnen we zelfs als we online werken makkelijk contact houden met elkaar en kunnen we belangerijke documentatie delen met elkaar. Laterna is wel gebleken dat discord niet zo veilig is als ik in eerste instantie dacht, dus in de toekomst zal ik deze communicatie software waarschijnlijk niet nog een keer gebruiken.

<img src="https://user-images.githubusercontent.com/77282414/172339240-6f1f849a-a73f-409e-8e8a-70078a0975fc.PNG" width="150">

Agile werken was ook voor de eerste keer dit semester. De scrum manier van werken kende ik al van vorige semester, daar waren toen vooral de rollen belangrijk onderling. Dit semester moesten we die rollen verdeling weer los laten. In het begin voelde dit wel raar, maar maakte het wel makkelijker om bewust te zijn van wat er gaande was in het hele project. De een was niet alleen bezig met de front-end of de ander met de back-end, er werd onderling gewisseld. Hierdoor was iedereen in staat om elkaar te helpen, want ze wisten er van af en of waar ze mee bezig waren. 
Verdere ontwikkeling in het agile werken bleef in het begin wel hangen, we hadden in het begin dan ook moeite met het houden van stand-ups, tot wij deze lichtelijk aanpasten zodat deze ideaal pasten bij onze werkwijze. Wij hielden ze compact en concreet, als iemand kon helpen gingen die er dieper op in samen en kwamen later na met een korte reflectie wat het probleem was. 
Daarnaast hebben we ook nog gewerkt, onbewust wel, met "over-the-shoulder" code review. Dit is de meest voorkomende en informele code-review. Een "over-the-shoulder" recensie is eigenlijk precies zoals het klinkt. Ik zou een stuk code kunnen schrijven en Bas kijkt mee, ik leg dan aan Bas uit wat ik aan het doen ben en welk effect het zal gaan hebben.
Voor de volgende keer dat ik weer ga werken met agile wil het de stand-ups meteen oppakken en kijken naar mogelijke uitbreidingen die we kunnen toevoegen aan onze werkwijze en communicatie. Zo kan je kijken of misschien Kanban wat voor ons is, hiermee kan je makkelijk signaleren wanner iets nodig is en kan gebruikt worden om van alles in het leven te organiseren.


## **5. Cultural differences and ethics** 

      **Learning outcome:**

      You **recognize** and **take into account** cultural differences between project stakeholders and ethical aspects in software development.


Cultuur omvat religie, eten, wat we dragen, hoe we het dragen, onze taal, huwelijk, muziek en is over de hele wereld anders. <a href="https://carla.umn.edu/culture/definitions.html" >Het Center for Advanced Research on Language Acquisition<a/> gaat een stap verder en definieert cultuur als gedeelde gedragspatronen en interacties, cognitieve constructies en begrip die worden geleerd door socialisatie. Cultuur kan dus worden gezien als de groei van een groepsidentiteit die wordt gestimuleerd door sociale patronen die uniek zijn voor de groep.
   
Binnen onze eigen groep hebben we deze culturele verschillen getest doormiddel van een presentatie die met ons is gedeeld via school. In deze presentatie staan vragen gefomuleerd over verschillende aspecten die je misschien tegen kan komen in het leven, bedoeld om onderling discussies te stimuleren.
    
Deze discussies hebben we helaas wel maar met zijn 4en kunnen houden in persoon, de 5e was online te vinden en 2 zijn er gestopt. De discussies die hebben we gehouden waren vrijwel alleen om te kijken of hun misschien een andere onderbouwing hadden van hun antwoorden. De antwoorden die we namelijk gaven kwamen voor een groot gedeelte overeen. Tijdens deze discussies kon je wel merken dat we open waren en eerlijk durfde te antwoorden, als ik dit zou moeten vergelijken met het begin van dit semester was dit een grote vooruitgang. Zeker ben ik niet of dit gevoel terecht was, maar de omgeving, toon in de stem en de sfeer in het algemeen waren vrolijker en meer gerust.
   
Er wordt gezegd dat groepsgenoten vaak meer overeenkomsten hebben dan verschillen, maar die verschillen kunnen soms groter zijn dan de overeenkomsten. Hoewel deze verschillen een levendiger omgeving kunnen creëren, kunnen ze ook leiden tot meer dan een paar problemen als gevolg van cultuurclash. Gelukkig desondanks dat we sommige vragen verschillend antwoorden, waren we bereid om elkaars andere perspectieve aan te horen en begrepen hun andere zicht op het probleem ook. In het begin waren de culturele verschillen wel groter, dit was niks negatiefs, maar het was wel op te merken. 
Hoe een cultuur er ook uitziet, één ding is zeker: culturen veranderen altijd. Cultuur lijkt de sleutel te zijn geworden tot onze onderling verbonden wereld, die bestaat uit zoveel etnisch diverse samenlevingen, maar ook met conflicten over religie, etniciteit, morele overtuigingen en in wezen, de elementen waaruit cultuur bestaat.
   
Mensen kunnen oorlog voeren als hun culturen niet overeen komen, nou is dat natuurlijk gelukkig niet overal het geval. Wel komt het vaak voor dat mensen worden buitengesloten door deze verschillen. Mensen moeten het nog leren te omarmen dat we verschillend zijn. In het einde van dit semester, eigenlijk al best wel laat, was het pas goed te merken dat wij als groepsgenoten helemaal niet zo heel veel verschillen. Inderdaad met de een praat je net wat anders of heb je het over een ander onderwerp, maar dat zal altijd zo blijven.



## **6. Requirements and Design** 
      **Learning outcome:**

      You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using **multiple types of test techniques**.
      
Documentatie: <a href="https://github.com/431433/S3-portfolio/tree/main/GP./Documentation">linkje<a/>

Na ons eerste overleg met de opdrachtgever waren we aan de slag gegaan om requirements op te stellen, op deze manier konden we het bestaansrecht van het project doorlopend blijven toetsen door deze altijd te bespreken. Zie het als een vorm van procesbewaking. Hierdoor was het altijd duidelijk wat we moesten doen en hoe de opdrachtgever het ook voor zich zag.


Voor het uiterlijk van de applicatie hebben we zoals eerder vermeld in dit document gebruik van schermschetsen gemaakt in Adobe XD. 
Dit helpt me niet alleen om te verwoorden hoe we van plan zijn een probleem aan te pakken, maar door hardop op papier te denken, kan iedereen - ikzelf, mijn team en de opdrachtgever - zien hoe ideeën beginnen, evolueren en uiteindelijk tot de oplossing waar we hebben allemaal naar toe gewerkt vorm krijgt.


<img src="https://user-images.githubusercontent.com/77282414/173248764-38eb3638-acdc-423d-82a6-c4aef91dbb43.png" width="500">

Het delen van schetsen, zowel intern als extern, maakt samenwerking en creativiteit binnen het  team mogelijk, wat leidt tot een gedeeld begrip en afstemming van begin tot eind. Hierdoor kunnen we geen miscommunicatie oplopen met de opdrachtgever en kunnen we makkelijk feedback krijgen om mogelijke verbeteringen toe te voegen. Door het gebruik van de Adobe XD feature, prototyping, konden we ook Black Box Testing gebruiken om de structuur en ontwerp optimaal te testen.

Black Box Testing is een softwaretestmethode waarbij de functionaliteiten van softwareapplicaties worden getest zonder kennis te hebben van de interne codestructuur, implementatiedetails en interne paden. Black Box Testing richt zich voornamelijk op input en output van softwareapplicaties en is volledig gebaseerd op softwarevereisten en specificaties. Het wordt ook wel gedragstesten genoemd.

<img src="https://user-images.githubusercontent.com/77282414/173249170-6aa650cf-d25f-490b-bafd-ce2cde13553a.PNG" width="250">


Om onze website ook mee te testen heb ik de website door een performance testing website gehaald. (https://gtmetrix.com/reports/kind-sky-062238903.1.azurestaticapps.net/mYJSRQvH/)
Performance Testing is een softwaretest proces dat wordt gebruikt voor het testen van de snelheid, responstijd, stabiliteit, betrouwbaarheid, schaalbaarheid en resourcegebruik van een softwaretoepassing onder een bepaalde werkdruk. Het belangrijkste doel van een performance is het identificeren en elimineren van de prestatieknelpunten in de softwaretoepassing.

Al deze tests heb ik gebruikt om zo’n duidelijk beeld te krijgen wat de opdrachtgever nou van ons vraagt. De prestatie test heb ik dan gebruikt om te checken of onze website niet te zwaar is en daardoor als erg traag wordt ervaren. Dit allemaal heeft geholpen bij het duidelijk beeld van de opdracht en gaf ook een duidelijk beeld waar de focus op lag. Bij elk toekomstig project wil ik ook deze manier van communicatie houden.
   
   
## **7. Business processes** 
      **Learning outcome:** 

      You analyze and describe **simple** business processes that are **related** to your project.


Een bedrijfsproces is een reeks gerelateerde, gestructureerde activiteiten en stappen die worden uitgevoerd door de mensen of apparatuur in een organisatie om de basisdoelen van de organisatie te bereiken, zoals winstmaximalisatie en klanttevredenheid.

Bedrijfsprocessen kunnen vele malen worden herhaald op alle organisatieniveaus en zijn al dan niet zichtbaar voor de klanten.

Een bedrijfsproces wordt vaak beschouwd als een stroomdiagram of workflow van logische stappen, en het dient als een primaire basis voor verschillende gerelateerde ideeën zoals bedrijfsprocesbeheer, procesoptimalisatie, procestoewijzing, processimulatie, procesautomatisering, enz.

***Een workflow voor taakbeheer, ook wel workflowprocesbeheer genoemd, is een manier om een reeks kleinere taken te versnellen om een groter doel te bereiken. In ons geval hebben we deze workflow gebruikt om alle stappen duidelijk op papier te hebben die we moeten onderlopen om de kwaliteit van onze code hoog te houden. In de workflow, die je hier onder kan zien, kan je alle stappen volgen die we hebben gebruik dit semester. Zodra er een nieuw backlog item is gaat het aangewezen persoon beginnen met de rest van de workflow. De reviews stukken die te zien zijn in de workflow wordt gedaan door andere groepsgenoten.***
<img src="https://user-images.githubusercontent.com/77282414/173546681-7e53a6c8-7d97-45e4-a64a-d942c9a48720.png" width="600">
  
De workflow die hierboven staat is geen business proces, wat wij hadden gemaakt wordt eerder geclassificeerd als een technisch proces. Bij een business proces kan je deze beter beeld geven via ‘zwembaden’. Een zwembad vertegenwoordigt belangrijke deelnemers in een proces. Verschillende zwembaden kunnen verschillende bedrijven of afdelingen zijn, die toch bij het proces betrokken zijn. Zwembanen binnen een zwembad tonen de activiteiten en stromen voor een bepaalde rol of deelnemer, en definiëren zo wie verantwoordelijk is voor welk deel van het proces. In de toekomst moeten we dan ook eerder beginnen met zulke modellen om de activiteiten beter beeld te geven zowel aan de opdrachtgever als voor ons zelf. Deze business proces modeling notering vraagt tijd en energie, maar die inspanning wordt uiteindelijk dus beloond met veel meer inzicht en vooruitgang. Het doel van bedrijfsprocesmodellering is het creëren van een cyclus van continue verbetering. De te nemen stappen zijn: modelleren, implementeren, uitvoeren, verifiëren en optimaliseren. Het business proces speelt daarbij een belangrijke rol.

![bpmn-zwembaan](https://user-images.githubusercontent.com/77282414/174150516-212282ec-7df7-43f4-b5ec-64259f17e9b2.png)
***Swim lanes***

## **8. Professional** 
      **Learning outcome:**

      You act in a **professional manner** during software development and learning.

Dit semester hebben we voor het eerst echt de Agile Scrum manier van werken gevolgd, we hielden dagelijkse stand-ups op groepsproject dagen, sprintreview, sprintretrospectief etc. In het begin verliep het houden van de dagelijkse stand-ups wel stroef maar na kort overleg met een van onze docenten (Marc) kwam hij met het idee om het persoonlijker te maken maar wel concreet te zijn met de stand-ups. Zo konden we elkaar beter leren kennen en vonden we het minder moeilijk om het te zeggen als iets niet lukt. Hierdoor konden we samen mogelijk tot een oplossing komen.


Dit semester werkten we in sprints van 3/4 weken, na elke sprint was er contact met de opdrachtgever voor een korte oplevering/update van het project en de bijhorende stand van zaken. Ik mailde dan altijd onze opdrachtgever om een vergadering in te plannen. Na zo'n oplevering/update hielden we in discord de dag erna een retrospective om alles na te bespreken en het netjes bij te houden in feedpulse.

In discord hielden we ook altijd contact over opkomende vergaderingen of eventuele vertragingen die we ervaren met het OV of files, hier hadden we dan ook een apart 'kanaal' voor die we 'meetings'noemde, zo waren er ook kanalen voor notities of off-topic vragen. Op deze manier konden we makkelijk overzicht houden en makkelijk documentatie terug vinden.

In het begin merkte ik wel dat ik minder makkelijk communiceerde met mijn groepje, we overlegten een plan van aanpak met elkaar en daar bleef het meestal bij. Pas na ongeveer 5 weken ging de communicatie soepeler naar mijn gevoel en kon ik ook vragen stellen over mijn indivuele project, we waren niet meer genoodzaakt om puur en alleen te praten over het groepsproject en verder niks. Richting het einde van dit semester was de communicatie voor mij perfect, ik durfte gesprekken te starten en kon mijn mening geven als ik het niet ergens mee eens was, of als ik dacht dat er een betere manier was.
   
In het begin van de proftaak hebben we ook veel geleerd over TypeScript samen met Vue extensies. Vooral dat deze niet samen werken, hierdoor hebben we helaas onze volledige front-end opnieuw moeten doen toen we van een Vue project met TypeScript gegaan waren naar een Vue project met Javascript. We hebben door deze switch wel geleerd hoe we via command lines een project kunnen aanmaken waar de meest gebruikte extenties, zoals vue router, al in zitten. Dit scheelde veel werk waardoor we een niet al te grote achterstand opliepen.
   
Om merge-conflict te voorkomen werkten we ook met verschillende branches, op deze manier konden we eerst elkaar codes checken en testen voordat deze automatisch werd deployed via de master branch naar Azure. Deze stappen zijn ook terug te vinden in leerdoel 7, bij de onderste afbeelding, waar wij deze workflow hebben uitgewerkt.

<img src="https://user-images.githubusercontent.com/77282414/173251063-a283d762-1a96-4929-a0f5-1285c0e213df.PNG" width="750">
   
De workflow die hierboven wordt weergeven is van onze front-end, de bedoeling was een Personal branching Git workflow. Dat is vergelijkbaar met feature branching, maar in plaats van één enkele vertakking per functie, is het per ontwikkelaar. Deze aanpak werkt goed als teamleden aan verschillende functies en bugs werken. Elke gebruiker kan terug mergen naar de hoofdbranch wanneer zijn of haar werk gedaan is. De bedoeling begon goed, maar het daadwerkelijk uitvoeren is minder gelukt. 
‘Persoonlijke vertakking’ is handig voor langlopende functies die mogelijk niet in een enkele releasecyclus passen. Deze strategie kan goed werken voor kleine teams waarin elk teamlid zijn eigen onderdeel van de applicatie ontwikkelt, wat voor ons grotendeels ook het geval was. 
Het idee was goed bedoeld dit semester en deze git workflow is ook heel handig lijkt mij. In de toekomst wil ik deze dan dus ook zeker nog een keer gebruiken, maar dan juist. Niet meer dat een nieuwe branch wordt gemaakt vanuit een andere feature branch zoals bij ons is gebeurd. Er moet een duidelijk overzicht blijven van de branches.

