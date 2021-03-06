# Contactenlijst
[Klik hier om naar de pagina te gaan](http://minor.niels-schopman.nl)

## Core functionaliteit
De basis van mijn component is het weergeven van cotactinformatie uit een lijst van contacten. Je kan door de contactenlijst gaan, op een contact klikken en zo de contactinformatie weergeven. De basis is op een semantische en logische wijze gemaakt. Wanneer je op een link klikt dan kom je in de core op een nieuwe pagina de juiste contactinformatie. Wanneer css aan staat is de lijst mooi gestijld doormiddel van progressive enhancement en fallbacks. Wanneer Javascript aanstaat dan worden de details op de hoofdpagina weergegeven zonder een nieuwe link te openen.

## Features/technologie

#### html

- Duidelijke semantische structuur. <b>Alle browsers</b>
- Basis navigatie toegevoegd die tot en met ie6 ondersteund wordt (styling) en alle versies van chrome, firefox etc. <b>since IE6+, Firefox 2+, Chrome 1+ etc</b>
- HTML van features wordt pas gecreëerd nadat het getest wordt op ondersteuning, en wordt vervolgens toegevoegd. <b>IE9/ Firefox 3.5/ Chrome 4/ Safari 3.1/ IOS Safari 3.2/ Android 2.1</b>

#### CSS

- gebruik gemaakt van sticky <b>Chrome 56 [bron](https://www.chromestatus.com/feature/6190250464378880)/ Firefox 32/ Safari 6.1 (webkit prefix)/ Edge 16</b>
- Gebruik gemaakt van transities (zonder prefixes) <b>IE10/ Edge 12/ Firefox 16/ Chrome 26/ Safari 6.1/ IOS safari 7.1/</b>
- gebruik gemaakt Veranderende achtergrondkleur (keyframes & animatie zonder prefixes) <b>IE10/ Edge 12/ Firefox 16/ Chrome 43/ Safari 9/ IOS safari 9.2/</b>
- responsive (flexbox zonder prefixes)<b> IE 10 deels/ Edge 12/ Firefox 28/ Chrome 29/ Safari 9/ IOS safari 9.2/</b>
- Verwijderen van border van alle laatste li elementen (last-child) <b> IE 9/ Edge 12/ Firefox 3.5/ Chrome 4/ Safari 3.2/ IOS safari 3.2/</b>
- navigatie aan de zijkant van scherm zetten met onmouseover events <b> IE 9/ Edge 12/ Firefox 5/ Chrome 4/ Safari 3.2/ IOS safari 3.2/</b>

#### JavaScript

Alle Javascript wordt ondersteund op de volgende browsers:
<b>QuerySelector: IE9/ Firefox 5/ Chrome 4 (getest tot 10)/ Safari 3.1/ IOS Safari 3.2/ Android 2.1</b> --- <b>ClassList vanaf eerste deelse ondersteuning: IE10/ Edge 12/ Firefox 3.6/ Chrome 8/ Safari 5.1/ IOS Safari 5.1</b>

- testen op ondersteuning
- Filter op eerste getypte letter voor overzicht
- Filter op contacten uit lijst 
- HTML creëren 
- contactdetails op zelfde pagina als contactenlijst (single page)

### browswerondersteuning
- Voor de ondersteuning per feature, zie dikgedrukt onder Features/technologie.
- Zonder bronvermelding is er caniuse.com gebruikt


#### IE

IE7

![IE7](https://lh3.googleusercontent.com/rGIlBbXZU83D-1Ra66RD4-Q2dBat0MA9V_k5iGOcHARWe6v_HWQs3xsy2bssWDZHYTuNgaHtciG5TpTaJBJxv-3uw5dvc70tnnDBrv5X73t7ab5xEPirprc5rsspltl5axGU0-1CcckJDhpNec8KEcVHbTXe41UBhSoSaGCWsp2TIbfK3Em7tUxRPvU-bnL68q7hnhB0bga2PtLbDj7zQxejqI2XPpSlagVrg7e5qhEU4MaO_irUkVBdxnTS-1_eDNxk8Fu9yOltxL7DuOpwSqgkmCbzR6L5uxvonH93P6RHuI-POFOQcXolBYqN2wHQFCAq-yEZZjc9HmliGxkT14sYjcF5gPf3-ashFXNNBHE05t9Lb8y1F2zf3ADHBRLtmKvDUFm9n9O-BdG3GEBQjih9QfGNJB-Z09eC41AejX8J0tGrr1DJG7cebFzs4iOhr0hqYMJs9TklAUSmlHFq1Dwu3_rXtp5NWHhQni2yeN2agJwCyHf4MubtKQwW_hN5EGTlqfXbG4TmZEOiEYH0zROYgb7Nq9SwwakKTPnGxHefy8z27YQFU7EmBPGd4rlPAlcnr3EcQaBD1FQtZv_8lQGxtyNlx3i66q_Ldf8=w563-h323-no)

IE8

![IE8](https://lh3.googleusercontent.com/l49DzC3-PAwsr4FQP94om7SiubFRysDIQLY0px2ysZqdT8tYoDXTHHPUyMYCe6Az3dpYehfssO5ilTNvI3dcyvYVxUP4sT5IohN2O9ITa5je9Ycjpze95pgbyjJRTYZEVfZh__XaqOBj4I4sLS1QXzzIp6qZ5dvbKLQf-aO28M4OvZOvVerCX-9I554NnWSI1H0Q81KqEnntudSIQRP5Ojb_EWogX_L_-oaCdSsNI8fSIDz5QyaqSJKWcpfaqJipIj7rrYsXtfPjkiNV6Ea_xdLvb4ysB_chSNaU4W0iRtKCY0QtEyxcmCY9cAHV7MkCQZOeB706DWZlxvvJf-3UBdkmxd8s50R3hfTW4UbVN0WuxOy156upL-cb1HpjgYqwNBeehHI9c0omogVbuddicAVaQliTTViQ8JdPgHR-ryGp_kr-WyKmN9_KLwwjsI9_V2L64MkWBtHlrZV3vNZEHQoJwh0C6dfjpvMBMWV9F-aQnt7g5i74vC4WYFGv2w3R-NiQEZUxqascR9OAw5v71wsWkzhsAe5H6BdjYGo-fzDO7driAflZzJPvWI8ZNTEFpQ9TBLdzoWcmZDd7eAUWCQxMk3B6LXIwBAU3sfk=w447-h276-no)

![IE8](https://lh3.googleusercontent.com/_FAWrCWAxlXpzhoasJIOXh4heU7YCgEsQi-DTI--WKhjDh2NvLaKMJNMsg8b2o3st2ErNJ6J6llKGWdGsGGnC_rPN6NTg8BbHqwLdYlRqcPxC6ltHoLF_HB-bdQz1CL9RvkRGKfjPms_j1LTOLtlvuJzO-MuROrBlRSg0kPxfTbw76_yWT5ahzJFsPCREE7bftaDVPyLgM9ajwpQDWqRs5DYnBLJY_UPuckOdM8Ck0cEm0Oz67uQ_jRnJu84BZynynn64wQdNpT5w8ypdV6M5kA4FbR8w044VLo1_WMNmGFb85XZAMMs2VTbN3WLucZeD4Az6pcRY5msXvNe9WT8WYBPtIimcWRqa5kKVVe1IfyAHq1UAzDm7paLQSYsGWNoNttDw21vRtaC21pPcTeZX6Y72FTV5Mv-aQ2pyfS9F9me0cSyXp-gBVIh1ds2sJQWw0tf1UYihQmlr_VbcG8JoNs7_rRCJGUvmtOWMLX4UPYALns0NkmluA-GKfPu7BT_sh1qHxjeWIIqHzWUrLPaZVErUEYBtCYxTVIXAbNKVzDC7XY6w0rs874FkBpC85-BvnwOcvIdGL7qtEZbEtGrcG1psVed1a9C5FW5zCo=w2002-h1390-no)

IE9

![IE9](https://lh3.googleusercontent.com/Dn5Weop83ey0dKHuHH_O6jbIjYc-CIO0AgzbWf-mIjWJv_4u8Jau_DxPUmfg_7rTcQbGZqZ0qqgVgxNjE6hR1LOGjvkppZsapV2d7qpIHxrQdwIIW-eaHpifE0FWyOhJAPJb9WRxPYSuh1MwUUIUb7CrL4Iy_UEFxoBNSb57BYN13qehjN_hTlRRXlm6eWDX24eejZhlw-0JH1g5zEJjXw3RvZyea-BMF47Mx7apbxWtn2H6A0v8z1CFgOAZRWK5Yyw41m2ypUHeWgRxCS1wypmF6wRqHTjzadSme8Ml4SENrCsuV4Yw9IQ3EAbawXpoCUZtUsO12iThtCXfYajqPgprfFlM86rPrmtXKELa_olQJ-2hkoPk7XWHk1JQTQSP0xyk1ggRAPmHr1SK23l5Z_wdlZj-k6kgnMHq8UC0LExXwuF5kMSPM1dmvBXN6l7lzvofADhVO7d-mFy2oRuF9jfGKSZGJ6IwMflAMhVy-kiQq8HNxR2PH9Mdg1MUInpWu0s16pizyhwzsa2JLe7sxsFKcVUdHkprpTMxy0Lo8XhYoVzX68pcRPWNswS8luIjqJEAwcShxjIEIWGhFHVuAGmJIioJixW2TNYMZW0=w2002-h1044-no)

IE10

![IE10](https://lh3.googleusercontent.com/-TzG4YGZbob0iXOka3XIfTiY7PLNR8TqjETeWSMdMp0K4zyTkDLHMCR7-CRXnJu0zJGMF-GUjICkLIgXRfCzZL4_5I7hPyjipWbOzHG7WjGVTPPH8ris0hAecjwJTNx0h3fZmvFVr_8Zf7RNyMaorAHYT_FlrbV-7fCp7rQ3HTv-3NnRYBuLPRX2IWmeTfP4i5Q8kqrVxTcbUE8l9f7Ltc4EBpUwJPv32KLfp14K8ZwtcHbW2sSEZarKFfzPlHTPsaVwsoymmaL54HfgXlXEmG5vm3pRKhoWb3wwVvaj3LjXNAaIjsO3o7GutxpOjtSmLscst6rk8oPZfZNmYc6C18cWAtqn0YHJDtm-jGOSEWRYK-bB02NOoL21PAoO6Yj2HTKv0-814vlQc_8aySNpLywun4d6eSwNQHrxJq78IupjdxWVFKHsjbh79tr4s9_2MAGiDNFBciKj5ikkJKNWA6jYVdU2eu4fyZPNq7J57O0VhAFfo5TftxSq2B_b6zNxF81pZDgOo_H3WC1V6DjLOC7vrTCJfM1H5ICUw7vb74SZ3o_pLWOd9AKgCaWndRCobh3gYV-PD8k3k-11eJhHHGlmbUD82uNhEnY7-PU=w2004-h1160-no)

IE11

![IE11](https://lh3.googleusercontent.com/vUiDzRsDAvhwK6-iBj06ZY75_qmgjv2JUG9SUQrMABNIDIK1UYNuAIMBHVbQv7UH9yWpjlprrgD4CcW5m7eZURUbL7IDQs_meVWkBeMvEHSYZhc3W8R7VLgpDCveaLJOfhCG0n3dON4hiyQ9bbxcf9bkocT915N8LkuwYBZR1iVgeSdrWejrociefyOVDCKqU7mwMR9tb3Ixra9WdCV4a8Shzm6io0scEAjba7WQBzm5F8chrW1tPxH11p8mDhYIIxoC_WPp1NWFTu0YE58o-7j19uhYp5IRfP_Oyr5m-Tw6PEzEUUvHINp4fpWbSAww5k9MKX-Oe1_4LxwepyZkIpBbLjI89l1jW-5WNSjV6fZHKQEOOwBGVpAfIKaW8GjR97oPLRdPExfQSB0J1ceqUl17JFVEMraPI97gaS7agXkMgqgIjANwOLXgRDXnOKgl-qc9ID9Vz4Mq3TTMWsZZKMxlrZ-PcqVyEhh3Df2mb0YhK2BNrvgavn-S9Sa714K7eIcF8d__fWS-pk-rh_Hvgu-wg9BtGy8-wsyvCrqF8If-A7a5uB99B8aiACh99Dw6g_XoGvTsdDHHxghRMxZIuRvi0ITmqdASot0F7Fc=w2042-h1142-no)

#### Chrome 

![Chrome 10](https://lh3.googleusercontent.com/7p7U-JTlBeUbj5cQa93-4jZdONy8k0PfrCsREdRdIMqZeeS7rG2VjK64o9IYn_dFjIy7qSrW4wMAORRLu6t2Ug-SI8h81UsLtJ9iT5VsO8IxlV-D8BpIZm3jFIhfiFzMi9G7S83O-C01Xr-zEl3UEZhUq3uhCy9N-RzWGhNWXaGVek6onx4V6cv4-jcQBn9jQFdiFmsEMUUgYSY3FFwJcWEnCb6V2cDVm793buG9u4_Rz1FMwFukKKDzMj-jHNeUb6MjgEXrnFrN9di7Xq-d78V28ab4pLgFAnPK-CIUi7q86LWDLS0e24rh-5wKxNmo3kdFpTuFBtiCr0I0Ls6hCroacxUxgNfKoxnwETSQnA25_j88iqfVGu0IVrOqhAh_-e-bhIR7E1F_ziHJV5u62mnHyhcO63E8EkJ3Gws81AJWbGdkNUB6dz7OCNHv8xPHhr-ijDzxO10TOZCTk8Ji40e7Or3p84hI9Tz8WoSmXQVLsaKanVzBY_rBx0HRuCQIlpxAbx8mZ7024G-vMyFW973BY5Ky_VCYbTY4J78N0uoJiePjwaZEWDxIn8bKAqT5h88f2i-QwbPjvDi1aVHejXOOr5tgADNFHj6WUEA=w512-h689-no)

#### Firefox 6

![Firefox 6](https://lh3.googleusercontent.com/pWqy_MUlYHQtrv1Cq0Rutq4dBQd4-QJOR7OBKYMjZ4vU5PfLYtoautYmbg6KvXxIqA3i2qb7GTM_gKNBpOMHSqRddV6jDD6O1dhu5wvNtMhihpvK2uLROgzzVWrt8kKF6ylRgJtN7bOLo7xGzSLWpdwsJzIRYPW6JfFn4qw25c6FRShKqMCuoRwwO6V3lNLiFrjxEgz9eSWu2NirZqMTrqpRnGGEvQ3bUk7yaMRPWUtXOBGIRiZi-VCtVfLNXZHayvEmc3U6Yq8qdQaCjmSjKERA7_GXQeAy1XEXx-LpgDpj77IEadcuYu6ZQBnlP3uSIZ-sDc5EXaZKSYKe8JIYHvz7LQYh9f0EXc4c1_DVHkPjts7DRc_Zhc9czJnbdDxbracgVvHeY3ULFhfFwoAnEA1ii2cyjrvWIBFE0PVKImqmRpio0_0Bvll2ewyWkTLh5ZJLpIXujpjf6L89ieUXRupNst-fSmmFx1-3u-ANDLOVkIWHJuTR__iAxGvxccoIro6sLWuck5KdaDKgikvGwnXSbvm2r0AMfu1VvPSWTFRu4Rgw6PPyAHiZ7YTrKTRMnDtbvXwaXyA6Y_wdQL4yS9py8HWpNDPUCM_HKgg=w512-h1039-no)

## Accessibility issues

#### Ontdekte foute op oude browsers:

- search balk staat zonder flexbox niet echt netjes uitgelijnd 
- verder geen noemenswaardige fouten. Volgensmij is ie que fallbacks en progressive enhancement goed.

#### Wat ik heb onderzocht en toegepast

- Juiste HTML semantiek (HTML validator)
- Tests voor Javascript features
- Kleurcontrast en leesbaarheid
- Responsiveness op mobiel
- volledig tapbaar met o.a. veranderende focus state doormiddel van Javascript
- Duidelijke headers, links, navigatie (terug naar contacten)

![HTML Validator](https://lh3.googleusercontent.com/vy2YQq67XFnlmYuY8HCu7DSNhzfSjtbVbxhsXbt-W5hYBCgkcepko7R-rxjXZaAkLz2zVHAi3NL6Y8CfobZmYojlrle_zLFKMvlhktb8857Xzt2E5ihIlRd95TC0qR4PwR7X3Cy4B5m4gFgNpL0gojEg0Rh3nUGp5XFfnHii1kiYWk3xFw8uB8VS58XMp49t-Icq0CePkL_6eFopbCk9aIAKBQXyTiKH6fi29i8bb5QWjM67PcuGgrL8vP_PU7ygihPqszm6FdSA0HSEeHk7nAQQWev5IKP06wW1ld_Tbqib1PwyLxoUK5DQ2aTlnygeFNFnJ3dZFfXqn82shvODQUxSB9y1wVur2UHTI2RtUyxPMnajtpjAPZhXc9JF2nd6ttWWDbHrQKMBacdDvTi4HmN8dwWBkPnUkuyHpliPJ6XIeUfvREj-pTSqiS7D1bxproL2w8ZUwgZ-BILW37EsEo0Ag2ik7oCev28xNJ_QnNeZd6cd6cZ3EL0Nd3Mpb1-zPJH8QxDlYqf7D3yehhkKxT6pu9COQ1785W8id05oilx_KtqV1f4zjhgCCvbRKBeIZOQ98-g9Y1sHqcmOzFAJMrLNBvnz67JCq0QGwmI=w2304-h424-no)

![Kleurenblindheid](https://lh3.googleusercontent.com/-TQudxsftw6euYqWlDKYKgEjHJD9Ci0RvAAjVXj39mh09m6st19ENecrPC3QbVyj3RBynmkwFqoHLgdp3XKk0WgYfE6BVbQ8Zq3X3ofP8FbM6ICU71mo4l9Yi7E8LjxPfT3rcsf3wJGK80W2RpWzXK3mwsUcLjHgdD3hSpI1nIkierYQYspLMmWImy_LPDw2vnL6ooyfSGdQvFv-RTIIc2YZa5MTfQVX1YaLWsFv757vU2NZtaVqCRIBX2nw1UWzTBYKF8wpQo_bLV0kkN1URpWRfga8vTOoGffxbHgK65-nKlBXOXDZy9rgBpKAcIky8cyNu_WC4IfaknddIdBmkgEmbg1rIGuKzMXaNVLkzr4i8juUgCJ6fuuEdwt6dtdWvBkPg4Ap3C0qXnjj8UiWvF76Cx_Hfxk8afAkuTP5MxHukHfK_bkKqn5Td_3KaUtV7GHKSWES84f4ZxjEmIg62uwlgrsYs3Pm6BMpgYkgDu69oLUfN_YDHO1unVKTfZGL2bU0AVpA71L9KzBldjnoqJqsL3mxY9OB2dDUHl_JrynA7HPFFHqqAFgNhiM1j1RaHz1QHNKEzcX71cOhc_ipDMHESLDWO_Ade7upGNc=w620-h353-no)

![Kleurenblindheid](https://lh3.googleusercontent.com/l6Wi6siH_MTrUXaCPmQKtrVcNHkgm32pMVDZdSU2etLtrF1feXkGKSnd4brWORB-6-A7w4FU-xVTC4FdeG2p9kNEkzFWfcBap3epevX2Fq3YRK8k6yA_CC3MLi2BM5Q2LRkFsyDRWFxujLkDAkLH8lfLJiFI13qUffveuYU7O3VLYBkyoaB-3WRcB4MDkeQQoeTDoPmIMSzrS5F3hDLi3UcHA_ubCzC3_ylLGbDWhyAxhG8mFvqQnaLAtH3mKqr2ko51IA4_Gv5YuT2xY3rv8_s1EmnnciqHdB5P7uHIPRx7lr0C8-O2T5ZYWxDd5onVAfXLzNhzMhKEKGSZOd0kRNeDA6NMn3X2Ihv83wYf0ij6agQKRoobHmu9nbyrWI4fqpFpTtmcgz6eHDL9S3OFvoP-BnckjUAueGb-NhJKXgfEUgDXaOePe2HaM7OBS2slnw56i-aqHqbTGy_I7cC8rPx69X2asHF0-keYIr7LqomSw9O-Vy9C5vk--bTMk1XAWBmwoDLSUMOhxXXqFoFnAWxFI0Mbt9r_vJxaE-nScJoEVf3yaruwi-NeRKPiO25VNphu1zJWMlQVB7E0KGuAIM44aTKGcs88EB70088=w2364-h1348-no)

![mobiel lijst](https://lh3.googleusercontent.com/le3QO72EDy0H3g5IjyJCyO5W6nHrAN4rqO0kL5F01cYgXs1xopEXav0N0pK_BSPnnU7Se3VT6e3uE5fWwGIL7cAXpUDWCrW32bBoeYMJocAvpYbIN_8YF7hPVu8lg9luLNIFb5mJDGIUoleCkI4DadkX1Fa2Z955PvlwDyZKzogUGvRbTgfl75AYIhx-rstHLiXCKroU_8-LptMB72dTTQ1rofLTJ9vf7Thib8Bkq81l2or2UmrWvpdyDv_F8RHx4SI9I0E5QqPAhEDXh5qDjynZt0wiiYrUvfI9qToDvZAnFqm8uH7WO67pVKBuNEd5_5IkN6R8FD1BkmOBtPszCGd_RU6rPOrZUm2OfOegvBq1nerI4zJS105xSTDi2KRBKYO69n0Tpu4W-i3ha985x8Y1gNXRtVyDwrOIVwtfda7zTz6GNj5CXEOXxgnBTXB7Ljs_H5AU1MUqsSFqhr15C-n_ioXRqv7ZGmQf6v_9Gn9tOCO1HHzvbb1njZ3KLAPSsAqRlUu8QL26wofpgs5yxCr15nj9h_qSoeDoi6hNQr5hf2rZX6a7Y-TFOAnorGAfepp0wbmVkcVzRU9EjDEC-YUQAy74bDEaVF6n4yo=w642-h1390-no)

![mobiel detail](https://lh3.googleusercontent.com/q5SjEqwAy0CzulEUD7m0FFyVh8aFVxjDGFYpeQEhOmejB1p4efXIYY933kQtIXO8ul3x6ihLVsQbdlwmitju8ATo_t_RTiEHJUDt_ClZ2iLZrmAg6EcKFCyUgYCfgZYrQ7-2chKsAAMnfGUZ0PC8YLxGxwu7jje72t7fyU5rHJG7EXH1C1bm1EXdd9USKKEtvEx9Lu8XkLKODRoWncRUG_UFAxZ9wrOcqXfLv-j7IvtOJ_nnxJRJv-Ehqlp4fJOePIbzHxIAHvoRDakZRVdYynGnHzbXww8pGZzGGQzwoVFHB813h5cKIFhSkUuQgM_ggQ8OSBezHPeNZc_0ej_JgyK1aMwHEY0LNhz_fBXvascLRVZXyXZ8UjZJefWj2xcST1G7tQ2Lm4ltiK6OhiDVlG5D6Qd9u7h3lEAsHnL0gpEt25rBTXXBlx6pZqmJhHUDP8pOOrWr0Jp8Xhu9-AtNpCwOlAmXx77JqevU3SCgkqb5cW3tl5DAbY5JNrMgiXA1r2hA9PUXYPd4WCYA7g3g5vLrVKs5ixQl1y7S-f7YefBb3PJVBeUYhly3oFxyqc9Tcj0z_B8I5Ioj3_v7HvrzHLRv54No7NM_lQ_5dT8=w642-h1390-no) 

## Wat ik heb geleerd & waar ik van opkeek

- HTML5 wordt niet in IE8 ondersteund. Contacten waren eerst doormiddel van de section tag opgemaakt. Echter herkent ie8 die tag niet waardoor alle links van de navigatie niet meer werkten --> moeten we dan geen html5 gebruiken voor dit soort dingen? of in ieder geval sections voor div tags vervangen?
- CSS selectoren worden niet altijd goed in IE8 ondersteund. Zo kan je niet .side-nav div { ***** } doen. Je moet specifiek met classes werken of alleen met tags. Combinaties zijn niety mogelijk.
- Er wordt gezecht dat je per feature moet kijken wanneer deze ondersteund werd. Wat ik heb gedaan is alle features die Javascript vereisen onder dezelfde test geschaard. Hierdoor blijft alle basis functionaliteit behouden, enm krijg je vanaf bepaalde ondersteuning toegang tot alle "upgraded" features. Alle css die buiten javascript wordt toegevoegd is degradable en is niet bepalend voor core functionaliteit. 


















