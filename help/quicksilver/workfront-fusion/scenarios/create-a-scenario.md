---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Skapa ett scenario i Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1398'
ht-degree: 0%

---

# Skapa ett scenario i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Arbetsflöde för att skapa ett scenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Följande uppgifter förklarar hur du skapar ett [!DNL Adobe Workfront Fusion]-scenario.

En övning som vägleder dig genom att skapa ett automatiseringsscenario finns i [Skapa ett scenario för övningsautomatisering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

En övning som vägleder dig genom att skapa ett integreringsscenario med hjälp av data som vi tillhandahåller finns i [Skapa ett scenario för praktikintegrering i Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Mer information om hur du skapar ett scenario från en mall finns i [Skapa scenarier med  [!DNL Adobe Workfront Fusion] mallar](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront</td>  
      <td>Alla</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront-licens</td>  
      <td>
        Nytt: Standard<br>
        Eller<br>
        Aktuell: Arbete eller högre
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion-licens</td>  
      <td> 
        Aktuell: Inga Workfront Fusion-licenser krävs.<br>
        Eller<br>
        Äldre: Alla
      </td>  
    </tr>  
    <tr>  
      <td>Produkt</td>  
      <td> 
        Nytt: Välj eller Prime Workfront Plan: Din organisation måste köpa Adobe Workfront Fusion.<br>
        Ultimate Workfront Plan: Workfront Fusion ingår.<br>
        Eller<br>
        Aktuell: Din organisation måste köpa Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Börja skapa ett scenario

1. Klicka på **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) i den vänstra panelen.

1. Klicka på **[!UICONTROL Create a new scenario]** i det övre högra hörnet på sidan.
1. Om du skapar ett nytt scenario klickar du på **[!UICONTROL New scenario]** i det övre vänstra hörnet på skärmen som visas (scenarioredigeraren) och anger ett namn för scenariot.
1. Fortsätt till [Lägg till en modul i ett scenario](#add-a-module-in-a-scenario).

## Lägga till en modul i ett scenario

1. Klicka på frågetecknet om du vill lägga till den första modulen i scenariot. ![](assets/question-mark-icon.gif)

   eller

   Om du vill lägga till ytterligare moduler i scenariot klickar du på handtaget till höger om modulen som du vill att det ska följa.

1. I rutan som visas söker du efter och klickar på programmet eller tjänsten som du vill börja med.

   Tidigare valda appar visas i rutan för enkel åtkomst och i avsnittet **[!UICONTROL Favorites]** längst ned på skärmen.

   Om du klickar på **[!UICONTROL Add another module]** beror de moduler som visas på var i scenariot du lägger till modulen. Vissa moduler kan bara placeras mellan andra moduler och andra bara i början av scenariot.

   >[!TIP]
   >
   >De två vanligaste modultyperna är åtgärder och utlösare. Mer information finns i [Typer av moduler](../../workfront-fusion/modules/module-types.md).

1. Klicka på den första modulen som du vill lägga till i scenariot i listan med moduler som visas.

   Vilka moduler som visas beror på var du vill lägga till en modul i ditt scenario. Vissa moduler kan bara placeras mellan andra moduler och andra bara i början av scenariot.

   De två vanligaste modultyperna är åtgärder och utlösare. Mer information finns i [Typer av moduler](../../workfront-fusion/modules/module-types.md).

1. Fortsätt till [Anslut modulens app eller webbtjänst till  [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Anslut modulens app eller webbtjänst till [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion-moduler som ansluter till ett program (till exempel [!DNL Workfront], [!DNL Salesforce] eller [!DNL Jira)] innehåller fältet [!UICONTROL Connection]. Här kan du ange den anslutning som du vill att den här modulen ska använda för att ansluta till programmet. Du kan välja en befintlig anslutning i listrutan eller skapa en ny anslutning.

När du väljer eller skapar en anslutning för ett program i ett scenario använder andra moduler för det programmet automatiskt samma anslutning, såvida du inte väljer en annan anslutning när du konfigurerar de senare modulerna.

Mer information finns i [Anslutningsöversikt](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Så här skapar du en anslutning inuti en [!DNL Workfront Fusion]-modul:

1. Klicka på **[!UICONTROL Add]** för att öppna rutan **[!UICONTROL Create a connection]**.
1. (Valfritt) Ändra standardvärdet **[!UICONTROL Connection name]**.
1. (Villkorligt) Om programmet kräver avancerade anslutningsinställningar, till exempel ett ID, en nyckel eller [!UICONTROL secret], anger du den informationen.

   Du kan behöva klicka på **[!UICONTROL Show advanced settings]** för att visa fälten där du kan ange den här typen av information.

1. Klicka på **[!UICONTROL Continue]**.
1. I inloggningsfönstret som visas anger du dina inloggningsuppgifter för att logga in på appen om du inte redan har gjort det.
1. (Villkorligt) Om en **[!UICONTROL Allow]**-knapp visas kontrollerar du de åtgärder som anslutningsprogrammet kan utföra och klickar sedan på knappen för att ansluta appen till [!DNL Workfront Fusion].
1. Fortsätt till [Konfigurera modulen](#configure-the-module).


## Konfigurera modulen

1. Konfigurera inställningarna för modulen i fälten under anslutningsfältet och klicka sedan på **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   De här inställningarna är olika för alla moduler. En rubrik med fet stil anger en obligatorisk inställning.

   >[!TIP]
   >
   >När du arbetar med ditt scenario kan du när som helst klicka på modulen för att visa den här rutan med inställningar.
   >
   >
   >Om du ser en svart cirkel i en modul har du inte konfigurerat inställningarna för den. Klicka på modulen för att öppna den och fortsätta konfigurera.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Om du lägger till den första modulen i ditt scenario väljer du ett alternativ som anger var du vill att scenariot ska börja varje gång det körs.

   ![](assets/choose-where-start-350x194.png)

1. Upprepa stegen i avsnitten [Lägg till en modul i ett scenario](#add-a-module-in-a-scenario) och [Konfigurera modulen](#configure-the-module) för att lägga till andra moduler i scenariot.

1. (Valfritt) Kopiera och klistra in en modul eller en grupp med moduler.

   Mer information finns i [Kopiera moduler eller scenarier i Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Fortsätt till [Konfigurera och arbeta med ditt scenario](#configure-and-work-with-your-scenario).

## Konfigurera och arbeta med ditt scenario

1. Gör något av följande för att konfigurera ditt scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ange när och hur ofta scenariot ska köras</td> 
      <td> <p>Klicka på klockikonen. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Mer information finns i <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Schemalägg ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ställ in ett flöde</td> 
      <td> <p>Klicka på skiftnyckelsikonen <img src="assets/wrench-icon.gif"> mellan de två modulerna och använd något av följande alternativ. Mer information finns i <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Lägga till ett filter i ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Set up a filter]</strong>: Kontrollera vilka paket som används vid vissa punkter i scenariot.</li> 
        <li><strong>[!UICONTROL Unlink]</strong>: Tar bort en väg.</li> 
        <li><strong>[!UICONTROL Add a router]</strong>: Lägger till en router mellan moduler. </li> 
        <li><strong>[!UICONTROL Add a module]</strong>: Lägger till en ny modul mellan moduler.</li> 
        <li><strong>[!UICONTROL Add a note]</strong>: Lägger till en anteckning i flödet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfigurera scenarioinställningarna</td> 
      <td>Klicka på ikonen [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> De här inställningarna är främst avsedda för avancerade användare. Mer information finns i <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfigurera inställningar för flödeskontroll</td> 
      <td> <p>Klicka på ikonen [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Du kan ställa in en aktivitet så att den upprepas ett visst antal gånger, konvertera en array till en serie paket och sammanfoga flera paket till ett enda paket. Mer information finns i <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flödeskontroll i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förbättra scenariot med avancerade verktyg</td> 
      <td>Klicka på ikonen [!DNL Tools]. <img src="assets/tools-icon.gif"> Du kan skapa utlösare, åtgärder, aggregatorer och transformatorer. Mer information finns i <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Verktyg</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verktyg för textanalys</td> 
      <td>Klicka på ikonen [!DNL Text parser] <img src="assets/text-parser-icon.gif">. Du kan hämta element från HTML-kod, söka efter och extrahera strängelement som matchar ett sökmönster, söka efter och ersätta text och"skrapa" data från en webbplats. Mer information finns i <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Verktyg</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Gör något av följande för att arbeta med ditt scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visa en logg över händelser som inträffar när scenariot körs</td> 
      <td> <p>Klicka på pilen [!UICONTROL Exit editing] <img src="assets/exit-editing-arrow.png"> i scenarioredigeraren för att visa sidan Scenarioinformation. Loggen visas längst ned i fönstret eller i det nedre högra hörnet. Den innehåller information om varje fas och eventuella fel som uppstått under körningen av scenariot.</p> <p>Om du vill återgå till att arbeta med ditt scenario i [!DNL scenario editor] klickar du var som helst på sidan Scenarioinformation.</p> <p>Mer information om sidan Scenarioinformation finns i <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Scenarioinformation i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Få tillgång till de mest använda programmen och tjänsterna</td> 
      <td> Klicka på en ikon i avsnittet <strong>[!UICONTROL Favorites]</strong> längst ned på skärmen. Ikoner visas automatiskt i det här avsnittet när du lägger till program och tjänster i ditt scenario. Du kan också klicka på ikonen [!UICONTROL Add] <img src="assets/add-icon.gif"> om du vill lägga till program och tjänster i det här området manuellt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa en animering som visar hur data flödar genom scenariot</td> 
      <td>Klicka på ikonen [!UICONTROL Explain flow] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Justera modulernas layout automatiskt </td> 
      <td>Klicka på ikonen [!UICONTROL Auto-align] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skriv eller visa anteckningar om scenariot</td> 
      <td>Klicka på ikonen [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort en modul</td> 
      <td>Högerklicka på modulen och klicka sedan på <strong>[!UICONTROL Delete module]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Om du vill testa och köra scenariot klickar du på **[!UICONTROL Run once]**.

   Det är viktigt att kontrollera att scenariot fungerar som du tänkt dig innan du aktiverar det. När det är aktiverat körs scenariot enligt dess schema. Om allt inte fungerar som det ska läser du [Felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. När du är klar med redigeringen av scenariot (eller när som helst medan du redigerar) klickar du på ikonen [!UICONTROL Save] längst ned i fönstret ![](assets/save-icon.gif).

Mer information om hur du aktiverar ett scenario finns i [Aktivera eller inaktivera ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Kortkommandon för Workfront Fusion-scenarier

Du kan använda följande kortkommandon när du skapar eller redigerar ett scenario:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Åtgärd</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Ctrl+Skift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Skift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Run Once]</td> 
   <td>Ctrl+Skift+Retur</td> 
   <td><span style="font-weight: normal;">Cmd+Skift+Retur</span> </td> 
  </tr> 
 </tbody> 
</table>
