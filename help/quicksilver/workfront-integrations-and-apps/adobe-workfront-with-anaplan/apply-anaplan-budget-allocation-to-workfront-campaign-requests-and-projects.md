---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Använd en [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] kampanjförfrågan eller kampanjprojekt
description: Det här integreringsscenariot synkroniserar alla budgetallokeringar som har gjorts i [!DNL Anaplan] tillbaka till [!DNL Workfront]. Scenariot hämtar alla länkade kampanjbudgetposter och skickar sedan det budgade värdet till det länkade Workfront-projektet om budgetvärdet har ändrats.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Använd en [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] kampanjförfrågan eller kampanjprojekt

Det här integreringsscenariot synkroniserar alla budgetallokeringar som har gjorts i [!DNL Anaplan] tillbaka till [!DNL Workfront]. Scenariot hämtar alla länkade kampanjbudgetartiklar och skickar sedan budgetvärdet till den länkade [!DNL Workfront] projekt om budgetvärdet har ändrats.

>[!IMPORTANT]
>
>&quot;Campaign&quot; i den här artikeln avser det användningsfall för marknadsföringskampanj som det här scenariot representerar och inte på något sätt är kopplat till [!DNL Workfront Fusion] Adobe Campaign-anslutning eller till den nyligen borttagna [!UICONTROL Campaign] objekt i [!DNL Workfront].


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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

&#42;&#42;För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## Förväntat [!DNL Workfront] Konfiguration

Du måste ha följande i [!DNL Workfront] om du vill använda det här scenariot:

* En användarprofil i [!DNL Workfront] namngiven **[!DNL Anaplan Integration]**, som har systemadministratörsbehörighet.

   Mer information om hur du skapar en användare i [!DNL Workfront], se [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Förväntat [!DNL Anaplan] Konfiguration

Du måste ha följande i [!DNL Anaplan] om du vill använda det här scenariot:

* En användarprofil i [!DNL Anaplan] namngiven **[!UICONTROL [!DNL Workfront] Integration]**, som har systemadministratörsbehörighet.
* The [!DNL Anaplan] Modell som du vill använda för det här scenariot.
* Listan i [!DNL Anaplan] Modell som fångar kampanjbudgetar.

   Listans modul måste ha stöd för följande attribut:

   * [!UICONTROL [!DNL Workfront] Request GUID]
   * [!UICONTROL [!DNL Workfront] Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Estimated Revenue]
   * [!UICONTROL Brand]

   Den här listan och modulen måste lagra ytterligare information som är nödvändig för den normala funktionen hos [!DNL Anaplan], inklusive möjligheten att ställa in en budget och meddela att budgetlisteposten är klar att synkroniseras tillbaka till [!DNL Workfront].

* En vy i [!DNL Anaplan] anropad **[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]**.

   Den här vyn måste innehålla följande kolumner i den här ordningen:

   1. [!UICONTROL Item Name]

   2. [!UICONTROL [!DNL Workfront] Request GUID]

   3. [!UICONTROL [!DNL Workfront] Project GUID]

   4. [!UICONTROL Campaign Name]

   5. [!UICONTROL Budget]

   6. [!UICONTROL Estimated Revenue]

   7. [!UICONTROL Brand]
   Vyn ska filtreras så att objekt som har en [!UICONTROL [!DNL Workfront] Project GUID] och en indikator på att budgetanslag ska överföras till Workfront.

Instruktioner om dessa åtgärder finns i [!DNL Anaplan] dokumentation.

## Distribuera till Workfront Fusion

Utför följande steg för att distribuera det här integreringsscenariot till ditt Fusion-konto. Detta bör endast göras efter att du fyllt i [!DNL Workfront] och [!DNL Anaplan] konfiguration.

1. Navigera till [!UICONTROL Templates] menyn i [!DNL Workfront Fusion] och klicka på **[!UICONTROL Apply [!DNL Anaplan] budget allocations to Workfront campaign requests & projects]** scenariomall.
1. Ersätt variabelvärdena för följande [!DNL Anaplan] variabler:

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Arbetsyte-ID]</td> 
      <td>ID:t för en arbetsyta från din [!DNL Anaplan] konto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>ID:t för en modell från din [!DNL Anaplan] och den valda arbetsytan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Namnet på listan från din [!DNL Anaplan] och den valda arbetsytan och modellen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Visningsnamn]</td> 
      <td> <p>Namnet på vyn som innehåller kampanjbudgetar som är klara att överföras till [!DNL Workfront].</p> <p>(Exempel: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Information om hur du konfigurerar filer och processer finns i [!DNL Anaplan] installationsdokumentation.

1. Markera eller lägga till en [!DNL Anaplan] anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med [!DNL Anaplan] anslutning när du uppmanas till detta.
1. På **[!UICONTROL Convert CSV to JSON Object]** lägger du till en ny datastruktur för att mappa CSV-kolumnerna till ett användbart JSON-objekt.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. När du uppmanas till det väljer du den här datastrukturen för andra moduler i den här scenariodistributionen.
1. På **[!UICONTROL Check Linked Project]** modul, markera eller lägga till en [!DNL Workfront] anslutningsprofil.
1. Uppdatera alla återstående [!DNL Workfront] moduler med [!DNL Workfront] anslutning när du uppmanas till detta.

## Andra rekommenderade scenariomallar

Om du vill slutföra arbetsflödet som den här mallen representerar måste du även distribuera följande extra mall:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] kampanjförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Ytterligare scenarier för utgiftsoptimering är:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] faktiskt antal timmars uppdateringar av en [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
