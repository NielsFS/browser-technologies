# Menu component

## Wat doet dit component?

Navigatiemenu gemaakt dat op kleinere schermen/window veranderd in een uitklapbaar menu. Hierbij heb ik rekening gehouden met de core functionaliteit van mijn menu. Dat houdt in dat hij in enkel HTML naar behoren werkt. Vervolgens heb ik daar een laag css aan toegevoegd en met javascript heb ik bewerkstelligt dat hij ook daadwerkelijk uitklapt. Wanneer je Javascript uitzet dan werkt hij nog het zelfde, en hetzelfde geld voor wanneer je css uitzet.



## Eerste ruwe schets:

![schets](https://lh3.googleusercontent.com/5aycH_0YKV2COKlLcybscmo8wm_7h0xfWke5CefGvpt70XN3KJ1_BTznBZHrj-snONo9PcfCPsE-tb9XhHu5oPzJOXP0N4vdpfDCZyV4GnQaeliJ-uCYd0oWcyENvAUSkH7ZnuyZCFXRYJ-YrEAj-9JIMPcElC0MkPj8PL1Hf_tAa8cVzveToYXkLIARFCquGMmh51Be5zKcfC6_tNQc_e-QcQTZ0GnAVdFM1dRTbhhkaV2J6jyOK2mEbBVG-H4DfMwXUjxaeHXOlu-ZdtA21QwZqtZnVBcE7O3cPjp7uEw952zLMywPv-f2skhxeWzx8CWnKyaNV24ziJTiKF2hE-iJ_fPOLJ6thnEHLTspDFpd8YmcYRV-fQcKuLXp5VjiXdQSZysRl9NGQy0kOiWv_2aN3IDbqdfl1fSb3YU4Q8OCeGDthUEc9DXAg7HnyJREAj02gDZePzmjRSMtjoT0JKwCaakVhppL7Ilb-vYplkIF7OTdsBHvx83ZZ1kSfTkgxGijf1oYLm_mWCWHJF416wgidqme3Zrm5nONooEUvYqkEw3sn9kFK1Zt3W3qT5W0DNiXpbn1H9h96FZCmmdbQo2Ivdhnl11I6TvUL_M=w1224-h1632-no)


## Bronnen & artikelen

#### caniuse.com
[link](www.caniuse.com)
#### presentatie voorhoede over progressive enhancement (weekly nerd)
[link](https://moodle.cmd.hva.nl/mod/url/view.php?id=19943)
#### MDN (implement feature detection)
[link](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/Feature_detection)

## Welke Browsers/ devices ondersteunen dit

Alle browsers en devices ondersteunen mijn component omdat hij altijd terug valt op de basis html. Verder zit er niks "standaard" in de css die er voor zorgt dat het component onbruikbaar wordt. Ook wanneer Javascript uitgezet is. 

Er is een test toegevoegd die checkt of de browser QuerySelector/QuerySelectorAll ondersteund. Wanneer dit niet het geval is dan wordt de Javascript niet uitgevoerd en valt het component terug op de basis HTML en CSS. 

	if(document.querySelectorAll){
		<!-- plaats code hier -->
	};	


Op de volgende afbeelding is te zien door welke browsers het volledige component (met Javascript) ondersteunen:

 ![caniuse.com](https://lh3.googleusercontent.com/vwhLesz7dZpx4ElxN8JiUQHlcu-a84unIIGrUy-3e-Y_ICiOOpAE3xqqalxrpwnkK5GrH9ioryslrqXn0L69-T1w2UzKXzbu9IuoI5e48uYUhOs2SsC5OH9bfy0HNFzSigIE2_0zk1KgIJAcwhsYXXMJ6CUm8nK5BfFiFFV64lp4FmClw4768Ihqn1F3E3HE4sx8MMM1vVmRfUncGWaI1pY9sBFQ3xn0FikZwRH6cNVc04rIxckKS-P5AVt22y6z15HV7Rv4lKdz0ImtXrLLeSGjbCzXEf8VePSEnlfObSJKxK7h1y3wFXRbrwfwD_wCeeM3ulTHHKvh6n_YWqmUB1aYY5Eiplr4xpBkTixvAqkPnl-YLXa8HI17gyEd33MQHQ1U409oUnYPwkBEbdHtZEQfUIV6P6GDNwwTPezWBmObY2D4RJUdYS0gWXAwYYwOqO2TBrqgzEJJHyeD1xCX_Wk2t55pVNj_RikN9Jgr1aXBkahI2iFpgSdP0zPK-c4kkWLaPN553ldix5LYCRTXmflQsnL3ojn__YQm926jvkhLVp-Q3p-k7VCftz3dMVQb3-JSkPVbAXoUlZQF9ifSSKdQvs266OUZNh3JVig=w2546-h954-no)



## Hoe ik er voor heb gezorgd dat de core functionaliteit het overal doet

#### HTML

Ik ben begonnen met de basis HTML layout. Hierbij heb ik gekozen voor passende elementen. 
Ik heb er voor gezorgd dat wanneer zowel Javascript en CSS uitstaat, de content duidelijk in zicht is. Het navigatie menu staat onderaan. Doormiddel van een link kan je snel naar het menu worden gebracht.

#### CSS

Na de HTML ben ik alles gaan stylen. Hierbij ben ik begonnen met de basis styling om alles in een mooi venster te krijgen. Vervolgens heb ik in css er voor gezorgd dat het menu venster uit zicht in de browser is. Doormiddel van het toevoegen van de class .show komt het venster weer in zicht. 

Verder heb ik de css zo gemaakt dat wanneer Javascript uit valt, het menu wel nog volledig werkt

#### JS

Doormiddel van Javascript wordt het menu getoont en uit zicht gehaald wanneer je op de hamburger klikt. Ook zijn er een aantal dingen die Javascript standaard toevoegd zonder dat er iets ergens op de pagina een event gebeurt. Zo vervangt javascript standaard het woord menu voor een hamburger icoon. Wanneer Javascript uit staat krijg je gewoon het leesbare woord menu te zien. 

