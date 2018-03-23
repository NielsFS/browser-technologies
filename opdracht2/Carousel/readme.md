# Menu component

[pagina](https://nielsfs.github.io/browser-technologies/opdracht2/Carousel/carousel.html)

## Wat doet dit component?

Dit carousel scrollt tussen 3 vensters. In die vensters heb ik tekst geplaatst, maar foto's en andere dingen kunnen er ook in geplaatst worden. Onderin de carousel staan 3 bolletjes waar op geklikt kan worden. De carousel verplaatst zich dan naar de corresponderende slide. Om de carousel feature volledig te kunnen gebruiken moet je wel een nieuwere browser hebben. 


## Eerste ruwe schets:

![schets](https://lh3.googleusercontent.com/ORxTWszU_1A4pOx74U0UcPAO1dSVwxJigCcJHhNx4ODt3cFgERGjczBXbK7m824PyBbiAJrCMefYXTBiUapkB5V4lsOhIelghP-YUb_whL70ltZlSt0xtCyHi8EZzWUzOcl5QHPwLz3ElCCyVOxhDA_LEelI6RwSygWulTsJk-FeMY1EyviYSP1cCnZBanD1Jp99Gt-ga0Y-2BivAl31V_9oEiabphdHySgxL25nb0dbjlgWYtYaQvuufD2VkXyJ1RcApYXF0FLMqpf_q53Vg3g-SgMVF0M7uKfiaGSH3LahaXUA9O5eDF-0wSlmdJlto3UKp-x-hqap8Z3hY0uLimuAPShnkG_yYscK5PNgfuNziKfhOWFT1fE6aZZiuY-ngnYhqs_tedVxbHFWIZO9Uu_2bPE9iLrJYrItUusahslZjZaLeTHYfwDuBJwS6NbEGQGyshXqF56Cc5KgzTkzOhBaT7s46KO5I-UCrPWY8vP7NwHXlUvgY878qBJF9s_olQmZvSIf_NCfJteIJZVz9QZjiT0C3kNIhwUN7gkkU6zETg72DbYryiaJG3rqQPxxrzaedcW3aV8Pex1-yYZGVzZJ0Ms8O8NS7M2VJOw=w1224-h1632-no)


## Bronnen & artikelen

#### caniuse.com
[link](www.caniuse.com)
#### presentatie voorhoede over progressive enhancement (weekly nerd)
[link](https://moodle.cmd.hva.nl/mod/url/view.php?id=19943)
#### MDN (implement feature detection)
[link](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/Feature_detection)
#### 
[link](https://css-tricks.com/on-target/)

## Welke Browsers/ devices ondersteunen dit

Alle browsers en devices ondersteunen mijn component omdat hij altijd terug valt op de basis html die gewoon leesbaar is. Wanneer een browser niet :target ondersteund dan wordt de carousel een gestylede lijst met alle stukken tekst daar in. 

Er is een test toegevoegd die checkt of de browser QuerySelector/QuerySelectorAll ondersteund. Wanneer dit niet het geval is dan wordt de Javascript niet uitgevoerd en valt het component terug op de basis HTML en CSS. Toevallig komt de querySelector ondersteuning aan browsers precies overeen met de ondersteuning voor :target. Hierdoor kan ik simpelweg de volgende test doen:

	if(document.querySelectorAll){
		<!-- plaats code hier -->
	};	


Hieronder zie je de ondersteuning voor QuerySelector, en dus de ondersteuning voor het volledige component in browsers:

 ![caniuse.com](https://lh3.googleusercontent.com/vwhLesz7dZpx4ElxN8JiUQHlcu-a84unIIGrUy-3e-Y_ICiOOpAE3xqqalxrpwnkK5GrH9ioryslrqXn0L69-T1w2UzKXzbu9IuoI5e48uYUhOs2SsC5OH9bfy0HNFzSigIE2_0zk1KgIJAcwhsYXXMJ6CUm8nK5BfFiFFV64lp4FmClw4768Ihqn1F3E3HE4sx8MMM1vVmRfUncGWaI1pY9sBFQ3xn0FikZwRH6cNVc04rIxckKS-P5AVt22y6z15HV7Rv4lKdz0ImtXrLLeSGjbCzXEf8VePSEnlfObSJKxK7h1y3wFXRbrwfwD_wCeeM3ulTHHKvh6n_YWqmUB1aYY5Eiplr4xpBkTixvAqkPnl-YLXa8HI17gyEd33MQHQ1U409oUnYPwkBEbdHtZEQfUIV6P6GDNwwTPezWBmObY2D4RJUdYS0gWXAwYYwOqO2TBrqgzEJJHyeD1xCX_Wk2t55pVNj_RikN9Jgr1aXBkahI2iFpgSdP0zPK-c4kkWLaPN553ldix5LYCRTXmflQsnL3ojn__YQm926jvkhLVp-Q3p-k7VCftz3dMVQb3-JSkPVbAXoUlZQF9ifSSKdQvs266OUZNh3JVig=w2546-h954-no)

Hieronder zie je de ondersteuning voor :target in browsers. Deze komt precies overeen met querySelector:

![caniuse.com](https://lh3.googleusercontent.com/dXVdAfx-N2KxyK9V5gqIPrPA2ERlpTWGosDuRzi85RlvmJRzJ9YCjwZ9HevaYvrkhW4_wesob-R1Tpmq32s_84xbgUei5Uokcxi9LRpBmmkBwfuHZUMdSTNPzU_9edmwLwJ0YRkR8ZM83nqR6FigtmfoRkuhbRhN_wazPX6j9VAkvCvTaBRN9zTp87pjewgx4KQREt3LIdm3jz52LHq5DSmf6B8tsdKcwJptUlMM0gx31Nj62a7lLqMF5MQ85tsAltbGwmVU_4XNY-6f-AWHPIYp2Lg1VQVD1DhUKGrmZvpGlV7kTtWr2hsvIum6AfTYBb6ps6cAvAqhTYUGO1DmBYEKieom8_cMn7qzTAU6d4gpZzUSxaIZAA7CHlmXQFCg4XlpBKBlJg7RXmWJYYEaTK9zEbAbhixysn61KXps5DWmp1wYn2U_EJa1bXraGtXL__eEVGsnRRh4LCYYRq9BqLZusqNehhYodbAtockXi2EsCO_Tcxwceqxwy0sDq5LlGsb4gPCz8YBPMW7flEweUassmPhyZpuQB4fDfIiI6IzWG_lHgZKXYVm2dSGZIq78D4RvGJhuk28Wq_KPYdbr4-WawSYCECxc-ARlyeo=w2004-h978-no)

## Hoe ik er voor heb gezorgd dat de core functionaliteit het overal doet

#### HTML

Ik ben begonnen met de basis HTML layout. Hiervoor heb ik gekozen voor elementen die altijd ondersteund zullen worden zoals het <p> elememnt. Daar bovenop ben ik het carousel gaan bouwen. Hiervoor heb ik twee containers gemaakt die het hele carousel houden, en daarbinnen in het tekstvlak. 

#### CSS

Nadat de basis html stond ben ik doorgegaan met het toevoegen van css. Ik heb de verschillende stukken tekst naast elkaar laten floaten, en vervolgens doormiddel van :target kan je door de slides navigeren. Wanneer een browser geen :target ondersteund dan werkt de carousel niet, maar zie je de tekst wel gewoon onder elkaar weergegeven. hierdoor zal je altijd de tekst kunnen zien en werkt de core functionaliteit altijd. 

#### JS

Ik heb In Javascript een kort scriptje gemaakt die checkt of een browser querySelector ondersteund. Toevallig had ik gezien op caniuse dat de ondersteuning hiervan hetzelfde is als :target over alle browsers. Hierdoor heb ik de volgende test gemaakt:

	if(document.querySelectorAll){
    var carousel = document.querySelector('.text-holder');
    carousel.classList.add('enable-feature');
    };

Waneer de browser door de check komt dan wordt er een css class toegevoegd die de carousel in werking zet.


