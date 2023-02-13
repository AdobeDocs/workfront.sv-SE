---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skicka [!DNL Adobe Workfront] utgifter för [!DNL Anaplan] listobjekt
description: Det här integreringsscenariot delar utgiftsrelaterad information från en [!DNL Adobe Workfront] projekt med [!DNL Anaplan] budgetlisteartikel. Genom att dela den här informationen kan ni bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] utgifter för [!DNL Anaplan] listobjekt

Det här integreringsscenariot delar utgiftsrelaterad information från en [!DNL Adobe Workfront] projekt med [!DNL Anaplan] budgetlisteartikel. Genom att dela den här informationen kan ni bättre utnyttja utgiftsoptimeringen och den ekonomiska analysen som [!DNL Anaplan] tillhandahåller.

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

* En användarprofil i [!DNL Workfront] namngiven *[!UICONTROL *[!DNL Anaplan] Integration]**, som har systemadministratörsbehörighet.

   Mer information om hur du skapar en användare i [!DNL Workfront], se [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Campaign Brief]** anpassat formulär kopplat till projektobjektet för att lagra anpassade datavärden som du väljer att skicka till [!DNL Anaplan].

   Formuläret måste innehålla följande fält:

   | Fältnamn | Fälttyp |
   |---|---|
   | [!UICONTROL Last Transmission Date] | Datum |
   | [!UICONTROL Integration Notes] | Textfält för stycke |

   Mer information om hur du skapar anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Förväntat [!DNL Anaplan] Konfiguration

Du måste ha följande i [!DNL Anaplan] om du vill använda det här scenariot:

* En användarprofil i [!DNL Anaplan] namngiven **[!UICONTROL [!DNL Workfront ] Integration]**, som har systemadministratörsbehörighet.
* The [!DNL Anaplan] Modell som du vill använda för det här scenariot.
* Listan i [!DNL Anaplan] Modell som ni vill ha för kampanjbudgetar.
* An **[!UICONTROL Anaplan Actual Expense Import]** som innehåller följande kolumner, i den här ordningen:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]
   Förbered [!UICONTROL [!DNL Anaplan] Actual Expense Import] fil:

   1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel].
   1. Spara filen i CSV-format.
   1. Överför filen till [!DNL Anaplan].

      Instruktioner finns i [!DNL Anaplan] dokumentation om hur du importerar data till moduler från en fil.

   1. Anteckna det namn du gett filen. den kommer att användas under distributionen av [!UICONTROL Fusion] scenariomall.

   Exempel på CSV-innehåll

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* An **[!UICONTROL [!DNL Anaplan] Planned Expense Import]** som innehåller följande kolumner, i den här ordningen:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]
   Förbered [!UICONTROL [!DNL Anaplan] Planned Expense Import] fil:

   1. Kopiera och klistra in följande i en textredigerare eller [!DNL Excel]
   1. Spara filen i CSV-format
   1. Överför filen till Anaplan.

      Instruktioner finns i [!DNL Anaplan] dokumentation om hur du importerar data till moduler från en fil.

   1. Anteckna det namn du gett filen. den kommer att användas under distributionen av [!UICONTROL Fusion] scenariomall.

   Exempel på CSV-innehåll

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>


* A **[!UICONTROL Project Update Import]** process som förbereds för import av data som levereras i en filöverföring.

>[!NOTE]
>
>Det finns separata importfiler för planerade och faktiska utgifter så att de kan rapporteras oberoende av planerat respektive gällande datum.

Instruktioner om dessa åtgärder finns i [!DNL Anaplan] dokumentation.

## Distribuerar till [!DNL Fusion]

Utför följande steg för att distribuera integreringsscenariot till din [!DNL Fusion] konto. Detta bör endast göras efter att du fyllt i [!DNL Workfront] och [!DNL Anaplan] konfiguration.

1. Navigera till [!UICONTROL Templates] menyn i [!DNL Workfront Fusion] och klicka på **[!UICONTROL Send Workfront expenses updates to [!DNL Anaplan] list item]** scenariomall.
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
      <td>ID:t för arbetsytan från din [!DNL Anaplan] konto som du vill använda för det här scenariot.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modell-ID] </td> 
      <td>ID:t för modellen från din [!DNL Anaplan] och den valda arbetsytan som du vill använda för det här scenariot.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Namnet på listan från din [!DNL Anaplan] konto och den valda arbetsytan och modellen som du vill använda för det här scenariot.</td> 
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

   Information om hur du konfigurerar filer och processer finns i [!DNL Anaplan] installationsdokumentation.

1. Markera eller lägga till en [!DNL Anaplan] anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med [!DNL Anaplan] anslutning när du uppmanas till detta.
1. Markera eller lägga till en [!DNL Workfront] anslutningsprofil.
1. Uppdatera alla återstående [!DNL Workfront] moduler med [!DNL Workfront] anslutning när du uppmanas till detta.
1. På **[!UICONTROL Build Actual Expense CSV]** lägger du till en ny datastruktur för att mappa projektattributen till CSV-kolumner.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. På **[!UICONTROL Build Planned Expense CSV]** lägger du till en ny datastruktur för att mappa projektattributen till CSV-kolumner.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

## Andra rekommenderade scenariomallar

Den här scenariomallen kompletteras av följande mallar för utgiftsoptimeringsscenarier som också kan distribueras:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] faktiskt antal timmars uppdateringar av en [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Ytterligare scenarier för länkning av budgetbegäranden:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för länkning av kampanjförfrågningar:

* [[!UICONTROL Create an [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] kampanjförfrågan]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] kampanjförfrågan eller kampanjprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
