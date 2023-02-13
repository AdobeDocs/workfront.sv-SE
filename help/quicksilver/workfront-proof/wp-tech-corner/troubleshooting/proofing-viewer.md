---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Felsökning - [!DNL Workfront Proof] korrekturläsare
description: Om ditt korrekturinnehåll inte läses in och du bara kan se ett tomt korrekturläsare, är det troligtvis därför att något blockerar den här åtgärden lokalt. Prova de möjliga lösningarna nedan.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1274'
ht-degree: 0%

---

# Felsökning - [!DNL Workfront Proof] korrekturläsare

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om ditt korrekturinnehåll inte läses in och du bara kan se ett tomt korrekturläsare, är det troligtvis därför att något blockerar den här åtgärden lokalt. Prova de möjliga lösningarna nedan.

## Kontrollera webbläsaren och [!DNL Flash Player] Versionerna är uppdaterade

Alla utvecklare arbetar hela tiden med sina program och de släpper regelbundet nya funktioner och korrigeringar för sina produkter. Detta är för att förbättra användarupplevelsen och upprätthålla säkerhetsnivån så att det är den bästa metoden att endast använda de senaste versionerna. Detta hjälper också till att undvika konflikter mellan programmen.

### [!DNL Flash Player] Plugin-version

För att kontrollera din nuvarande [!DNL Flash Player] finns på [[!DNL Adobe] webbplats](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

Om versionsnumret skiljer sig från det som står för din plattform går du till [[!DNL Flash Player] nedladdningssida](http://get.adobe.com/flashplayer/otherversions/) och få den senaste versionen.

Observera: rekommenderar vi att du använder originalet [!DNL Adobe] plugin-program, så om webbläsaren använder en inbyggd lösning kan du inaktivera det och installera [!DNL Adobe] lösning.

### Webbläsarversion

Idag uppdateras de flesta webbläsarna automatiskt, men om du har problem bör du kontrollera vilken version du använder och uppdatera vid behov.

I webbläsaren går du till [!UICONTROL Menu] och hitta [!UICONTROL About] (i vissa fall kan detta vara synligt under [!UICONTROL Help] meny). I [!UICONTROL About] I den här popup-rutan hittar du information om den aktuella webbläsarversionen och även ett alternativ för att uppdatera/söka efter uppdateringar.

Se i Chrome:

![ProofView_3.png](assets/proofview-3-350x206.png)

När du har fått det senaste [!DNL Flash Player] installerade plugin-program och webbläsarversioner försöker öppna korrekturet igen och se om problemet är löst.

## Kontrollera din lokala [!DNL Flash] Det finns tillgängligt lagringsutrymme

Våra [!DNL Workfront Proof] Visningsprogrammet baseras på Flash och vi lagrar vissa uppgifter om korrektur (dvs. kommentarer, korrekturrutor, [!DNL Workfront Proof] visningsprograminställningar) på datorn med [!DNL Flash Player]. Om [!DNL Workfront Proof] Visningsprogrammet öppnas, men det finns inget innehåll inuti som du bör kontrollera att Flash-lagringsutrymmet är tillgängligt på datorn och att [!DNL Workfront Proof] får använda den.

Om det finns lite lagringsutrymme allokerat, men du arbetar med större korrektur med flera sidor och kommentarer, försök att öka [!DNL Flash] Lagring och ladda om ditt bevis.

Se vår [Problem med att visa korrektur - [!DNL Flash] Förklaring av delade objekt](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) för detaljerade anvisningar.

## Identifiera var problemet finns

* Öppnar korrekturen i en annan webbläsare?
* Om du använder en webbläsare dagligen och du har problem med att visa korrektur där kan du försöka öppna samma korrektur i en annan webbläsare på datorn. Det gör du genom att kopiera korrekturlänken från URL-fältet i huvudwebbläsaren och klistra in den i en annan webbläsare. Om korrekturet öppnas där kan du granska huvudwebbläsarkonfigurationen, plugin-program och tillägg eftersom dessa kan störa.
* Vi har ingen webbläsare att föredra, men om du har prestandaproblem i din nuvarande webbläsare rekommenderar vi att du byter till en annan.
* Öppnar korrekturen på en annan dator på din plats?
Om ditt korrektur inte öppnas i någon webbläsare på datorn kan du försöka öppna det på en annan dator på din plats och/eller utanför din plats. På så sätt kan du avgöra om ett problem beror på din dator eller om det är något i ditt lokala nätverk.
Om din säkerhetsnivå är högre ansluter du till [!DNL Workfront Proof] kan blockeras av:

   * Ditt lokala AV-program
   * Din nätverkslösning
   * Konfigurera DNS, brandvägg eller proxy
   * Det här är de inställningar som vi inte kan kontrollera. Det finns olika säkerhetslösningar tillgängliga och vi kan inte avgöra vilka som är implementerade i ditt nätverk och vilka som kan blockera anslutningar till [!DNL Workfront Proof]. Det är inte heller upp till [!DNL Workfront Proof] för att bestämma din interna säkerhetskonfiguration. Om du har problem med att öppna korrektur på flera datorer i ditt nätverk rekommenderar vi att du kontaktar IT-teamet så att de kan kontrollera nätverksinställningarna och auktorisera eller lägga till [!DNL Workfront Proof] till tillåtelselista, om det behövs.

* Är anslutningarna till [!DNL Workfront Proof] tillåts i ditt nätverk?
I korrekturläsaren läser vi in sidornas rutor - fragment. Om innehållet inte läses in korrekt kan det bero på att vissa anslutningar till [!DNL Workfront Proof] blockeras i ditt nätverk. Du måste se till att alla anslutningar och allt innehåll från *.proofhq.com läggs till i tillåtelselista. IT-avdelningen bör kunna hjälpa till att verifiera detta.

## Granska plugin-program

Om webbläsaren och [!DNL Flash Player] plugin-programmet är uppdaterat och nätverket blockerar inte anslutningarna till [!DNL Workfront Proof] det kan finnas något i webbläsaren som påverkar visningen av korrektur. Idag finns det flera plugin-program och tillägg i webbläsaren och vissa av dem stör eller står i konflikt med de andra.

Det bästa sättet är att ta bort alla okända tillägg och bara behålla de som du använder och som du litar på. Varje webbläsare bör ge dig alternativ för att kontrollera/ändra/ta bort plugin-program och tillägg. Våra [!DNL Workfront Proof] Visningsprogrammet är baserat på [!DNL Flash] och vi använder JavaScript för att läsa in visningsprogrammet så att du särskilt vill granska de plugin-program som kan påverka dessa.

Gå till nedanstående sidor för mer detaljerade instruktioner från utvecklarna om hur du inaktiverar webbläsartilläggen:

* Krom: [plugin-program](https://support.google.com/chrome/answer/142064?hl=en-GB) / [tillägg](https://support.google.com/chrome/answer/113907?hl=en-GB)
* Firefox: [tillägg](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer: [tillägg](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari: [tillägg](http://support.apple.com/en-gb/HT203353)

Om det finns något tillägg som stör inläsningen av korrektur kan du försöka kontrollera informationen i webbläsarens konsol.

![ProofView_4.png](assets/proofview-4-350x57.png)

I de flesta nyare webbläsare finns det ytterligare utvecklarverktyg tillgängliga och de kan användas för mer avancerad felsökning.

Om du har problem med att visa korrektur:

* Öppna webbläsarens konsol och läs in korrekturet igen.
* Kontrollera om det finns några varningar eller meddelanden i konsolen. Dessa uppgifter kan hjälpa till att identifiera vad som är orsaken till problemen.
* Låt IT-avdelningen analysera resultaten. De bör kunna ge råd och hjälpa till att lösa det lokala problemet.
* Dela resultaten med [supportteam](https://support.workfront.com/hc/en-us/requests/new). Vi hjälper gärna till.

Om du inte vet hur du öppnar konsolen i webbläsaren kan du läsa de registrerade stegen:

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS)
* [Internet Explorer](http://screencast.com/t/bYzq1iQv)
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj)
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

Du kan även läsa dokumentationen till webbläsarutvecklaren för mer detaljerade instruktioner.

## Kontrollera inställningar för blandat innehåll

Alla anslutningar till [!DNL Workfront Proof] är över HTTPS. I dialogrutan [!DNL Workfront Proof] Visningsprogrammet läser in rutorna via HTTP och data skyddas med tokens. Detta skapar blandat innehåll som vissa webbläsare eller säkerhetslösningar kan blockera (som standard eller enligt manuell konfiguration).

Om detta är orsaken till att korrektur inte öppnas på datorn (du bör kunna se de relevanta varningarna i webbläsarens konsol) godkänner du sådana anslutningar för [!DNL Workfront Proof] eller ändra inställningarna för att tillåta passivt blandat innehåll på datorn. Det blandade innehållet kan blockeras av webbläsaren, AV-programmet, nätverkskonfigurationen osv. - för att fastställa den exakta orsaken kontaktar du IT-teamet/nätverksadministratörerna. De bör också kunna hjälpa till att aktivera det blandade innehållet på din dator.

Kontakta oss [supportteam](https://support.workfront.com/hc/en-us/requests/new) om du behöver hjälp från vår sida.
