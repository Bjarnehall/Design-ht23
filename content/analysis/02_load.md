---
Title: Load
Description: Performance report
Template: analysis
---
Rapport om prestanda och laddningstider
=======================

Denna rapport kommer att behandla laddningstider och hur en hemsidas uppbyggnad kan komma att påverka prestanda och upplevelse för användaren. Med hjälp av vertyg för att mäta prestanda och inspektion av innehåll på webbplatserna kommer jag att analysera utifrån dessa aspekter.



Urval
-----------------------

Mitt urval består av tre webbplatser vilka skiljer sig åt vad det gäller storlek, bransch och målgrupp, man kan även tänka sig deras utvecklingsbudget.
Habo kommun är en kommunal webbplats vilken i första hand vänder sig till dess invånare, en mindre kommun i norra Småland.
https://www.habokommun.se

Nordic climate group är en koncern som har en mängd kyltekniska företag anslutna till sig, detta är ett stort företag som verkar i hela norden. 
https://www.nordicclimategroup.se

Akai är en musikinstrumentstillverkare som främst fokuserar på trummaskiner och samplers. De vänder sig till kunder runt om hela världen, såväl professionella musiker med företagsmässiga studios som hobbymusiker. 
https://www.akaipro.com


Metod
-----------------------

För att utföra min rapport kommer jag att använda mig av ett verktyg som heter ’page speed insight’ för att mäta prestanda, 'google sheets' för att sammanställa data samt inspektions verktyg i Microsoft edge browser för att utvärdera detaljer kring webbplatserna. Jag kommer att mäta sidornas prestanda samt inspektera dess innehåll för att se vad det är som påverkar prestanda. Jag kommer att jämföra sidorna med varandra för att se om det finns några skillnader kring hur utvecklarna har arbetat med detta. Sedan kommer jag att göra en egen bedömning av hur väl de olika sidorna har lyckats med att leverera en bra sida i förhållande till prestanda.


Resultat
-----------------------

<div class="img-analys">
    <img src="%assets_url%/img/habofull.jpg" alt="Bild på habo kommuns hemsida">
</div>
<div class="img-analys">
    <img src="%assets_url%/img/habokommmunprest.jpg" alt="Bild från inspektera i edge">
</div>
Habo kommun är en typisk informationsbaserad hemsida vilken vill ge dess användare information om kommunen och erbjuda service för invånare samt nyfikna utomstående. Sidan är enkelt uppbyggd och bör således prestera bra. Genom att analysera sidans prestanda med hjälp av pagespeed insights kan vi se att sidan presterar något bättre i mobil vy än desktop om än skillnaden är liten. Pagespeed insight ger ett poäng på 57 i mobil vy och 55 i desktop. Genom att inspektera sidan med hjälp av webbläsaren tittar jag på dess innehåll, sidan består av 20 requests som totalt innebär att 4.8mb måste laddas för användaren. Filen ’vinter_webb.jpg’ är den bild vi möts av i above the fold på landningssidan. Denna bild ligger på 3.7mb i storlek vilket är 77% av all data vi hämtar från sidan. Utöver denna bild har vi inga stora requests.
<br>
<div class="img-analys">
    <img src="%assets_url%/img/ncgfull.jpg" alt="Bild på nordic climate groups hemsida">
</div>
<div class="img-analys">
    <img src="%assets_url%/img/ncgrequests.jpg" alt="Bild från isnpektera i edge">
</div>
Nordic climate groups webbplats är uppbyggd som en kontakt och bloggsida. De berättar vilka de är och ger oss ett slags nyhetsflöde som uppmanar besökaren att ta kontakt med dem. Webbplatsen har rörliga bilder som ger ett stort intryck även om sidan ser ut att vara enkelt uppbyggd. Genom att använda pagespeed insight får vi information om att detta är en sida som presterar bättre i desktop än mobil vy. I desktop vy får vi ett poäng på 85 medan i mobil vy 51. Genom att inspektera sidan kan vi se att sidan består av 96 requests som kräver en datamängd på 8.7mb totalt. Filen ’norrsken2.mp4’ är den rörliga bild som användaren möts av på landningssidan i above the fold. Denna rörliga bild ligger på 3.8mb i storlek och är det enskilda request som kräver mest och är 44% av den data som hämtas, utöver detta finns inga stora requests.

<div class="img-analys">
    <img src="%assets_url%/img/akaifull.jpg" alt="Bild på akais hemsida">
</div>
<div class="img-analys">
    <img src="%assets_url%/img/akaiperformancetime.jpg" alt="Bild från isnpektera i edge">
</div>
Akais webbplats är uppbyggd som en presentationssida över deras produkter där användaren möts av ett galleri med rörliga bilder och stillbilder. Hemsidan ger ett stort intryck där image och teknik är i fokus. Genom att analysera sidan i pagespeed insight så kan vi se att denna sida presterar bättre i desktop än i mobil vy. I desktop får vi ett prestanda värde på 66 i kontrast till 32 poäng i mobil vy.
Genom att inspektera akais hemsida kan vi se att den består av totalt 270 request som ger oss en datamängd på 44.8mb. Det finns 8 st filer som alla ligger över 1 mb i storlek, utav dessa requests finns en png fil på 2.2mb och sju stycken xhr anrop som ligger på en storlek som sträcker sig från 3.4mb upp till 5.2mb. totalt står dessa för 32.3mb vilket motsvarar 72% av datamängden för sidan. Utöver detta så finns ytterligare xhr anrop samt png filer i mindre storlek.

