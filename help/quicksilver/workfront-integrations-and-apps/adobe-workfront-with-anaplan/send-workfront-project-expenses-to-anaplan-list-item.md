---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skicka [!DNL Adobe Workfront] utgifter till ett [!DNL Anaplan] listobjekt
description: Det här integreringsscenariot delar utgiftsrelaterad information från ett [!DNL Adobe Workfront] projekt med ett [!DNL Anaplan] budgetlistobjekt. Genom att dela den här informationen kan du bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som  [!DNL Anaplan] tillhandahåller.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] utgifter till ett [!DNL Anaplan]-listobjekt

Det här integreringsscenariot delar utgiftsrelaterade detaljer från ett [!DNL Adobe Workfront]-projekt med ett [!DNL Anaplan]-budgetlisteobjekt. Genom att dela den här informationen kan du bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

&#42;&#42;Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## [!DNL Workfront]-konfiguration förväntades

Du måste ha följande i [!DNL Workfront] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Workfront] med namnet *[!UICONTROL *[!DNL Anaplan] Integration]** som har systemadministratörsbehörighet.

  Mer information om hur du skapar en användare i [!DNL Workfront] finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ett **[!UICONTROL Campaign Brief]** anpassat formulär som är kopplat till projektobjektet för att lagra anpassade datavärden som du väljer att skicka till [!DNL Anaplan].

  Formuläret måste innehålla följande fält:

  | Fältnamn | Fälttyp |
  |---|---|
  | [!UICONTROL Last Transmission Date] | Datum |
  | [!UICONTROL Integration Notes] | Textfält för stycke |

  Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## [!DNL Anaplan]-konfiguration förväntades

Du måste ha följande i [!DNL Anaplan] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Anaplan] med namnet **[!UICONTROL [!DNL Workfront] Integration]** som har systemadministratörsbehörighet.
* Modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* Listan i modellen [!DNL Anaplan] som du vill hämta kampanjbudgetar för.
* En **[!UICONTROL Anaplan Actual Expense Import]**-fil som innehåller följande kolumner, i den här ordningen:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]

  Så här förbereder du filen [!UICONTROL [!DNL Anaplan] Actual Expense Import]:

   1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel].
   1. Spara filen i CSV-format.
   1. Överför filen till [!DNL Anaplan].

      Instruktioner finns i [!DNL Anaplan]-dokumentationen om hur du importerar data till moduler från en fil.

   1. Observera namnet som du gav filen. Det kommer att användas under distributionen av scenariomallen [!UICONTROL Fusion].

  Exempel på CSV-innehåll

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* En **[!UICONTROL [!DNL Anaplan] Planned Expense Import]**-fil som innehåller följande kolumner, i den här ordningen:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]

  Så här förbereder du filen [!UICONTROL [!DNL Anaplan] Planned Expense Import]:

   1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel]
   1. Spara filen i CSV-format
   1. Överför filen till Anaplan.

      Instruktioner finns i [!DNL Anaplan]-dokumentationen om hur du importerar data till moduler från en fil.

   1. Observera namnet som du gav filen. Det kommer att användas under distributionen av scenariomallen [!UICONTROL Fusion].

  Exempel på CSV-innehåll

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* En **[!UICONTROL Project Update Import]**-process förberedd för att köra import av data som levererats i en filöverföring.

>[!NOTE]
>
>Det finns separata importfiler för planerade och faktiska utgifter så att de kan rapporteras oberoende av planerat respektive gällande datum.

Instruktioner om dessa åtgärder finns i dokumentationen för [!DNL Anaplan].

## Distribuerar till [!DNL Fusion]

Utför följande steg för att distribuera det här integreringsscenariot till ditt [!DNL Fusion]-konto. Detta bör endast göras efter att den nödvändiga [!DNL Workfront]- och [!DNL Anaplan]-konfigurationen har slutförts.

1. Navigera till menyn [!UICONTROL Templates] i [!DNL Workfront Fusion] och klicka på mallen för **[!UICONTROL Send Workfront expenses updates to [!DNL Anaplan] list item]**-scenarier.
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
      <td>ID:t för arbetsytan från ditt [!DNL Anaplan]-konto som du vill använda för det här scenariot.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>ID:t för modellen från ditt [!DNL Anaplan]-konto och den valda arbetsytan som du vill använda för det här scenariot.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Namnet på listan från ditt [!DNL Anaplan]-konto och den valda arbetsytan och modellen som du vill använda för det här scenariot.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Actual Expense Import]</td> 
      <td> <p>Namnet på filen som ska ta emot faktiska utgiftsdata för projektet.</p> <p> (Exempel: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Planned Expense Import]</td> 
      <td> <p>Namnet på filen som ska ta emot projektplanerade utgiftsdata.</p> <p> (Exempel: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Namnet på den process som ska utföra importen av projektutgiftsdata.</p> <p>(Exempel: WF int - läs in projektutgifter)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Information om hur du konfigurerar filer och processer finns i installationsdokumentationen för [!DNL Anaplan].

1. Välj eller lägg till en [!DNL Anaplan]-anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med en [!DNL Anaplan]-anslutning när du uppmanas till det.
1. Välj eller lägg till en [!DNL Workfront]-anslutningsprofil.
1. Uppdatera alla återstående [!DNL Workfront] moduler med en [!DNL Workfront]-anslutning när du uppmanas till det.
1. Lägg till en ny datastruktur i modulen **[!UICONTROL Build Actual Expense CSV]** för att mappa projektattributen till CSV-kolumner.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. Lägg till en ny datastruktur i modulen **[!UICONTROL Build Planned Expense CSV]** för att mappa projektattributen till CSV-kolumner.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Andra rekommenderade scenariomallar

Den här scenariomallen kompletteras av följande mallar för utgiftsoptimeringsscenarier som också kan distribueras:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] faktiska timmars uppdateringar av ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Ytterligare scenarier för länkning av budgetbegäranden:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till ett [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för länkning av kampanjförfrågningar:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en  [!DNL Adobe Workfront] kampanjbegäran]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en  [!DNL Adobe Workfront] kampanjbegäran eller ett kampanjprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
