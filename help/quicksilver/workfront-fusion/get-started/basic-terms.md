---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Grundläggande termer i Adobe Workfront Fusion
description: Adobe Workfront Fusion kräver en Adobe Workfront Fusion-licens förutom en Adobe Workfront-licens.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---

# Grundläggande termer i [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver [!DNL Adobe Workfront Fusion] utöver en [!UICONTROL Adobe Workfront] licens.


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Åtgärd</p> </td> 
   <td>En modul som gör att du kan läsa eller skriva paket från eller till en vald app eller tjänst.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>En typ av modul som sammanfogar flera paket (flera datarrayer) till ett enda paket. Mer information finns i <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[!UICONTROL Aggregator] modulen i [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-nyckel</td> 
   <td>En unik kod som identifierar användaren, utvecklaren eller programmet som anropar en programvaras API, som används för autentisering. Sedan [!DNL Adobe Workfront Fusion] moduler fungerar genom att ansluta API:er. API-nycklar är ibland nödvändiga. API-nycklar distribueras av det program som kräver dem. Om du till exempel behöver en API-nyckel för [!DNL ActiveCampaign]begär du det via [!DNL ActiveCampaign] konto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Program eller tjänst</td> 
   <td> <p>Ett program, oftast.</p> <p>En app kan också vara en specialfunktion som hanterar data, till exempel en iterator eller en aggregator. </p> <p>En tjänst är en källa med paket som kan innehålla ett webb-API, en webbsida, olika typer av servrar (FTP, SMTP, IMAP) och så vidare. </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">App Connector</td> 
   <td>En app som ansluter till ett annat system.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Paket</p> </td> 
   <td> <p>Ett paket är en grundläggande enhet som returneras eller tas emot av moduler. Ett paket består av artiklar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>När du lägger till en app eller tjänst i ett scenario måste du troligen först skapa en anslutning mellan [!DNL Workfront Fusion] och programmet eller tjänsten för att hämta eller skicka valda data. Mer information finns i <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Anslutningar - översikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Cykel</p> </td> 
   <td> <p>En cykel refererar till två faser av scenariot som körs: operation och commit. Scenariot kan bestå av en eller flera cykler. Mer detaljerad information finns i <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datalager</p> </td> 
   <td> <p>Ett verktyg som lagrar data från scenarier eller gör det möjligt att överföra data mellan enskilda scenarier eller scenariokörningar. Mer information finns i <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Datalager i [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Dataöverföring</p> </td> 
   <td> <p>Mängden data som överförts via ditt scenario. Mer information finns i <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Scenarioinformation i [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filter</p> </td> 
   <td> <p>Ytterligare funktioner som kan användas mellan två moduler. Med ett filter kan du bara arbeta med paket som uppfyller vissa villkor. Det finns ett antal olika filter som du kan använda. Mer information finns i <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Lägga till ett filter i ett scenario i [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>Ett namn som används för att unikt identifiera ett paket. Ett ID används vanligtvis för att särskilja ett paket som ska uppdateras eller tas bort från en viss tjänst.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Objekt</p> </td> 
   <td> <p>En del av ett paket. Paket kan bestå av flera objekt. Det finns flera olika typer av alternativ: text, tal, booleskt (ja/nej), datum, tid, buffert (binära data), samlingar, markeringsmeny, matris och validering.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>En typ av modul som gör att du kan ta ett datapaket (en datamatris) och dela upp det i separata paket. Mer information finns i <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] modulen i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Modul</p> </td> 
   <td> <p>Ett enskilt steg i ett scenario som utför en funktion, till exempel att skapa en post, i det tillhörande programmet eller tjänsten.</p> <p>Varje program eller tjänst har olika moduler som definierar hur den svarar på en begäran.</p> <p>Det finns fyra typer av moduler: åtgärder, utlösare, iteratorer och aggregatorer.</p> <p> <img src="assets/module.jpg"> </p> <p>Mer information finns i <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Typer av moduler</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Åtgärd</p> </td> 
   <td> <p>En uppgift som utförs av en modul.</p><p>Mer information finns i <a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">Åtgärder i [!DNL Adobe Workfront Fusion]</a>.</p>
  </tr> 
  <tr> 
   <td role="rowheader">Offentliga/privata nycklar</td> 
   <td>Offentliga och privata nycklar används för att kryptera och dekryptera data. Den offentliga nyckeln kan distribueras och alla som har den offentliga nyckeln kan kryptera data, men bara den privata nyckeln kan dekryptera den. På samma sätt kan en användare med en privat nyckel kryptera data som alla med den offentliga nyckeln kan dekryptera. Krypteringen av den privata nyckeln garanterar att data kommer från den privata nyckelns ägare och fungerar som validering av datakällan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>Gör att du kan duplicera data eller lägga till nya vägar till ett scenario, så att du kan omdirigera data och hantera olika grupper av data separat. Mer information finns i <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">[!UICONTROL Router] modulen i [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Scenario</p> </td> 
   <td> <p>En serie automatiserade steg som skapats av användare, där varje steg representeras och utförs av en modul. Syftet med ett scenario är att flytta och hantera data.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Mer information finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i[!UICONTROL  Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transaktioner</p> </td> 
   <td> <p>[!DNL Workfront Fusion] använder transaktionsbearbetning för att fånga scenariots livscykel. En transaktion består av flera faser under vilka data omvandlas från ett konsekvent läge till ett annat konsekvent läge. Det finns fyra faser: initiering, åtgärd (läsning eller skrivning), implementering/återställning och slutförande.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Utlösare</p> </td> 
   <td> <p>En modul som gör att du kan hämta paket som har lagts till eller uppdaterats sedan den senaste körningen av ett scenario. Det finns två typer av utlösare: avsökning och direktutlösare (webhooks). Mer information finns i <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webkrok</p> </td> 
   <td> <p>En särskild typ av utlösare som gör att du kan köra ett scenario omedelbart efter det att ett nytt paket är tillgängligt. Mer information finns i <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Direktutlösare (webhooks) i [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
