# Progressive enhancement features

verbeteringen nodig = *

### 1.Afbeeldingen

Het niet laden van afbeeldingen is uiteraard enorm jammer aangezien dat voor een groot deel is waar mijn web applicatie over gaat. Echter zou je dan wel nog gewoon de titels van de foto’s kunnen zien en kan je er nog steeds op klikken voor een bijbehorende beschrijving.

Alles werkt in Principe. Titels worden weergegeven en de bijbehorende beschrijvingen zie je gewoon

![](https://lh3.googleusercontent.com/HpOj6_8mq2zr55eZX1eQGe3WYnZD9eeDxEzp-5OWGAz1tuQ4M7Ur3xM9aCj4bSaa7Vl7BDSxghLwc2cMbzwlvI4UVnfffqzI2RMvLl1DiVAl4p1jqtqEfQJsw9q6Xyxl8MKtXh6kvJlmKXWcYZX-IQ0w-Uj2ZPRnvoAZlStMzjPaJIAO14ES5IWKN2AVgznHrtLVaeA9zd5_YfSdGI1hPoXacEQNbdsRXdhKl9lSowJwFm288FnX2ibzCX5xYZtJSsQh02LQW8_cJJSVXo3Tv5t-AvrEoTIK0S8fWAmpbiLjCut4dtVI8nxy2MLIwetX2mHeRpUfLE4YzNq6jT5VeP_CGTogSI4tlAnAuP9w9ZC56sYVxVQbhnjReBoGOsn-DdaaATPzxk8Uf48CuCKbTEIBOg_KmX13eq-n3tmuiWr1JtscGCl4_VV-V9mRowfrdXXI8sIQ03dTJPAyD9_yL-nIGKb-9ZoTMIvs6fEqq1fPljWZTb_KWw9FyPAl2O-Ebk510vQZ2vnLYhUNw2LRvlFaah6Zz_ie-9ac9IP3lgIQ199Pc_9ROMklcYwfSpledwiD8jg5qwYPCQ0U2zB6VvSBpbtyLU5eR0_hg0s=w525-h290-no)

### 2.Custom fonts.

De standaard font is een google font. Wanneer die niet werkt heb ik een aantal fallback fonts. Het gebruik van custom fonts vertraagt mijn pagina niet echt. De pagina zelf laad snel, alleen de content laad traag. Indien ik een zwaardere website zou moeten laden dan had ik gebruik kunnenmaken van “font-display: swap;” Dit zorgt er voor dat de custom font pas geladen wordt nadat de pagina geladen is. 

	font-family { 'Raleway', sans-serif, serif;}

### 3.Javascript *

Zonder Javascript werkt mijn pagina niet en wordt er niks weergegeven. Ik zie hier niet een
oplossing voor aangezien mijn pagina volledig draait op generated content.

Oplossing: Server side renderen

### 4.Kleur*

Mijn pagina ziet er goed uit voor alle vormen van kleurenblindheid. Echter is het iets minder makkelijk om bepaalde focus en hover states goed te zien. Dit zou verbeterd kunnen worden.

Met de Funkify extensie voor Chrome heb ik de verschillende vormen van kleurenblindheid getest. Echter kan de kleurentest om bepaalde redenen niet de achtergrond (rood) in een grijstint weergeven. Mogelijk omdat ik die met een css truuc heb gemaakt. 

![kleurenblindheid test](https://lh3.googleusercontent.com/7ydn2Ri9hw0j-p5bvji9YZYGRbk0brkboatqStbR_jkyBtIU6bWpN1CMfQ5tddY1YGHdgZRZ-V4_SW7xyzMWkkJfnJuFJPHbf8EUB3OaSUAEeFsgdg6l7ATMKZ68ni8ahb6FdcnxNlJ4xG5StCcvKlnTLwKOiGrL8aMT8kXYukgYEcrBMbaAC8qITkg2ZSxtxgHArVkmQ_pgBRxXdW-y6dzq4C6SLW9Vj9p84mAc6ViV_Bf6ysGlRiUhKpotDX0YYIrxougxt8oD9vHC0wt7XT4o7DJVWvV4ICweHahb5p-ZfekLkijdqmz_8qdFn6CkDSvqW4-0oVFFwaWVYztRPGWucyXBLXCT8z3OcUUea-Ng0Bgy_jHlPazZwmdXgXq0si07134Vlu_VLcgpMAB34s2xZZOrZc43jd4H1Z-8BAJYUSmqZ8ilYhoZYQ3HuHgRqav8B8C0K3VGkxm3irXC5UZ7S0SLiDFRa8S1VZmsxYg93zaON7dqAfkiFnMTFQXJnAYaPgsIR7J7FoDyKgSY6fBjrbmSxaC_wTei4PJX2o66AIV58xpulYR_tFaY19xD3tVZMybTsZa3dhi4vWdNhNY9-rsA8AHUFE5pPno=w656-h270-no)


### 5.Breedband internet *

Op langzaam internet is mijn pagina erg traag. In totaal moeten er 935 afbeeldingen worden
ingeladen. Op normaal internet doet hij dit goed maar op traag internet doet hij er minuten over.

Oplossing: Een oplossing zou zijn om telkens 10 a 20 resultaten in te laden, en on scroll nog meer resultaten in teladen.

### 6.Cookies

Zonder cookies doet mijn website het prima omdat ik zelf niks met cookies doe

### 7.LocalStorage

Het uitzetten van local storage doet net als cookies niet zo heel veel met mijn pagina. Echter zou het toevoegen van een caching optie mijn pagina mogelijk een stuk sneller laadbaar maken. Dit hangt er echter van af of de data die wordt opgehaald van Adamlink wel cacheerbaar is. 

### 8.Muis/Trackpad *

Onder muis / trackpad kan je alleen door de navigatiebalk van mijn pagina tabben. Je kan
momenteel niet een van de gegenereerde plaatjes selecteren. 

Oplossing: er is momenteel geen href gespecificeerd voor mijn generated content. Deze ga ik nu wel toevoegen zodat de elementen gefocust kunnen worden. De volgende stap is om te zorgen dat wanneer ik op een link klik, de focus op de gegenereerde text komt te staan. Hierdoor zal een screenreader de juiste tekst gaan voorlezen.

**Oplossing geimplementeerd**
Linkjes en Href aan gegenereerde content toegevoegd. On click komt focus op de text 
beschrijving te staan. Duidelijke focus states gemaakt. 


# extra research

### Wifi hotspots/https
Het is belangrijk dat wanneer de web applicatie live gaat dit op een beveiligd netwerk is. Alle links moeten daarom op https staan en er moet een ssl certificaat zijn van de hosting provider.

Een andere beveiliging maatregel is het toevoegen van een webapplicatie firewall. Voorbeelden van firewalls zijn: Cloudfare, Incapsula, Cloudbric en Akamai.

Momenteel is het niet van groot belang dat mijn applicatie beveiligd wordt aangezien het niet met vertrouwelijke data omgaat en er ook geen informatie van de gebruiker opslaat. 

### Content blockers
Wanneer gebruikers een Javascript blocker zouden gebruiken dan zou mijn pagina onbruikbaar zijn. Hier is helaas niet snel een oplossing voor te vinden tenzij de content server side gerenderd zou worden. Dan zou de content mogelijk wel nog kunnen verschijnen. 

Alle zoek en display elementen zouden niet meer werken omdat die Javascript nodig hebben. Echter 
werkt de website verder wel nog gewoon.

### CDN’s
CDN zorgen er voor dat content op je pagina sneller wordt opgehaald en weergegeven. Dit komt doordat de informatie van de meest dichtstbijzijnde server (voor de gebruiker) wordt opgehaald. Dit zorgt er voor dat de laadtijd een stuk sneller wordt omdat de informatie niet uit één, maar uit twee servers komt. 

![CDN](https://seohackercdn-seohacker.netdna-ssl.com/wp-content/uploads/2013/08/advantages-self-hosted-cdn.jpg?x68951)

Dit zou interessant kunnen zijn voor mijn pagina wanneer het live en gehost zou worden. Echter vraag ik me af of dit erg veel zin heeft omdat ik eigenlijk alle informatie van Adamlink ophaal. De informatie staat niet op mijn pagina server opgeslagen. Daarom zou het zo kunnen zijn dat een CDN in dit geval niet echt zou werken.

### Ad blockers

Ik heb zelf ad blockers geïnstalleerd en deze hebben geen effect op het gebruik van mijn
webapplicatie.