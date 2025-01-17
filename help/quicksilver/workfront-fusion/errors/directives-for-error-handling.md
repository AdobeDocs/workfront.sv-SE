---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Direktiv för felhantering i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%

---

# Direktiv för felhantering i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Direktiv för felhantering](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/directives-for-error-handling.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

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

## Direktiv för felhantering

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Återställning</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>Scenariokörningen stoppas omedelbart och en <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">återställningsfas</a> startas på alla moduler i ett försök att återställa alla till deras ursprungliga tillstånd. De efterföljande modulerna bearbetas inte.</p> <p>Om du utelämnar ett fåtal feltyper inaktiveras scenariot efter det antal på varandra följande fel som anges under scenarieinställningarna. Mer information finns i <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Antal efterföljande fel</a>.</p> <p>Scenariots körningsstatus är markerad som "error".</p> <p>Obs! Detta är standardbeteendet om ingen felhanterarväg är kopplad till modulen och inställningen <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Allow storing incomplete executions]</a> under [!UICONTROL Scenario settings] inte är markerad.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Verkställ</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>Scenariokörningen stoppas omedelbart och en implementeringsfas startas på alla moduler. De efterföljande modulerna bearbetas inte.</p> <p>Alla obearbetade paket ignoreras.</p> <p>Scenariots körningsstatus är markerad som "success". Mer information om implementeringsfaser finns i <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Genomför</a> i artikeln <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Scenariokörning, cykler och faser i Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Återuppta</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Ett ersättningsutdata anges och skickas till modulen som påträffar ett fel.</p> <p>De efterföljande modulerna bearbetas.</p> <p>Scenariots körningsstatus är markerad som "success".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorera</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>Felet ignoreras och efterföljande moduler bearbetas inte.</p> <p>Om det finns obearbetade paket fortsätter scenariokörningen normalt.</p> <p>Scenariots körningsstatus är markerad som "success".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Brytning</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>Scenario-körningens tillstånd lagras i kön med ofullständiga körningar där felet kan lösas manuellt. Mer information finns i <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Visa och lösa ofullständiga körningar i Adobe Workfront Fusion</a>. </p> <p>Det finns dock några undantag. Mer information finns i <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Tillåt lagring av ofullständiga körningar</a> i artikeln <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Panelen för scenarioinställningar i Adobe Workfront Fusion</a>.</p> <p>De efterföljande modulerna bearbetas inte.</p> <p>Om det finns obearbetade paket fortsätter scenariokörningen normalt.</p> <p>Scenariots körningsstatus är markerad som "varning" när alternativet [!UICONTROL Automatically complete execution] är inaktiverat.</p> <p>Mer information finns i avsnittet <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> nedan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Försök igen</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>I vissa fall kan det vara användbart att köra en felande modul igen ett par gånger när det finns en möjlighet att orsaken till felet kan passera över tiden.</p> <p>Workfront Fusion innehåller för närvarande inte direktivet Retry, men det går att använda flera tillfälliga lösningar för att efterlikna dess funktionalitet. Mer information finns i <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Försök att hantera fel igen i Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Felhanteringsdirektiven kan för närvarande inte användas utanför en felhanteringsväg.
>
>   Mer information finns i [Felhanterarväg](../../workfront-fusion/errors/error-handling.md#error) i artikeln [Felhantering i Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] har för närvarande ingen Throw-modul som gör att du enkelt kan generera (utlösa) fel villkorligt, men en tillfällig lösning kan användas för att efterlikna dess funktioner.
>
>   Mer information finns i [Lösning för Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw) i artikeln [Hantering av utlösta fel i Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Brytning {#break}

När ett fel hanteras av direktivet [!DNL Break] skapas en post i mappen Ofullständiga körningar. Den här posten lagrar läget för scenariokörningen tillsammans med data från tidigare moduler. Posten refererar till modulen där felet uppstod och innehåller information om vilka data som togs emot av modulen som indata. För varje datapaket som orsakar felet skapas en separat post.

Mer information finns i [Visa och lösa ofullständiga körningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Åtgärda fel som uppstår till följd av direktivet Break

Du kan lösa felet manuellt genom att uppdatera scenariot (om det behövs) och köra det en gång.

Du kan också konfigurera scenariot så att det automatiskt bearbetar en ofullständig körning genom att köra scenariot igen. Så här konfigurerar du modulen för att bearbeta ofullständiga körningar:

1. Aktivera alternativet [!UICONTROL **Slutför körning automatiskt**] i Break-modulen.
1. I fältet **Antal försök** anger eller mappar du det maximala antalet försök som du vill att modulen ska göra om körningen

   Talet måste vara mellan 1 och 100.
1. Ange eller mappa antalet minuter mellan varje försök i fältet **Intervall mellan försök**.

När det här alternativet är aktiverat hämtas den ofullständiga körningen (efter den tid som anges i fältet [!UICONTROL Interval between attempts]) och körs med de ursprungliga indata. Detta upprepas tills körningen av modulen har slutförts utan fel eller tills det angivna antalet försök har uppnåtts.

>[!NOTE]
>
>Om det initiala försöket misslyckas, ökar intervallet mellan försöken exponentiellt varje annat försök.


När&quot;Automatiskt slutförd körning&quot; är aktiverat markeras scenariot som slutfört eftersom felhanterarens automatiska återförsök hanterar problemet automatiskt. I det här fallet får användarna inte något e-postmeddelande om den misslyckade körningen.

När&quot;Automatiskt slutförd körning&quot; är inaktiverad markeras körningen som&quot;Varning&quot;.

Det finns vissa undantag från körningar som lagras under Ofullständiga körningar, och med vissa feltyper går det inte att utföra en scenariokörning automatiskt igen.

Mer information finns i [Tillåt lagring av ofullständiga körningar](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) i artikeln [Panelen för scenarioinställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Mer information finns i [Avancerad felhantering i Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
