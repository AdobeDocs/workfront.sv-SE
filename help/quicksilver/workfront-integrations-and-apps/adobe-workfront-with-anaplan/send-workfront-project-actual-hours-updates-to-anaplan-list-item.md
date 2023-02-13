---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skicka [!DNL Adobe Workfront] faktiskt antal timmars uppdateringar av en [!DNL Anaplan] listobjekt
description: Det här integreringsscenariot delar information om faktiska timmar som fångats på en [!DNL Adobe Workfront] projekt med [!DNL Anaplan] budgetlisteartikel. Genom att dela den här informationen kan ni bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] faktiskt antal timmars uppdateringar av en [!DNL Anaplan] listobjekt

Det här integreringsscenariot delar information om faktiska timmar som fångats på en [!DNL Adobe Workfront] projekt med [!DNL Anaplan] budgetlisteartikel. Genom att dela den här informationen kan ni bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.

Den här scenariomallen innehåller en lista med timmar summerade efter projekt, dag och roll som registrerats i aktiva projekt under de senaste tre månaderna.

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

* En användarprofil i [!DNL Workfront] namngiven **[!UICONTROL Anaplan Integration]**, som har systemadministratörsbehörighet.

   Mer information om hur du skapar en användare i [!DNL Workfront], se [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Förväntat [!DNL Anaplan] Konfiguration

Du måste ha följande i [!DNL Anaplan] om du vill använda det här scenariot:

* En användarprofil i [!DNL Anaplan] namngiven **[!UICONTROL [!DNL Workfront ] Integration]**, som har systemadministratörsbehörighet.
* The [!DNL Anaplan] Modell som du vill använda för det här scenariot.
* Listan i [!DNL Anaplan] Modell som du vill använda för det här scenariot.
* En fil i [!DNL Anaplan] namngiven **[!UICONTROL Anaplan Actual Hours Import]** som innehåller följande kolumner, i den här ordningen:

   1. [!UICONTROL Workfront Project GUID]

   2. [!UICONTROL Hours]

   3. [!UICONTROL Hours Estimated Cost]

   4. [!UICONTROL Entry Date]

   5. [!UICONTROL Role Name]

   6. [!UICONTROL Campaign Name]

   7. [!UICONTROL [!DNL Anaplan] List Item ID]
   Förbered [!DNL Anaplan] Faktisk utgiftsrapportfil:

   1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel]
   1. Spara filen i CSV-format
   1. Överför filen till [!DNL Anaplan].

      Instruktioner finns i [!DNL Anaplan] dokumentation om hur du importerar data till moduler från en fil.

   1. Anteckna det namn du gett filen. den kommer att användas under distributionen av [!UICONTROL Fusion] scenariomall.

   Exempel på CSV-innehåll

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL Project Actual Hours Import]** process som förbereds för import av data som levereras i en filöverföring.

Instruktioner om dessa åtgärder finns i [!DNL Anaplan] dokumentation.

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera integreringsscenariot till din [!DNL Fusion] konto. Detta bör endast göras efter att du fyllt i [!DNL Workfront] och [!DNL Anaplan] konfiguration.

1. Navigera till [!UICONTROL Templates] menyn i [!DNL Workfront Fusion] och klicka på **[!UICONTROL Send Workfront actual hours updates to [!DNL Anaplan] list item]** scenariomall.
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
      <td role="rowheader">[!UICONTROL File Name: Actual Hours Import]</td> 
      <td> <p>Namnet på filen som ska ta emot faktiska timdata för projektet.</p> <p> (Exempel: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Actual Hours Import]</td> 
      <td> <p>Namnet på den process som ska utföra importen av projekttimdata.</p> <p>(Exempel: WF int - läs in projekttimmar efter roll)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Underdomän]</td> 
      <td>Underdomänen till din [!DNL Workfront] konto. Detta används för att skapa en länk tillbaka till [!DNL Workfront] projektet i en anteckning som kan genereras.</td> 
     </tr> 
    </tbody> 
   </table>

   Information om hur du konfigurerar filer och processer finns i [!DNL Anaplan] installationsdokumentation.

1. Markera eller lägga till en [!DNL Anaplan] anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med [!DNL Anaplan] anslutning när du uppmanas till detta.
1. Markera eller lägga till en [!DNL Workfront] anslutningsprofil.
1. Uppdatera alla återstående [!DNL Workfront] moduler med [!DNL Workfront] anslutning när du uppmanas till detta.

## Andra rekommenderade scenariomallar

Den här scenariomallen kompletteras av följande mallar för utgiftsoptimeringsscenarier som också kan distribueras:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Ytterligare scenarier för länkning av budgetbegäranden:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för länkning av kampanjförfrågningar:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] kampanjförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] kampanjförfrågan eller kampanjprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
