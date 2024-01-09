---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Felsökning - [!DNL Workfront Proof] korrekturläsare
description: Om ditt korrekturinnehåll inte läses in och du bara kan se ett tomt korrekturläsare, är det troligtvis därför att något blockerar den här åtgärden lokalt.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Felsökning - [!DNL Workfront Proof] korrekturläsare

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om ditt korrekturinnehåll inte läses in och du bara kan se ett tomt korrekturläsare, är det troligtvis därför att något blockerar den här åtgärden lokalt. Prova de möjliga lösningarna nedan.

## Kontrollera webbläsaren <!--and [!DNL Flash Player]--> versionen är uppdaterad

Alla utvecklare arbetar hela tiden med sina program och de släpper regelbundet nya funktioner och korrigeringar för sina produkter. Detta är för att förbättra användarupplevelsen och upprätthålla säkerhetsnivån så att det är den bästa metoden att endast använda de senaste versionerna. Detta hjälper också till att undvika konflikter mellan programmen.

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### Webbläsarversion

Vanligtvis uppdateras de flesta webbläsare automatiskt, men om du har problem bör du kontrollera vilken version du använder och utföra en uppdatering, om det behövs.

Gå till webbläsaren [!UICONTROL Menu] och hitta [!UICONTROL About] (i vissa fall kan detta vara synligt under [!UICONTROL Help] meny). I [!UICONTROL About] I finns information om den aktuella webbläsarversionen och även ett alternativ för att uppdatera/söka efter uppdateringar.

I Chrome:

![Chrome-webbläsarversion](assets/proofview-3.png)

När du har installerat den senaste webbläsarversionen kan du försöka att öppna korrekturet igen och se om problemet är löst.

<!--
## Ensure Your Local [!DNL Flash] Storage is Available

Our [!DNL Workfront Proof] Viewer is based on Flash, and we store some data about the proofs (i.e., comments, proof tiles, [!DNL Workfront Proof] Viewer settings) on your computer using [!DNL Flash Player]. If the [!DNL Workfront Proof] Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that [!DNL Workfront Proof] is allowed to use it.

If there is some storage allocated, but you're working with the bigger proofs with multiple pages and comments try to increase the [!DNL Flash] Storage and re-load your proof.

Please see [Problems With Viewing Proofs - [!DNL Flash] Shared Objects Explained](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) for the detailed instructions.
-->

## Identifiera var problemet finns

* Öppnar korrekturen i en annan webbläsare?
* Om du använder en webbläsare varje dag och har problem med att visa korrektur där, kan du försöka öppna samma korrektur i en annan webbläsare på datorn. Det gör du genom att kopiera korrekturlänken från URL-fältet i huvudwebbläsaren och klistra in den i en annan webbläsare. Om korrekturet öppnas där kan du granska huvudwebbläsarkonfigurationen, plugin-program och tillägg eftersom dessa kan störa.
* Vi har ingen föredragen webbläsare, men om du har prestandaproblem i din nuvarande webbläsare rekommenderar vi att du byter till en annan.
* Öppnar korrekturen på en annan dator på din plats?
Om ditt korrektur inte öppnas i någon webbläsare på datorn kan du försöka öppna det på en annan dator på din plats och/eller utanför din plats. På så sätt kan du avgöra om ett problem har uppstått på din dator eller om problemet har uppstått i ditt lokala nätverk.
Om säkerhetsnivån är högre ansluter du till [!DNL Workfront Proof] kan blockeras av:

   * Ditt lokala AV-program
   * Din nätverkslösning
   * DNS-, brandväggs- eller proxykonfiguration
   * Det här är de inställningar som vi inte kan kontrollera. Det finns olika säkerhetslösningar tillgängliga och vi kan inte avgöra vilka som är implementerade i ditt nätverk och vilka som kan blockera anslutningar till [!DNL Workfront Proof]. Det är inte heller upp till [!DNL Workfront Proof] för att bestämma din interna säkerhetskonfiguration. Om du har problem med att öppna korrektur på flera datorer i ditt nätverk rekommenderar vi att du kontaktar IT-teamet så att de kan kontrollera nätverksinställningarna och auktorisera eller lägga till [!DNL Workfront Proof] till tillåtelselista, om det behövs.

* Är anslutningarna till [!DNL Workfront Proof] tillåts i ditt nätverk?
I korrekturläsaren läser vi in sidrutorna - fragment av sidorna. Om innehållet inte läses in som det ska i slutet kan det bero på att vissa anslutningar till [!DNL Workfront Proof] är blockerade i ditt nätverk. Du måste se till att alla anslutningar och allt innehåll från *.proofhq.com läggs till i tillåtelselista. IT-avdelningen bör kunna hjälpa till att verifiera detta.

## Granska plugin-program

Om webbläsaren är uppdaterad och nätverket inte blockerar anslutningarna till [!DNL Workfront Proof]kan det finnas något i webbläsaren som påverkar visningen av korrektur. Det finns ofta flera plugin-program och tillägg tillgängliga i webbläsaren, och vissa av dem kan störa eller stå i konflikt med de andra.

Det bästa sättet är att ta bort alla okända tillägg och bara behålla de som du använder och som du litar på. Varje webbläsare bör ge dig alternativ för att kontrollera/ändra/ta bort plugin-program och tillägg. Vi använder JavaScript för att läsa in [!DNL Workfront Proof] visningsprogrammet så att du särskilt vill granska de plugin-program som kan påverka det.

Om det finns något tillägg som stör inläsningen av korrektur kan du försöka kontrollera informationen i webbläsarens konsol.

![Webbläsarkonsol](assets/proofview-4.png)

I de flesta nyare webbläsare finns det ytterligare utvecklarverktyg tillgängliga, och de kan användas för mer avancerad felsökning.

Om du har problem med att visa korrektur:

* Öppna webbläsarens konsol och läs in korrekturet igen.
* Kontrollera om det finns några varningar eller meddelanden i konsolen. Dessa uppgifter kan hjälpa till att identifiera vad som är orsaken till problemen.
* Låt IT-avdelningen analysera resultaten. De bör kunna ge råd och hjälpa till att lösa det lokala problemet.
* Dela resultaten med vårt supportteam. Vi hjälper gärna till.

## Kontrollera inställningar för blandat innehåll

Alla anslutningar till [!DNL Workfront Proof] är över HTTPS. I dialogrutan [!DNL Workfront Proof] Visningsprogrammet läser in rutorna via HTTP och data skyddas med tokens. Detta skapar blandat innehåll som vissa webbläsare eller säkerhetslösningar kan blockera (som standard eller genom manuell konfiguration).

Om detta är orsaken till att korrekturen inte öppnas på datorn (du bör kunna se de relevanta varningarna i webbläsarens konsol) måste du godkänna sådana anslutningar för [!DNL Workfront Proof] eller ändra inställningarna för att tillåta passivt blandat innehåll på datorn. Det blandade innehållet kan blockeras av webbläsaren, AV-programmet eller nätverkskonfigurationen för att fastställa den exakta orsaken. Kontakta IT-avdelningen/nätverksadministratörerna. De bör också kunna hjälpa till att aktivera det blandade innehållet på din dator.


