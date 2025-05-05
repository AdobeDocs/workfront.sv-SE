---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skicka  [!DNL Adobe Workfront] uppdateringar av faktiska timmar till ett  [!DNL Anaplan] listobjekt
description: Det här integreringsscenariot delar information om faktiska timmar som samlats in i ett [!DNL Adobe Workfront] projekt med ett [!DNL Anaplan] budgetlisteobjekt. Genom att dela den här informationen kan du bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som  [!DNL Anaplan] tillhandahåller.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] uppdateringar av faktiska timmar till ett [!DNL Anaplan]-listobjekt

Det här integreringsscenariot delar faktiska timuppgifter som samlats in i ett [!DNL Adobe Workfront]-projekt med ett [!DNL Anaplan]-budgetlisteobjekt. Genom att dela den här informationen kan du bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.

Den här scenariomallen innehåller en lista med timmar summerade efter projekt, dag och roll som registrerats i aktiva projekt under de senaste tre månaderna.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

&#42;&#42;Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## [!DNL Workfront]-konfiguration förväntades

Du måste ha följande i [!DNL Workfront] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Workfront] med namnet **[!UICONTROL Anaplan Integration]** som har systemadministratörsbehörighet.

  Mer information om hur du skapar en användare i [!DNL Workfront] finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## [!DNL Anaplan]-konfiguration förväntades

Du måste ha följande i [!DNL Anaplan] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Anaplan] med namnet **[!UICONTROL [!DNL Workfront] Integration]** som har systemadministratörsbehörighet.
* Modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* Listan i modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* En fil i [!DNL Anaplan] med namnet **[!UICONTROL Anaplan Actual Hours Import]** som innehåller följande kolumner, i den här ordningen:

   1. [!UICONTROL Workfront Project GUID]

   2. [!UICONTROL Hours]

   3. [!UICONTROL Hours Estimated Cost]

   4. [!UICONTROL Entry Date]

   5. [!UICONTROL Role Name]

   6. [!UICONTROL Campaign Name]

   7. [!UICONTROL [!DNL Anaplan] List Item ID]

  Så här förbereder du den [!DNL Anaplan] faktiska utgiftsrapportfilen:

   1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel]
   1. Spara filen i CSV-format
   1. Överför filen till [!DNL Anaplan].

      Instruktioner finns i [!DNL Anaplan]-dokumentationen om hur du importerar data till moduler från en fil.

   1. Observera namnet som du gav filen. Det kommer att användas under distributionen av scenariomallen [!UICONTROL Fusion].

  Exempel på CSV-innehåll

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* En **[!UICONTROL Project Actual Hours Import]**-process förberedd för att köra import av data som levererats i en filöverföring.

Instruktioner om dessa åtgärder finns i dokumentationen för [!DNL Anaplan].

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera det här integreringsscenariot till ditt [!DNL Fusion]-konto. Detta bör endast göras efter att den nödvändiga [!DNL Workfront]- och [!DNL Anaplan]-konfigurationen har slutförts.

1. Navigera till menyn [!UICONTROL Templates] i [!DNL Workfront Fusion] och klicka på mallen för **[!UICONTROL Send Workfront actual hours updates to [!DNL Anaplan] list item]**-scenarier.
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
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Namnet på listan från ditt [!DNL Anaplan]-konto och den valda arbetsytan och modellen.</td> 
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
      <td>Underdomänen för ditt [!DNL Workfront]-konto. Detta används för att skapa en länk tillbaka till ditt [!DNL Workfront]-projekt i en anteckning som kan genereras.</td> 
     </tr> 
    </tbody> 
   </table>

   Information om hur du konfigurerar filer och processer finns i installationsdokumentationen för [!DNL Anaplan].

1. Välj eller lägg till en [!DNL Anaplan]-anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med en [!DNL Anaplan]-anslutning när du uppmanas till det.
1. Välj eller lägg till en [!DNL Workfront]-anslutningsprofil.
1. Uppdatera alla återstående [!DNL Workfront] moduler med en [!DNL Workfront]-anslutning när du uppmanas till det.

## Andra rekommenderade scenariomallar

Den här scenariomallen kompletteras av följande mallar för utgiftsoptimeringsscenarier som också kan distribueras:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Ytterligare scenarier för länkning av budgetbegäranden:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till ett [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för länkning av kampanjförfrågningar:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en  [!DNL Adobe Workfront] kampanjbegäran]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en  [!DNL Adobe Workfront] kampanjbegäran eller ett kampanjprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
