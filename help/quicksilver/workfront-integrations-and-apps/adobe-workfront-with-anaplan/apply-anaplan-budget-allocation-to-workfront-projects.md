---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Använd en [!DNL Anaplan] budgetallokering för ett [!DNL Adobe Workfront] projekt
description: Det här integreringsscenariot synkroniserar alla budgetallokeringar som har gjorts i  [!DNL Anaplan] tillbaka till  [!DNL Workfront]. Scenariot hämtar alla länkade kampanjbudgetposter och skickar sedan det budgade värdet till det länkade Workfront-projektet om budgetvärdet har ändrats.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Använd en [!DNL Anaplan]-budgetallokering för ett [!DNL Adobe Workfront]-projekt

Det här integreringsscenariot synkroniserar alla budgetallokeringar som har gjorts i [!DNL Anaplan] tillbaka till [!DNL Workfront]. Scenariot hämtar alla länkade kampanjbudgetartiklar och skickar sedan det budgeterade värdet till det länkade [!DNL Workfront]-projektet om budgetvärdet har ändrats.

>[!IMPORTANT]
>
>&quot;Campaign&quot; i den här artikeln avser det användningsfall för marknadsföringskampanj som det här scenariot representerar och är inte på något sätt kopplat till [!DNL Workfront Fusion] Adobe Campaign-anslutningen eller till det nyligen borttagna [!UICONTROL Campaign]-objektet i [!DNL Workfront].

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

&#42;&#42;Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## [!DNL Workfront]-konfiguration förväntades

Du måste ha följande i [!DNL Workfront] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Workfront] med namnet **Anaplan-integrering** som har systemadministratörsbehörighet.

  Mer information om hur du skapar en användare i [!DNL Workfront] finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## [!DNL Anaplan]-konfiguration förväntades

Du måste ha följande i [!DNL Anaplan] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Anaplan] med namnet **[!DNL Workfront]Integration** som har systemadministratörsbehörighet.
* Modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* Listan i modellen [!DNL Anaplan] som samlar in kampanjbudgetar.

  Listans modul måste ha stöd för följande attribut:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Estimated Revenue]
   * [!UICONTROL Brand]

  Den här listan och modulen måste lagra ytterligare information som är nödvändig för den normala funktionen i [!DNL Anaplan], inklusive möjligheten att ställa in en budget och meddela att budgetlistobjektet är klart att synkroniseras tillbaka till [!DNL Workfront].

* En vy i [!DNL Anaplan] med namnet **[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]**.

  Den här vyn måste innehålla följande kolumner i den här ordningen:

   1. [!UICONTROL Item Name]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Campaign Name]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Estimated Revenue]

   6. [!UICONTROL Brand]

  Vyn ska filtreras så att objekt som har en [!UICONTROL [!DNL Workfront] Project GUID] och en indikator på att budgetallokeringar ska överföras till [!DNL Workfront] visas.

Instruktioner om dessa åtgärder finns i dokumentationen för [!DNL Anaplan].

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera det här integreringsscenariot till ditt [!DNL Fusion]-konto. Detta bör endast göras efter att den nödvändiga [!DNL Workfront]- och [!DNL Anaplan]-konfigurationen har slutförts.

1. Navigera till menyn [!UICONTROL Templates] i [!DNL Workfront Fusion] och klicka på mallen för **[!UICONTROL Apply [!DNL Anaplan] budget allocations to Workfront projects]**-scenarier.
1. Ersätt variabelvärdena för följande [!DNL Anaplan]-variabler:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Variabelnamn</th> 
      <th>Ersätt värde med</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace-id]</td> 
      <td>ID för en arbetsyta från ditt [!DNL Anaplan]-konto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>ID:t för en modell från ditt [!DNL Anaplan]-konto och den valda arbetsytan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modulnamn]</td> 
      <td>Namnet på modulen som beskriver kampanjattributen i den valda [!DNL Anaplan]-listan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Namnet på listan från ditt [!DNL Anaplan]-konto och den valda arbetsytan och modellen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Visningsnamn]</td> 
      <td> <p>Namnet på den vy som innehåller kampanjbudgetar som är klara att överföras till [!DNL Workfront].</p> <p>(Exempel: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Information om hur du konfigurerar filer och processer finns i installationsdokumentationen för [!DNL Anaplan].

1. Välj eller lägg till en [!DNL Anaplan]-anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med en [!DNL Anaplan]-anslutning när du uppmanas till det.
1. På **[!UICONTROL Convert CSV to JSON Object module]** lägger du till en ny datastruktur för att mappa CSV-kolumnerna till ett användbart JSON-objekt.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. När du uppmanas till det väljer du den här datastrukturen för andra moduler i den här scenariodistributionen.
1. Markera eller lägg till en [!DNL Workfront]-anslutningsprofil i modulen **[!UICONTROL Check Linked Project]**.
1. Uppdatera alla återstående [!DNL Workfront] moduler med en [!DNL Workfront]-anslutning när du uppmanas till det.

## Andra rekommenderade scenariomallar

Om du vill slutföra arbetsflödet som den här mallen representerar måste du även distribuera följande extra mall:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Ytterligare scenarier för utgiftsoptimering är:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] faktiska timmars uppdateringar av ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
