---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Integreringsmetoder i Adobe Workfront
description: Ni kan integrera [!DNL Adobe Workfront] med program från tredje part. Dessa integreringar kan göra att [!DNL Workfront] och skräddarsy den efter organisationens behov. Du kan använda någon eller alla av dessa integreringar, beroende på vilken som är mest användbar för en viss uppgift.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 0%

---

# Integreringsmetoder i Adobe Workfront

Ni kan integrera [!DNL Adobe Workfront] med program från tredje part. Dessa integreringar kan göra att [!DNL Workfront] och skräddarsy den efter organisationens behov. Du kan använda någon eller alla av dessa integreringar, beroende på vilken som är mest användbar för en viss uppgift.

## Inbyggda integreringar

Workfront innehåller olika integreringar som du kan konfigurera direkt från Workfront eller från ett annat program genom att installera Workfront-tillägget för det programmet. Dessa inbyggda integreringar täcker många vanliga scenarier för användning och fokuserar på att utöka och koppla samman användarupplevelser för slutanvändare.

Workfront inbyggda integreringar fokuserar i hög grad på personlig produktivitet och samarbete. Dessa integreringar minskar avbrotten i en enskild användares arbetsflöde, vilket gör att användaren kan ta emot Workfront-meddelanden, få åtkomst till information och arbeta med Workfront-objekt utan att behöva lämna det integrerade programmet.

Fördelar med inbyggda integreringar kan vara följande:

* Många av dessa inbyggda integreringar är tillgängliga utan extra kostnad. (Andra kräver ett extra inköp.)
* Inbyggda integreringar täcker många av de vanligaste apparna som används av företag, till exempel [!DNL Slack], [!DNL Google Drive], eller [!DNL Adobe] produkter som [!DNL Adobe Creative Cloud] eller [!DNL Adobe Experience Manager] Resurser. Om ditt företag redan använder dessa program kommer integreringen smidigt att ingå i användarnas befintliga arbetsflöde.
* Integrera [!DNL Workfront] med ett program som används ofta kan användarna bli mer mottagliga.

>[!INFO]
>
>**Exempel:**
>
>Med [!DNL Workfront for Microsoft Teams integration]kan du få meddelanden i [!DNL Microsoft Teams] om [!DNL Workfront] arbetsposter. Utan att lämna [!DNL Microsoft Teams]kan du utföra åtgärder som att godkänna, kommentera eller ändra status för arbetsobjekt. Alla ändringar du gör i arbetsobjekt från [!DNL Microsoft Teams] återspeglas i [!DNL Workfront] också.

Mer information om inbyggda integreringar, inklusive en lista över tillgängliga inbyggda integreringar, finns i [[!DNL Adobe Workfront] inbyggd integreringsöversikt](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Anpassade OAuth2-program

Adobe [!DNL Workfront] administratörer kan skapa OAuth2-program för din instans av [!DNL Workfront]som ger andra program åtkomst [!DNL Workfront]. Användarna kan sedan ge dessa andra program behörighet att komma åt sina [!DNL Workfront] data. På så sätt kan du integrera Workfront med valfria program, inklusive egna, interna program.

>[!NOTE]
>
>När det gäller OAuth2 avser&quot;skapa en app&quot; processen att skapa den här typen av åtkomstlänk mellan en app och en server som Workfront.

Fördelar med att skapa en [!UICONTROL OAuth2] kan omfatta följande:

* Användarna kan använda dessa integreringar direkt i [!DNL Workfront], som inbyggda integreringar.
* Konfigurera eller använda en [!UICONTROL OAuth2] programmet inte kräver någon ytterligare teknisk kunskap, som att känna till [!DNL Workfront] API.
* Din organisation kan använda programvara som inte erbjuds som [!DNL Workfront] inbyggd applikation. Du kan fortfarande integrera programvaran med [!DNL Workfront] genom att använda [!UICONTROL OAuth2] -program, även om programvaran är tillverkarspecifik för din organisation.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] har ett offentligt API (Application Programming Interface) som gör att du kan utöka och förbättra din Workfront-upplevelse. Målet för [!DNL Workfront] API är att förenkla byggandet av egna integreringar med [!DNL Workfront] genom att införa en REST-full arkitektur som fungerar över HTTP. The [!DNL Workfront] API kräver viss teknisk kunskap, men det är ett mycket kraftfullt verktyg för att hämta, skapa och ändra data. Du kan anpassa API-anrop för att utföra mycket specifika funktioner.

Dessutom [!DNL Workfront] erbjuder ett API för händelseprenumeration. När en åtgärd utförs på en [!DNL Workfront] objekt som stöds av händelseprenumerationer, kan du konfigurera [!DNL Workfront] för att skicka ett svar till den önskade slutpunkten. Detta innebär att tredjepartsprogram kan ta emot uppdateringar från [!DNL Workfront] interaktioner via [!DNL Workfront] API strax efter att de har inträffat.

Fördelar med att använda [!DNL Workfront] API kan innehålla följande:

* Du kan använda [!DNL Workfront] API för att ansluta till nästan alla andra webbtjänster eller appar som har ett offentligt API. Det är därför möjligt att integrera [!DNL Workfront] med nästan vilken webbtjänst eller app du vill använda.
* The [!DNL Workfront] API:ts flexibilitet kan även omfatta företagets egna programvaror. Du kan använda och ändra [!DNL Workfront] data inifrån era egna program.
* Eftersom API:er är så vanliga för programvara är det troligt att de interna utvecklarna känner till dem. [!DNL Workfront] använder en REST-ful API, den vanligaste typen av API, vilket gör det ännu enklare för utvecklarna att komma igång snabbt.

>[!INFO]
>
>**Exempel:**
>
>Följande API-anrop placerar en kommentar i aktivitetens uppdateringsström med angivet ID.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Mer information om [!DNL Workfront] API, se [Grunderna i API](../wf-api/general/api-basics.md).

Mer information om händelseprenumerationer finns i [API för händelseprenumeration](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] gör att du kan automatisera arbetsflöden. Med [!DNL Workfront Fusion for Work Automation and Integration] kan ni skapa dessa automatiseringar för flera program och webbtjänster och skapa scenarier där programmen samverkar för att utföra en uppgift. Ett scenario är en visuell representation av den uppgift eller det arbetsflöde som byggs med hjälp av moduler, som är separata uppgifter som&quot;Hämta ett dokument&quot; eller&quot;Skapa ett projekt&quot;. Du sammanför moduler för att definiera arbetsflödet, och sedan körs arbetsflödet automatiskt när ett utlösande villkor uppfylls.

Fördelar med [!DNL Workfront Fusion] kan omfatta följande:

* [!DNL Workfront Fusion] kräver inte så mycket teknisk kunskap som API:t, eftersom det visuella gränssnittet hjälper till att förstå och konfigurera arbetsflödet. Det innebär att det kan användas av individer utanför ett utvecklingsteam, vilket kan spara tid och pengar åt organisationen.
* Sedan [!DNL Workfront Fusion] fungerar via API:t och har tillgång till de flesta program och webbtjänster. Många program har moduler som gör API-anrop, eller så kan du använda HTTP-, SOAP- eller JSON-modulerna för att interagera med webbtjänster som inte har någon dedikerad [!DNL Workfront Fusion] koppling.

>[!INFO]
>
>**Exempel:**
>
>Följande [!DNL Workfront] modulen i [!DNL Workfront Fusion] är konfigurerad för att lägga till en kommentar i det valda projektet. När modulen har körts visas kommentaren i projektets uppdateringsström i Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Mer information om [!DNL Workfront Fusion], se [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
