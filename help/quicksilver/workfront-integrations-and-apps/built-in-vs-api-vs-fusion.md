---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Integreringsmetoder i Adobe Workfront
description: Du kan integrera [!DNL Adobe Workfront] med tredjepartsprogram. Dessa integreringar kan utöka verktyget för  [!DNL Workfront]  och anpassa det efter organisationens behov. Du kan använda någon eller alla av dessa integreringar, beroende på vilken som är mest användbar för en viss uppgift.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Integreringsmetoder i Adobe Workfront

Du kan integrera [!DNL Adobe Workfront] med tredjepartsprogram och andra [!DNL Adobe]-produkter. Dessa integreringar kan utöka verktyget för [!DNL Workfront] och anpassa det efter organisationens behov. Du kan använda någon eller alla av dessa integreringar, beroende på vilken som är mest användbar för en viss uppgift.

## Inbyggda integreringar

Workfront innehåller olika integreringar som du kan konfigurera direkt från Workfront eller från ett annat program genom att installera Workfront-tillägget för det programmet. Dessa inbyggda integreringar täcker många vanliga scenarier för användning och fokuserar på att utöka och koppla samman användarupplevelser för slutanvändare.

Workfront inbyggda integreringar fokuserar i hög grad på personlig produktivitet och samarbete. Dessa integreringar minskar avbrotten i en enskild användares arbetsflöde, vilket gör att användaren kan ta emot Workfront-meddelanden, få åtkomst till information och arbeta med Workfront-objekt utan att behöva lämna det integrerade programmet.

Fördelar med inbyggda integreringar kan vara följande:

* Många av dessa inbyggda integreringar är tillgängliga utan extra kostnad. (Andra kräver ett extra inköp.)
* Inbyggda integreringar täcker många av de vanligaste apparna som används av företag, till exempel [!DNL Slack], [!DNL Google Drive] eller [!DNL Adobe] produkter som [!DNL Adobe Creative Cloud] eller [!DNL Adobe Experience Manager] Assets. Om ditt företag redan använder dessa program kommer integreringen smidigt att ingå i användarnas befintliga arbetsflöde.
* Om du integrerar [!DNL Workfront] med ett program som används ofta kan det öka användandet bland dina användare.

>[!INFO]
>
>**Exempel:**
>
>Med [!DNL Workfront for Microsoft Teams integration] kan du få meddelanden i [!DNL Microsoft Teams] om dina [!DNL Workfront] arbetsobjekt. Utan att lämna [!DNL Microsoft Teams] kan du utföra åtgärder som att godkänna, kommentera eller ändra status för arbetsobjekt. Alla ändringar du gör i arbetsobjekt från [!DNL Microsoft Teams] återspeglas även i [!DNL Workfront].

Mer information om inbyggda integreringar, inklusive en lista över tillgängliga inbyggda integreringar, finns i [[!DNL Adobe Workfront] Inbyggda integreringsöversikt](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Anpassade OAuth2-program

Administratörer för Adobe [!DNL Workfront] kan skapa OAuth2-program för din instans av [!DNL Workfront], som ger andra program åtkomst till [!DNL Workfront]. Dina användare kan sedan ge dessa andra program behörighet att komma åt sina [!DNL Workfront]-data. På så sätt kan du integrera Workfront med valfria program, inklusive egna, interna program.

>[!NOTE]
>
>När det gäller OAuth2 avser&quot;skapa en app&quot; processen att skapa den här typen av åtkomstlänk mellan en app och en server som Workfront.

Fördelarna med att skapa ett [!UICONTROL OAuth2]-program kan vara följande:

* Användare kan använda dessa integreringar direkt i [!DNL Workfront], på liknande sätt som inbyggda integreringar.
* Att konfigurera eller använda ett [!UICONTROL OAuth2]-program kräver ingen ytterligare teknisk kunskap, till exempel kunskap om [!DNL Workfront] API:t.
* Din organisation kan använda programvara som inte erbjuds som ett [!DNL Workfront]-inbyggt program. Du kan fortfarande integrera den här programvaran med [!DNL Workfront] genom att använda ett [!UICONTROL OAuth2]-program, även om programvaran är företagsspecifik.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](../administration-and-setup/configure-integrations/create-oauth-application.md).

