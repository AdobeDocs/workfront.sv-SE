---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skicka [!DNL Adobe Workfront] projektuppdateringar till [!DNL Anaplan] listobjekt
description: Det här integreringsscenariot delar status, status och viktig schemainformation från en [!DNL Adobe Workfront] projekt med [!DNL Anaplan] budgetlisteartikel. Genom att dela den här informationen kan ni bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] projektuppdateringar till [!DNL Anaplan] listobjekt

Det här integreringsscenariot delar status, status och viktig schemainformation från en [!DNL Adobe Workfront] projekt med [!DNL Anaplan] budgetlisteartikel. Genom att dela den här informationen kan ni bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
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

* En användarprofil i [!DNL Workfront] namngiven **[!UICONTROL [!DNL Anaplan] Integration]**, som har systemadministratörsbehörighet.

   Mer information om hur du skapar en användare i [!DNL Workfront], se [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Campaign Brief]** anpassat formulär kopplat till projektobjektet för att lagra anpassade datavärden som du väljer att skicka till Anaplan.

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

   Mer information om hur du skapar anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Förväntat [!DNL Anaplan] Konfiguration

Du måste ha följande i [!DNL Anaplan] om du vill använda det här scenariot:

* En användarprofil i [!DNL Anaplan] namngiven **[!UICONTROL [!DNL Workfront] Integration]**, som har systemadministratörsbehörighet.
* The [!DNL Anaplan] Modell som du vill använda för det här scenariot.
* Listan i [!DNL Anaplan] Modell som du vill använda för det här scenariot.
* A **[!UICONTROL Project Update Import]** som innehåller följande kolumner, i den här ordningen:

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

Förbered [!UICONTROL [!DNL Anaplan] Planned Expense Import] fil:

1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel]
1. Spara filen i CSV-format
1. Överför filen till Anaplan.

   Instruktioner finns i [!DNL Anaplan] dokumentation om hur du importerar data till moduler från en fil.

1. Anteckna det namn du gett filen. den kommer att användas under distributionen av [!UICONTROL Fusion] scenariomall.

Exempel på CSV-innehåll

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL Campaign Overview]

2. [!UICONTROL Key Message]

3. [!UICONTROL In Market Start Date]

4. [!UICONTROL In Market End Date]

5. [!UICONTROL Target Audience]

Inkludera även andra fält som du vill ange i mappningen.

* A **[!UICONTROL Project Update Import]** process som förbereds för import av data som levereras i en filöverföring.

Instruktioner om dessa åtgärder finns i [!DNL Anaplan] dokumentation.

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera det här integreringsscenariot till ditt Fusion-konto. Detta bör endast göras efter att du fyllt i [!DNL Workfront] och [!DNL Anaplan] konfiguration.

1. Navigera till [!UICONTROL Templates] menyn i [!DNL Workfront Fusion] och klicka på **[!UICONTROL Send Workfront project updates to [!DNL Anaplan] list item]** scenariomall.
1. Ersätt variabelvärdena för följande [!DNL Anaplan] variabler:

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
      <td role="rowheader">[!UICONTROL File Name: Project Update Import]</td> 
      <td>Namnet på filen som ska ta emot projektuppdateringsdata.<p>(Exempel: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Namnet på den process som ska utföra importen av projektdata.</p> <p>(Exempel: WF int - uppdatera kampanjinformation)</p> </td> 
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

   Filtret är konfigurerat att hämta in alla ofullständiga länkade projekt och de projekt som har slutförts under de senaste 29 minuterna. Om du ändrar frekvensen för [!DNL Fusion] scenario du vill uppdatera det här värdet när scenariomallen har distribuerats.

1. På **[!UICONTROL Build Projects Update CSV]** lägger du till en ny datastruktur för att mappa projektattributen till CSV-kolumner.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Uppdatera alla återstående [!DNL Workfront] moduler med [!DNL Workfront] anslutning när du uppmanas till detta.

## Andra rekommenderade scenariomallar

Den här scenariomallen kompletteras av följande mallar för utgiftsoptimeringsscenarier som också kan distribueras:

* [[!UICONTROL Send [!DNL Adobe Workfront] faktiskt antal timmars uppdateringar av en [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Ytterligare scenarier för länkning av budgetbegäranden:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för länkning av kampanjförfrågningar:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] kampanjförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] kampanjförfrågan eller kampanjprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