<br>
Data från resultat
----------------

<iframe width="760" height="250" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTM1v0wERBssvx50vs856-sZ9r5X6Hbpc4CvFMVgQ0RGWP06vl7wfr9Ukpic6gm5v7xX_9gvTas1Fo7/pubhtml?widget=true&amp;headers=false" title="Inkluderat Google Spreadsheet som visar data från undersökningen"></iframe>



Analys
-----------------------

Genom resultaten från PageSpeed Insight samt inspektion av hemsidorna med hjälp av verktyg i webbläsaren kan fler slutsatser dras. Den största datamängden som i sin tur påverkar prestanda och laddningstid har att göra med de bilder som presenteras på webbplatserna. Habo kommun och Nordic climate groups webbplatser är uppbyggda på ett liknande sätt och har således liknande bekymmer. En stor del av den datamängd som krävs för att ladda dessa sidor beror på att enskilda filer tar mycket plats då Habo sticker ut med en enskild bild som motsvarar 77% av datan som hämtas när webbplatsen besöks. Trots detta är Habos webbplats relativt snabbt då den inte har särskilt mycket innehåll. Den bild som laddas above the fold på Habos webbplats skulle kunnats optimeras för bättre laddningstid genom att komprimera bilden. Nordic climate group har en bild above the fold som även denna tar upp mycket utav datamängden men då det är en rörlig bild så sticker inte filstorleken ut, utan är redan komprimerad en hel del. Även om Habos webbplats laddar snabbare och presterar bättre ser jag mer förbättringspotential i deras webbplats än Nordic climate groups. Akais webbplats är uppbyggd på ett annat sätt och blir därför svår att jämföra med tidigare två webbplatser. Det är en krävande webbplats med mycket rörligt matrial som kräver mycket data. De har dock optimerat detta väl då de använder sig av xhr anrop i stor utsträckning. På webbplatsen 'mdn web docs_' beskrivs "(XHR) objects are used to interact with servers. You can retrieve data from a URL without having to do a full page refresh. This enables a Web page to update just part of a page without disrupting what the user is doing."(hämtat, 2023-12-03). Genom att arbeta på detta sätt så kan de leverera en webbplats med tungt bildmatrial på ett effektivt sätt och måste därmed ur ett användar perspektiv anses som den bästa av dessa webbplatser.

 För att lyfta en annan aspekt av prestanda och varför det är viktigt så vill jag lite kort behandla ämnet hållbarhet. All data som används vare sig det är i användarens egen maskin, webbplatsens datacenter eller överföringen där emellan har en viss miljöpåverkan igenom strömförbrukning. "*Optimizing our sites can reduce the amount of data stored and transferred, and the amount of power consumed by the user’s device. Building sustainably can also help extend the longevity of users’ devices, reducing the need for upgrades and replacements*" (Barker, 2023). Med dessa insikter så skulle vi kunna säga att Habo kommuns webbplats är den bästa men detta känns inte rättvist då den skulle kunnat optimeras relativt enkelt vilket man inte har gjort. För att dra ett gränsvärde för vad som är en bra prestanda ur ett användarperspektiv väljer jag en laddnings tid på två sekunder. Utav dessa tre webbplatser är det två webbplatser som jag godkänner och det är Habo kommuns webbplats som genom minimalistiskt innehåll klarar av detta och Akais webbplats som genom en god teknisk lösning klarar sig. Nordic climate groups hemsida underkänner jag då jag anser att en laddningstid på tre sekunder är för mycket och om man känner sig tvungen att använda sig av rörliga bilder på sin hemsida skulle man kunna hitta en lösning som liknar Akais mer. Men ur ett hållbarhetsperspektiv underkänner jag Akai då deras webbplats använder en orimlig mängd data för en sida som egentligen endast ska visa upp produkter.
<div class="img-analys">
    <img src="%assets_url%/img/energy.jpg?w=200" alt="Bild från refererad artikel">
    Bild från Introduction to web sustainability, Barker, M. (2023)
</div>

Diskussion
----------

Genom att optimera webbplatser och dess innehåll kan vi förbättra världen ur ett hållbarhetsperspektiv och då är det inte bara hur vi kan göra den bästa tekniska lösningen som behöver vara i fokus utan vi borde som utvecklare även ta ett steg tillbaka och fundera över vad som är nödvändigt att presentera på våra webbplatser. Måste webbplatsen innehålla storslagna bilder och rörligt matrial? Kan vi åstadkomma en attraktiv webbplats med mindre matrial? I alla lägen kan vi inte detta utan visuellt matrial har ett stort designvärde och bilder är ett väldigt effektivt sätt att enkelt åstadkomma en storslagenhet? Om vi hela tiden försöker utmana oss sjävla kan vi då kanske åstadkomma lika storslagna designer med mindre bildmatrial? Jag tror att om vi följer detta tankesätt kommer vi att tänka efter en gång extra innan vi använder bilder i våra webbplatser och om de verkligen tillför något. Om så är fallet, hur kan vi presentera dem på det mest effektiva sättet?

Referenser

-----------------------

Barker, M. (2023) *Introduction to web sustainability.* mdn_.
https://developer.mozilla.org/en-US/blog/introduction-to-web-sustainability/


Övrigt
-----------------------
//Jonas Bjarnehall