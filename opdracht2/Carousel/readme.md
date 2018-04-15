# Menu component

[pagina](http://carousel.niels-schopman.nl)

## Wat doet dit component?

Dit carousel scrollt tussen 3 vensters. In die vensters heb ik tekst geplaatst, maar foto's en andere dingen kunnen er ook in geplaatst worden. Onderin de carousel staan 3 bolletjes waar op geklikt kan worden. De carousel verplaatst zich dan naar de corresponderende slide. Om de carousel feature volledig te kunnen gebruiken moet je wel een nieuwere browser hebben. 


## Eerste ruwe schets:

![schets](https://lh3.googleusercontent.com/ORxTWszU_1A4pOx74U0UcPAO1dSVwxJigCcJHhNx4ODt3cFgERGjczBXbK7m824PyBbiAJrCMefYXTBiUapkB5V4lsOhIelghP-YUb_whL70ltZlSt0xtCyHi8EZzWUzOcl5QHPwLz3ElCCyVOxhDA_LEelI6RwSygWulTsJk-FeMY1EyviYSP1cCnZBanD1Jp99Gt-ga0Y-2BivAl31V_9oEiabphdHySgxL25nb0dbjlgWYtYaQvuufD2VkXyJ1RcApYXF0FLMqpf_q53Vg3g-SgMVF0M7uKfiaGSH3LahaXUA9O5eDF-0wSlmdJlto3UKp-x-hqap8Z3hY0uLimuAPShnkG_yYscK5PNgfuNziKfhOWFT1fE6aZZiuY-ngnYhqs_tedVxbHFWIZO9Uu_2bPE9iLrJYrItUusahslZjZaLeTHYfwDuBJwS6NbEGQGyshXqF56Cc5KgzTkzOhBaT7s46KO5I-UCrPWY8vP7NwHXlUvgY878qBJF9s_olQmZvSIf_NCfJteIJZVz9QZjiT0C3kNIhwUN7gkkU6zETg72DbYryiaJG3rqQPxxrzaedcW3aV8Pex1-yYZGVzZJ0Ms8O8NS7M2VJOw=w1224-h1632-no)


## Bronnen & artikelen

#### caniuse.com
[link](http://www.caniuse.com)
#### presentatie voorhoede over progressive enhancement (weekly nerd)
[link](https://moodle.cmd.hva.nl/mod/url/view.php?id=19943)
#### MDN (implement feature detection)
[link](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/Feature_detection)
#### 
[link](https://css-tricks.com/on-target/)

## Welke Browsers/ devices ondersteunen dit

Alle browsers en devices ondersteunen mijn component omdat hij altijd terug valt op de basis html die gewoon leesbaar is. Wanneer een browser niet :target ondersteund dan wordt de carousel een gestylede lijst met alle stukken tekst daar in.

De navigatie bolletjes staan standaard op display none. Wanneer Javascript uitgevoerd kan worden dan worden de bolletjes pas zichtbaar. 

Er is een test toegevoegd die checkt of de browser QuerySelector/QuerySelectorAll ondersteund. Wanneer dit niet het geval is dan wordt de Javascript niet uitgevoerd en valt het component terug op de basis HTML en CSS. Toevallig komt de querySelector ondersteuning aan browsers precies overeen met de ondersteuning voor :target. Hierdoor kan ik simpelweg de volgende test doen:

	if(document.documentElement.classList && document.querySelectorAll){
		<!-- plaats code hier -->
	};	


Hieronder zie je de ondersteuning voor QuerySelector, en dus de ondersteuning voor het volledige component in browsers:

 ![caniuse.com](https://lh3.googleusercontent.com/vwhLesz7dZpx4ElxN8JiUQHlcu-a84unIIGrUy-3e-Y_ICiOOpAE3xqqalxrpwnkK5GrH9ioryslrqXn0L69-T1w2UzKXzbu9IuoI5e48uYUhOs2SsC5OH9bfy0HNFzSigIE2_0zk1KgIJAcwhsYXXMJ6CUm8nK5BfFiFFV64lp4FmClw4768Ihqn1F3E3HE4sx8MMM1vVmRfUncGWaI1pY9sBFQ3xn0FikZwRH6cNVc04rIxckKS-P5AVt22y6z15HV7Rv4lKdz0ImtXrLLeSGjbCzXEf8VePSEnlfObSJKxK7h1y3wFXRbrwfwD_wCeeM3ulTHHKvh6n_YWqmUB1aYY5Eiplr4xpBkTixvAqkPnl-YLXa8HI17gyEd33MQHQ1U409oUnYPwkBEbdHtZEQfUIV6P6GDNwwTPezWBmObY2D4RJUdYS0gWXAwYYwOqO2TBrqgzEJJHyeD1xCX_Wk2t55pVNj_RikN9Jgr1aXBkahI2iFpgSdP0zPK-c4kkWLaPN553ldix5LYCRTXmflQsnL3ojn__YQm926jvkhLVp-Q3p-k7VCftz3dMVQb3-JSkPVbAXoUlZQF9ifSSKdQvs266OUZNh3JVig=w2546-h954-no)

Hieronder zie je de ondersteuning voor :target in browsers. Deze komt precies overeen met querySelector:

![caniuse.com](https://lh3.googleusercontent.com/dXVdAfx-N2KxyK9V5gqIPrPA2ERlpTWGosDuRzi85RlvmJRzJ9YCjwZ9HevaYvrkhW4_wesob-R1Tpmq32s_84xbgUei5Uokcxi9LRpBmmkBwfuHZUMdSTNPzU_9edmwLwJ0YRkR8ZM83nqR6FigtmfoRkuhbRhN_wazPX6j9VAkvCvTaBRN9zTp87pjewgx4KQREt3LIdm3jz52LHq5DSmf6B8tsdKcwJptUlMM0gx31Nj62a7lLqMF5MQ85tsAltbGwmVU_4XNY-6f-AWHPIYp2Lg1VQVD1DhUKGrmZvpGlV7kTtWr2hsvIum6AfTYBb6ps6cAvAqhTYUGO1DmBYEKieom8_cMn7qzTAU6d4gpZzUSxaIZAA7CHlmXQFCg4XlpBKBlJg7RXmWJYYEaTK9zEbAbhixysn61KXps5DWmp1wYn2U_EJa1bXraGtXL__eEVGsnRRh4LCYYRq9BqLZusqNehhYodbAtockXi2EsCO_Tcxwceqxwy0sDq5LlGsb4gPCz8YBPMW7flEweUassmPhyZpuQB4fDfIiI6IzWG_lHgZKXYVm2dSGZIq78D4RvGJhuk28Wq_KPYdbr4-WawSYCECxc-ARlyeo=w2004-h978-no)

De volgende browsers ondersteunen de de carousel:
<b>QuerySelector: IE9/ Firefox 5/ Chrome 4 (getest tot 10)/ Safari 3.1/ IOS Safari 3.2/ Android 2.1</b> --- <b>ClassList vanaf eerste deelse ondersteuning: IE10/ Edge 12/ Firefox 3.6/ Chrome 8/ Safari 5.1/ IOS Safari 5.1</b>

Hieronder zie je dat in ie9 de feature uitstaat doordat classlist niet ondersteund wordt. In Ie10 wordt hij wel ondersteund

![IE9](https://lh3.googleusercontent.com/BrB97nQaMyKnVaOucIinnSW9-Fpc5c2tnkqoWrD2uNGAMHySPMnT4TY-lXKGJfy5YKMCKsiPBLYPpbg5E8uviFJJFR7-V__Sny1bVLKDo3kcFFfMrgHbWl688rUdjN03nIn2hKMIvfLaKSK5TYq0b7WBsM-q4hnpgeBtmnO8UVNSCY0creCx8aKa943wDNzuHAvg-QvH8auJf76crYpCIvw6kbkuqKBkNAHaOu8INooKerwTl3Kwh41SaR6I9CW06h_U1Mw5C-YWGEjK0BVO2lFBFCBJjdWD5hPp06yE83DaRVasD7tzMG4WeHSh2lc66Qt8KEa0XkcQP04USisqGbMwrOwaQtoAPT32e0CQTqveJc7UyaG4VnNNyRndTJIDe6MJghSveJxJ5n-DfmvQG6ZLSf6BBG1d4Uywyc058o6gY2cIUz2lQgnl5pLMSarWGejqgRSEX6P-MWx-IH2rfoF6UXEg--14-V8ekRuZ4Op3OKZZDsz6kaSP0cxRGDrxFCAyk5vdMEOUQquZK6-iTc0V5yI5XhyudYhj8bihollTXR6KZwvhwoCIcRScfKS-EjB2gjHGPR4UAL7ykrapzHVOhGFpn9B2PqNP_9c=w860-h1060-no)

![IE10](https://lh3.googleusercontent.com/7hj-rIEiqT34PH3j9YgKk18Lgz01auRP1KX8yvUGe_q6QdYbO9YQC84IKUpbWO1JbulgL7IK91uOIe3FhImDno3iQcMLpQa3hruaUeKk0_gyH2NwuVJaXgC0BXSnizLCh7CodoQYjIIZ5sz5lgEPRo17DcqkWddGAUQzU9xIMJ74JqveLSqmrj3VVM54-uatmNR60K87HYlGZIr3WqoQn05Zs6VP9wy97CpLZcm_u98zNZkGgMP3LeFkcYhsMy6I6yERDm7RzJlGAzWgEvDJqF21mzQ6c1nS9tIoHQFFcbTgbZOSzrPHldJ-0CW8PutYA8NwYnGmbM2JAEOftFN1X4-fBKzpjSj9rl2cpQkGx4GsK0qpeMD2gG6KtP6tMVy95i64CHRJD1hVnuKUmckB-CO2mPtpG_4f4ZTsQZox1EAuxED35x1yHA0nm4_j8QFGbKBATHq62S9eK4EZ8sEPCWxH2xHFzsXgDqtBh1BREQ52e1jeQTpXUaRPfL2wYobjKRdbuwsszBAKAu91zEMpuMz-atCTi_LRn4K0oZf2YkN1h38xMo2wHXx5QwK36u7mmc0YIcWCsIbH3Xpzj1fAgzT4wERG6L-jH3mi5D4=w832-h858-no)

## Hoe ik er voor heb gezorgd dat de core functionaliteit het overal doet

#### HTML

Ik ben begonnen met de basis HTML layout. Hiervoor heb ik gekozen voor elementen die altijd ondersteund zullen worden zoals het <p> elememnt. Daar bovenop ben ik het carousel gaan bouwen. Hiervoor heb ik twee containers gemaakt die het hele carousel houden, en daarbinnen in het tekstvlak. 

#### CSS

Nadat de basis html stond ben ik doorgegaan met het toevoegen van css. Ik heb de verschillende stukken tekst naast elkaar laten floaten, en vervolgens doormiddel van :target kan je door de slides navigeren. Wanneer een browser geen :target ondersteund dan werkt de carousel niet, maar zie je de tekst wel gewoon onder elkaar weergegeven. hierdoor zal je altijd de tekst kunnen zien en werkt de core functionaliteit altijd. 

#### JS

Ik heb In Javascript een kort scriptje gemaakt die checkt of een browser querySelector ondersteund. Toevallig had ik gezien op caniuse dat de ondersteuning hiervan hetzelfde is als :target over alle browsers. Hierdoor heb ik de volgende test gemaakt:

	if(document.documentElement.classList && document.querySelectorAll){
    var carousel = document.querySelector('.text-holder');
    var buttons = document.querySelector('.button-holder');
    carousel.classList.add('enable-feature');
    buttons.classList.add('show');
	};

Waneer de browser door de check komt dan wordt er een css class toegevoegd die de carousel in werking zet.