## API för [!DNL Workfront]

[!DNL Workfront] har ett offentligt API (Application Programming Interface) som gör att du kan utöka och förbättra din Workfront-upplevelse. Målet för API:t [!DNL Workfront] är att förenkla skapandet av dina egna integreringar med [!DNL Workfront] genom att införa en REST-full arkitektur som fungerar över HTTP. API:t [!DNL Workfront] kräver viss teknisk kunskap, men det är ett mycket kraftfullt verktyg för att hämta, skapa och ändra data. Du kan anpassa API-anrop för att utföra mycket specifika funktioner.

Dessutom erbjuder [!DNL Workfront] ett Event Subscription API. När en åtgärd inträffar för ett [!DNL Workfront]-objekt som stöds av händelseprenumerationer, kan du konfigurera [!DNL Workfront] så att ett svar skickas till den önskade slutpunkten. Detta innebär att tredjepartsprogram kan ta emot uppdateringar från [!DNL Workfront]-interaktioner via [!DNL Workfront] API:t strax efter att de har inträffat.

Fördelar med att använda API:t [!DNL Workfront] kan vara följande:

* Du kan använda API:t [!DNL Workfront] för att ansluta till nästan alla andra webbtjänster eller appar som har ett offentligt API. Det är därför möjligt att integrera [!DNL Workfront] med nästan alla webbtjänster och appar som du vill använda.
* [!DNL Workfront]-API:ts flexibilitet omfattar även ditt företags egna programvara. Du kan använda och ändra [!DNL Workfront]-data inifrån din egen programvara.
* Eftersom API:er är så vanliga för programvara är det troligt att de interna utvecklarna känner till dem. [!DNL Workfront] använder ett REST-fyllt API, den vanligaste typen av API, vilket gör det ännu enklare för dina utvecklare att komma igång snabbt.

>[!INFO]
>
>**Exempel:**
>
>Följande API-anrop placerar en kommentar i aktivitetens uppdateringsström med angivet ID.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Mer information om API:t [!DNL Workfront] finns i [Grunderna i API ](../wf-api/general/api-basics.md).

Mer information om händelseprenumerationer finns i [API för händelseprenumeration](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

Med [!DNL Workfront Fusion] kan du automatisera arbetsflöden. Med [!DNL Workfront Fusion for Work Automation and Integration]-licensen kan du skapa dessa automatiseringar för flera appar och webbtjänster och skapa scenarier där programmen fungerar tillsammans för att utföra en uppgift. Ett scenario är en visuell representation av den uppgift eller det arbetsflöde som byggs med hjälp av moduler, som är separata uppgifter som&quot;Hämta ett dokument&quot; eller&quot;Skapa ett projekt&quot;. Du sammanför moduler för att definiera arbetsflödet, och sedan körs arbetsflödet automatiskt när ett utlösande villkor uppfylls.

Fördelar med [!DNL Workfront Fusion] kan omfatta följande:

* [!DNL Workfront Fusion] kräver inte så mycket teknisk kunskap som API:t eftersom det visuella gränssnittet gör det lättare att förstå och konfigurera arbetsflödet. Det innebär att det kan användas av individer utanför ett utvecklingsteam, vilket kan spara tid och pengar åt organisationen.
* Eftersom [!DNL Workfront Fusion] arbetar via API:t har den åtkomst till de flesta program och webbtjänster. Många program har moduler för att göra API-anrop, eller så kan du använda HTTP-, SOAP- eller JSON-modulerna för att interagera med webbtjänster som inte har någon dedikerad [!DNL Workfront Fusion]-anslutning.

>[!INFO]
>
>**Exempel:**
>
>Följande [!DNL Workfront]-modul i [!DNL Workfront Fusion] har konfigurerats för att lägga till en kommentar i det valda projektet. När modulen har körts visas kommentaren i projektets uppdateringsström i Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Mer information om [!DNL Workfront Fusion] finns i [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
