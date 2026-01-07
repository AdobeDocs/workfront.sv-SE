---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skicka  [!DNL Adobe Workfront] projektuppdateringar till ett  [!DNL Anaplan] listobjekt
description: Det här integrationsscenariot delar förlopp, status och viktig schemainformation från ett [!DNL Adobe Workfront] projekt med ett [!DNL Anaplan] budgetlistobjekt. Genom att dela den här informationen kan du bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som  [!DNL Anaplan] tillhandahåller.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] projektuppdateringar till ett [!DNL Anaplan]-listobjekt

Det här integrationsscenariot delar förlopp, status och nyckelschemainformation från ett [!DNL Adobe Workfront]-projekt med ett [!DNL Anaplan]-budgetlistobjekt. Genom att dela den här informationen kan du bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.

>[!IMPORTANT]
>
>&quot;Campaign&quot; i den här artikeln avser det användningsfall för marknadsföringskampanj som det här scenariot representerar och är inte på något sätt kopplat till [!DNL Workfront Fusion] Adobe Campaign-anslutningen eller till det nyligen borttagna [!UICONTROL Campaign]-objektet i [!DNL Workfront].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla Adobe Workfront Workflow-paket och alla Adobe Workfront Automation and Integration-paket</p><p>Workfront Ultimate</p><p>Workfront Prime- och Select-paket med ytterligare köp av Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-licenser</td> 
   <td> <p>Standard</p><p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-licens</td> 
   <td>
   <p>Operationsbaserad: Ingen Workfront Fusion-licens krävs</p>
   <p>Kopplingsbaserad (äldre): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Om ni har ett Select- eller Prime Workfront-paket som inte innehåller Workfront Automation and Integration måste ni köpa Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om Adobe Workfront Fusion-licenser finns i [Adobe Workfront Fusion-licenser](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## [!DNL Workfront]-konfiguration förväntades

Du måste ha följande i [!DNL Workfront] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Workfront] med namnet **[!UICONTROL [!DNL Anaplan] Integration]** som har systemadministratörsbehörighet.

  Mer information om hur du skapar en användare i [!DNL Workfront] finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ett anpassat **[!UICONTROL Campaign Brief]**-formulär som är kopplat till projektobjektet för att lagra anpassade datavärden som du väljer att skicka till Anaplan.

  Följande fält är exempel på fält som kan inkluderas i det anpassade formuläret för att underlätta datamappning till Anaplan, men som inte krävs för det här integreringsscenariot:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Fältnamn</th> 
     <th>Fälttyp</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Inkludera alternativ som passar era processer.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## [!DNL Anaplan]-konfiguration förväntades

Du måste ha följande i [!DNL Anaplan] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Anaplan] med namnet **[!UICONTROL [!DNL Workfront] Integration]** som har systemadministratörsbehörighet.
* Modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* Listan i modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* En **[!UICONTROL Project Update Import]**-fil som innehåller följande kolumner, i den här ordningen:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] Project GUID]

3. [!UICONTROL Campaign Name]

4. [!UICONTROL Percent Complete]

5. [!UICONTROL Planned Start Date]

6. [!UICONTROL Planned Completion Date]

7. [!UICONTROL Planned Hours]

8. [!UICONTROL Planned Cost]

9. [!UICONTROL Planned Expense Cost]

10. [!UICONTROL Actual Labor Cost]

11. [!UICONTROL Planned Labor Cost]

12. [!UICONTROL Status]

Så här förbereder du filen [!UICONTROL [!DNL Anaplan] Planned Expense Import]:

1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel]
1. Spara filen i CSV-format
1. Överför filen till Anaplan.

   Instruktioner finns i [!DNL Anaplan]-dokumentationen om hur du importerar data till moduler från en fil.

1. Observera namnet som du gav filen. Det kommer att användas under distributionen av scenariomallen [!UICONTROL Fusion].

Exempel på CSV-innehåll

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Valfria kolumner kan vara:

1. [!UICONTROL Campaign Overview]

2. [!UICONTROL Key Message]

3. [!UICONTROL In Market Start Date]

4. [!UICONTROL In Market End Date]

5. [!UICONTROL Target Audience]

Inkludera även andra fält som du vill ange i mappningen.

* En **[!UICONTROL Project Update Import]**-process förberedd för att köra import av data som levererats i en filöverföring.

Instruktioner om dessa åtgärder finns i dokumentationen för [!DNL Anaplan].

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera det här integreringsscenariot till ditt Fusion-konto. Detta bör endast göras efter att den nödvändiga [!DNL Workfront]- och [!DNL Anaplan]-konfigurationen har slutförts.

1. Navigera till menyn [!UICONTROL Templates] i [!DNL Workfront Fusion] och klicka på mallen för **[!UICONTROL Send Workfront project updates to [!DNL Anaplan] list item]**-scenarier.
1. Ersätt variabelvärdena för följande [!DNL Anaplan]-variabler:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">[!UICONTROL File Name: Project Update Import]</td> 
      <td>Namnet på filen som ska ta emot projektuppdateringsdata.<p>(Exempel: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Namnet på den process som ska utföra importen av projektdata.</p> <p>(Exempel: WF int - Uppdatera kampanjinformation)</p> </td> 
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

   Filtret är konfigurerat att hämta in alla ofullständiga länkade projekt och de projekt som har slutförts under de senaste 29 minuterna. Om du ändrar frekvensen för scenariot [!DNL Fusion] vill du uppdatera det här värdet när scenariomallen har distribuerats.

1. Lägg till en ny datastruktur i modulen **[!UICONTROL Build Projects Update CSV]** för att mappa projektattributen till CSV-kolumner.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Uppdatera alla återstående [!DNL Workfront] moduler med en [!DNL Workfront]-anslutning när du uppmanas till det.

## Andra rekommenderade scenariomallar

Den här scenariomallen kompletteras av följande mallar för utgiftsoptimeringsscenarier som också kan distribueras:

* [[!UICONTROL Send [!DNL Adobe Workfront] faktiska timmars uppdateringar av ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Ytterligare scenarier för länkning av budgetbegäranden:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till ett [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för länkning av kampanjförfrågningar:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en  [!DNL Adobe Workfront] kampanjbegäran]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en  [!DNL Adobe Workfront] kampanjbegäran eller ett kampanjprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
