---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Skapa och jämföra planscenarier i scenarioplaneraren
description: När ni planerar företagets långsiktiga strategi finns det mycket information som ni kanske inte har eller tänker på i början. Det tar tid och experimenterande att komma fram till en slutlig strategi som era intressenter kan acceptera. Genom att utföra en konsekvensanalys för att skapa flera scenarier för din plan kan du förutse och utvärdera potentiella omständigheter på ett korrekt sätt och i slutändan utveckla den bästa möjliga planen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Skapa och jämföra planscenarier i [!DNL Scenario Planner]

<!--Audited: 07/2024-->

När ni planerar företagets långsiktiga strategi finns det mycket information som ni kanske inte har eller tänker på i början. Det tar tid och experimenterande att komma fram till en slutlig strategi som era intressenter kan acceptera. Genom att utföra en konsekvensanalys för att skapa flera scenarier för din plan kan du förutse och utvärdera potentiella omständigheter på ett korrekt sätt och i slutändan utveckla den bästa möjliga planen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>ANMÄRKNING</b></p>
<p>Kontakta Workfront om du har ett annat Workfront-paket.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td> <p>[!UICONTROL Light] eller högre</p> 
   <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
    <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om åtkomst till scenarioplanen finns i [Åtkomst krävs för att använda  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Skapa scenarier

Ett scenario är en kopia av en plan. Du kan skapa så många scenarier du behöver. Vi rekommenderar dock att du håller antalet scenarier så lågt som möjligt så att du enkelt kan jämföra dem.

{{step1-to-scenario-planner}}

1. Skapa en plan eller klicka på namnet på en befintlig plan.

   Mer information om hur du skapar planer finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Den första plan du skapar sparas automatiskt som [!UICONTROL Initial scenario].

1. Klicka på nedåtpilen bredvid ett befintligt scenario och klicka sedan på ikonen **[!UICONTROL Copy]** .

   ![Kopiera scenario](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Detta skapar ett nytt scenario med samma information som det kopierade scenariot. Det får automatiskt namnet [!UICONTROL Scenario 2] om det är det andra scenariot i din plan, [!UICONTROL Scenario 3] om det är det tredje och så vidare. Du kan inte byta namn på dina scenarier. Det finns ingen gräns för hur många kopior du kan göra.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Uppdatera ditt nya scenario på något av följande sätt:

   * Skapa, uppdatera eller ta bort initiativ

     >[!TIP]
     >
     >När du tar bort ett initiativ i ett scenario tas det bara bort från det valda scenariot, inte från alla scenarier.

     Mer information om hur du skapar initiativ finns i [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Uppdatera prioriteringarna i era initiativ
   * Justera personer eller budgetinformation
   * Granska och justera initialkonflikter i ditt scenario

     Mer information om hur du löser konflikter finns i [Lös initialkonflikter i  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna.

## Jämför scenarier

När du har skapat dina scenarier kan du jämföra dem för att hitta det bästa för din organisation.

1. Gå till planen som du vill jämföra scenarier för.
1. Klicka på **[!UICONTROL Compare scenarios]**. Scenariojämförelsesidan visas.

   Alla befintliga scenarier för planen visas sida vid sida i kortformat. Det inledande scenariot visas alltid först och är statiskt.

   ![Senariokort](assets/scenario-cards-overlapping-350x166.png)

1. (Valfritt) Bläddra till höger om du vill visa alla scenariokort.

   Följande information visas på ett scenariokort:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Namn på scenariot</td> 
      <td> <p>Ett namn som genererats automatiskt av Workfront och som inte kan redigeras. Till exempel [!UICONTROL Initial scenario], [!UICONTROL Scenario 2] och så vidare. </p> </td> 
     </tr> 
     <tr> 
      <td>Scenariobeskrivning</td> 
      <td>En manuell inmatning där du kan beskriva detaljerad information om scenariot. </td> 
     </tr> 
     <tr> 
      <td>Tillgängliga jobbroller</td> 
      <td>Antalet jobbroller som är tillgängliga från planens budget under planens varaktighet. </td> 
     </tr> 
     <tr> 
      <td>Obligatoriska jobbroller</td> 
      <td>Antalet jobbroller som krävs, baserat på dina initiativ. </td> 
     </tr> 
     <tr> 
      <td>Budget</td> 
      <td>Den totala budgeten som har definierats för planen i det här scenariot. Budgetinformation om planer finns i Översikt över <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Planer i [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Kostnader</td> 
      <td>De kostnader som är förknippade med satsningarna på scenariot. Mer information om kostnader finns i <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Översikt över initiativ i [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Användning</td> 
      <td>Procentandelen [!UICONTROL Budget Utilization] för planen i det här scenariot. Mer information om procentandelen [!UICONTROL Budget Utilization] finns i <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Planöversikt i [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Nettovärde</td> 
      <td>Planens [!UICONTROL Net Value] i det här scenariot. Mer information om [!UICONTROL Net Value] för en plan finns i <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Planöversikt i [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Initiativ</td> 
      <td>Antalet initiativ för planen i det här scenariot.</td> 
     </tr> 
     <tr> 
      <td>Konflikt</td> 
      <td>Antalet initiativ som visar någon typ av konflikt i planen för det här scenariot. Mer information om initieringskonflikter finns i <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Lös initialkonflikter i [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >När informationen skiljer sig mellan det inledande scenariot och ytterligare scenarier visas en upp- eller nedpil bredvid värdet som ändrats för att ange en ökning eller minskning av det värdet, jämfört med det ursprungliga scenariot.
   >
   >
   >![Pilar på scenariokort](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Till exempel budgeten, antalet jobbroller och antalet initiativ kan ändras från ett scenario till ett annat.

1. Klicka på namnet på ett scenario för att komma åt det och ändra det.

   Mer information finns i avsnittet [Skapa scenarier](#create-scenarios) i den här artikeln.

1. Klicka på **[!UICONTROL Add description]** om du vill lägga till en beskrivning av scenariot

   eller

   Klicka på beskrivningsfältet för att uppdatera det och klicka sedan var som helst på skärmen för att spara ändringarna.

1. (Valfritt) Klicka på **[!UICONTROL More]**-menyn ![Mer-ikon](assets/more-icon.png) för att **[!UICONTROL Copy]** eller **[!UICONTROL Delete]** scenariot.

   ![Kopiera eller ta bort scenario](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   När du kopierar ett scenario visas det automatiskt på kortsidan och får ett nytt namn enligt följande mönster: [!UICONTROL Scenario] `<next number in order>`.

1. (Villkorligt) Om du klickade på **[!UICONTROL Delete]** klickar du på **[!UICONTROL Yes, delete it]** för att bekräfta.

   Borttagna scenarier kan inte återställas.

   Mer information om att ta bort scenarier finns i [Ta bort planer i  [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara dina scenarier och din plan.
