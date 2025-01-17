---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenarieredigeraren i [!DNL Adobe] Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Scenarioredigeraren i [!DNL Adobe Workfront Fusion]

Med scenarioredigeraren kan du skapa och redigera scenarier i ett visuellt gränssnitt.

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Scenarieredigeraren i Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/navigate-workfront-fusion/scenario-editor.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

![](assets/scenario-editor.jpg)

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Öppna scenarioredigeraren:

1. Klicka på **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) i den vänstra panelen.

1. Om du vill skapa ett scenario klickar du på **[!UICONTROL Create a new scenario]** i det övre högra hörnet på sidan.

   eller

   Om du vill redigera ett befintligt scenario klickar du på scenariot.

   I scenarioredigeraren som visas kan du göra allt som anges i tabellen nedan. Mer information finns i [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. När du är klar med redigeringen av ett scenario (eller när som helst medan du redigerar) klickar du på ikonen [!UICONTROL Save]. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >När du har sparat ditt scenario kommer en ny version att finnas tillgänglig under menyn med tre punkter om du behöver komma åt den i framtiden. Tidigare sparade versioner är endast tillgängliga i 60 dagar.

## Tillgängliga scenarioredigeringsåtgärder

Följande åtgärder är tillgängliga i Scenarioredigeraren:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Lägg till den första modulen</td>
     <td> <p>Klicka på frågetecknet. <img src="assets/question-mark-full-size.png"></p> <p> Leta reda på och klicka sedan på programmet eller tjänsten som du vill börja med. Om du valde några appar i steg 2 visas de här för enkel åtkomst (och i avsnittet <strong>[!UICONTROL Favorites]</strong> längst ned på skärmen).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Lägga till en modul</td>
     <td>Håll pekaren över en modul, klicka på plusikonen till höger och klicka sedan på den modul du vill använda på menyn som visas.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Ange när och hur ofta scenariot ska köras</td>  
      <td> <p>Klicka på klockikonen. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Mer information finns i <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Schemalägg ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Ställ in ett flöde</td>   
     <td> <p>Klicka på ikonen [!UICONTROL wrench] <img src="assets/wrench-icon.gif"> mellan de två modulerna och använd något av följande alternativ:</p>    
       <ul>
         <li><strong>[!UICONTROL Set up a filter]</strong>: Kontrollera vilka paket som används vid vissa punkter i scenariot. Mer information finns i <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Lägga till ett filter i ett scenario i [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Unlink]</strong>: Tar bort en väg.</li>     
         <li><strong>[!UICONTROL Add a router]</strong>: Lägger till en router mellan moduler. </li>     
         <li><strong>[!UICONTROL Add a module]</strong>: Lägger till en ny modul mellan moduler.</li>     
         <li><strong>[!UICONTROL Add a note]</strong>: Lägger till en anteckning i flödet.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Ta bort en modul</td>   
     <td>Högerklicka på modulen och klicka sedan på <strong>[!UICONTROL Delete module]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Visa en logg över händelser som inträffar är ett scenario</td>     
     <td> 
       <p>Kör ett scenario. När scenariot har slutförts visas loggen i det nedre högra hörnet av [!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Beroende på scenariot kan loggen innehålla information om svårigheterna i varje fas och eventuella fel som uppstått under körningen av scenariot.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Konfigurera scenarioinställningarna</td>   
     <td>Klicka på ikonen [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> De här inställningarna är främst avsedda för avancerade användare.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Skriv eller visa anteckningar om scenariot</td>   
     <td>Klicka på ikonen [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Justera modulernas layout automatiskt </td>   
     <td>Klicka på ikonen [!UICONTROL Auto-align]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Visa en animering som visar hur data flödar genom scenariot</td>   <td>Klicka på ikonen [!UICONTROL Explain Flow]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exportera scenariot till datorn som en plan</td>   
     <td>Klicka på [!UICONTROL More]-menyn <img src="assets/more-icon.png"> och sedan på [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importera en scenarioplan från datorn</td>   
     <td>Klicka på [!UICONTROL More]-menyn <img src="assets/more-icon.png"> och sedan på [!UICONTROL Import Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Återställa en tidigare version av scenariot</td>   
     <td>Se artikeln <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Återställa en scenarioversion i [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Konfigurera inställningar för [!UICONTROL Flow Control]</td>   
     <td> <p>Klicka på ikonen [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Du kan ställa in en aktivitet så att den upprepas ett visst antal gånger, konvertera en array till en serie paket och sammanfoga flera paket till ett enda paket. Mer information finns i <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flödeskontroll i [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Förbättra scenariot med avancerade verktyg</td>   
     <td>Klicka på ikonen [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Du kan skapa utlösare, åtgärder, aggregatorer och transformatorer. Mer information finns i <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Verktyg</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Använda textanalysverktyg</td>   
     <td>Klicka på ikonen [!UICONTROL Text parser]. <img src="assets/text-parser-icon.gif"> Du kan hämta element från HTML-kod, söka efter och extrahera strängelement som matchar ett sökmönster, söka efter och ersätta text och"skrapa" data från en webbplats. Mer information finns i <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Verktyg</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Få tillgång till de mest använda programmen och tjänsterna</td>   
     <td> Klicka på en ikon i avsnittet <strong>[!UICONTROL Favorites]</strong> längst ned på skärmen. Ikoner visas automatiskt i det här avsnittet när du lägger till program och tjänster i ditt scenario. Du kan också klicka på ikonen Lägg till <img src="assets/add-icon.gif"> om du vill lägga till program och tjänster i det här området manuellt.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Testkör scenariot</td>   
     <td>Klicka på <strong>[!UICONTROL Run once]</strong> för att verifiera att scenariot körs som du förväntade dig innan du aktiverar det. När det är aktiverat körs scenariot enligt dess schema. Om allt inte fungerar som det ska kan du gå till avsnittet Felhantering och lära dig hur du hanterar fel.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Felsök scenariot med utvecklingsverktyget</td>   
     <td>Mer information finns i <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Felsöka scenarier med [!DNL Adobe Workfront Fusion] utvecklingsverktyget </a>.
</td> 
   </tr> 
<tr>
<td>Kontrollera scenariots status</td>
<td>Scenarier kan vara aktiva eller inaktiva. Du kan ändra scenariostatus genom att klicka på På/Av i scenarioinformationen.

Mer information finns i följande artiklar:
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">Aktivera eller inaktivera ett scenario i Adobe Workfront Fusion</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Scenarioinformation i Adobe Workfront Fusion</a></li>
</ul>
</td>
</tr>
<tr>
<td>Ändra scenariots schema</td>
<td>Aktiva scenarier körs enligt ett schema. Som standard körs ett scenario var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta ett aktiverat scenario körs. Fusionsscenarier kan schemaläggas så att de körs så ofta som var femte minut.

Mer information finns i <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">Schemalägg ett scenario i Adobe Workfront Fusion</a>.
</td>
</tr>
<tr>
<td>Byt namn på scenariot</td>
<td>Om du vill byta namn på ett scenario öppnar du det, klickar på scenariots namn i det övre vänstra hörnet och redigerar det. Tryck på Enter eller klicka utanför det redigerade fältet för att spara scenarionamnet.</td>
</tr>
<tr>
<td>Välj det första paketet</td>
<td>Vissa utlösarmoduler låter dig välja det första paket från vilket du vill att hämtningen av paket ska starta.

Mer information finns i <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">Välja var en utlösarmodul ska starta i Adobe Workfront Fusion</a>.</td>
</tr>
<tr>
<td>Ange antalet returnerade paket</td>
<td>Moduler returnerar som standard alltid bara två paket. Detta kan ändras i modulinställningarna i fältet [!UICONTROL Maximum number of returned bundles].</td>
</tr>
<tr>
<td>Konfigurera avancerade scenarioinställningar</td>
<td>[!DNL Adobe Workfront Fusion] ger dig möjlighet att konfigurera ett antal andra avancerade inställningar.

Mer information finns i <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md">Panelen för scenarioinställningar i Adobe Workfront Fusion</a>.</td>
</tr>
</tbody>
</table>
