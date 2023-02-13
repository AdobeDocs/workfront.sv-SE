---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skapa en [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan
description: Det här integreringsscenariot länkar en [!DNL Adobe Workfront] projekt (kampanj) med [!DNL Anaplan] budgetlisteartikel. Detta uppnås genom att en budgetförfrågan läggs till i [!DNL Workfront] projekt som behöver få finansiering. Det här scenariot söker efter obearbetade budgetbegäranden och kör sedan en process för att skapa en tom budgetlistartikel i [!DNL Anaplan] för att få igång budgetallokeringsprocesserna i Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Skapa en [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan

Det här integreringsscenariot länkar en [!DNL Adobe Workfront] projekt (kampanj) med [!DNL Anaplan] budgetlisteartikel. Detta uppnås genom att en budgetförfrågan läggs till i [!DNL Workfront] projekt som behöver få finansiering. Det här scenariot söker efter obearbetade budgetbegäranden och kör sedan en process för att skapa en tom budgetlistartikel i [!DNL Anaplan] för att snabbt komma igång med budgetallokeringsprocesser i [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Adobe Workfront Fusion] licens**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr>
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

&#42;&#42;För information om[!DNL  Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## Förväntat [!DNL Workfront] Konfiguration

Du måste ha följande i [!DNL Workfront] om du vill använda det här scenariot:

* En användarprofil i [!DNL Workfront] namngiven *[!UICONTROL *[!DNL Anaplan] Integration]**, som har systemadministratörsbehörighet.

   Mer information om hur du skapar en användare i [!DNL Workfront], se [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Budget Request]** anpassat formulär kopplat till [!UICONTROL Request] -objekt.

   Följande obligatoriska fält måste inkluderas i det anpassade formuläret för att underlätta datamappning till [!DNL Anaplan]:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Fältnamn</th> 
     <th>Fälttyp</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Budget Request Type]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Alternativ:</p> 
      <ul> 
       <li> <p>[!UICONTROL Adjustment to Funding]</p> </li> 
       <li> <p>[!UICONTROL Initial Funding]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Labor Funds]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Expense Funds]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

   Mer information om hur du skapar anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Projektmallar som representerar kampanjer och andra projekt som kräver finansiering, konfigurerade med en [!UICONTROL Budget Request] köämne. The [!UICONTROL Budget Request] köämnet har tilldelats till att använda [!UICONTROL Budget Request] eget formulär.
* A **[!UICONTROL Campaign Brief]** -formulär för projektobjektet.

   Formuläret måste innehålla följande fält:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Inkludera alternativ som passar era processer.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Mer information om hur du skapar anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Förväntat [!DNL Anaplan] Konfiguration

Du måste ha följande i [!DNL Anaplan] om du vill använda det här scenariot:

* En användarprofil i [!DNL Anaplan] namngiven **[!UICONTROL [!DNL Workfront] Integration]**, som har systemadministratörsbehörighet.
* The [!DNL Anaplan] Modell som du vill använda för det här scenariot.
* Listan i [!DNL Anaplan] Modell som fångar kampanjbudgetar.

   Listans modul måste ha stöd för följande attribut:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Requested Expense Funds]
   * [!UICONTROL Budget Request Type]
   * [!UICONTROL Reason for Funding Adjustment]

   Den här listan och modulen måste lagra ytterligare information som är nödvändig för den normala funktionen hos [!DNL Anaplan], inklusive möjligheten att ställa in en budget och meddela att budgetlisteposten är klar att synkroniseras tillbaka till [!DNL Workfront].

Instruktioner om dessa åtgärder finns i [!DNL Anaplan] dokumentation.

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera integreringsscenariot till din [!DNL Fusion] konto. Detta bör endast göras efter att du fyllt i [!DNL Workfront] och [!DNL Anaplan] konfiguration.

1. Navigera till [!UICONTROL Templates] menyn i [!DNL Workfront Fusion] och klicka på **[!UICONTROL Create an [!DNL Anaplan] list item from a Workfront budget request]** scenariomall.
1. Ersätt variabelvärdena för följande [!DNL Anaplan] variabler:

   | Variabelnamn | Ersätt värde med |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | ID:t för en arbetsyta från din [!DNL Anaplan] konto. |
   | [!UICONTROL [!DNL Anaplan] Model ID] | ID:t för en modell från din [!DNL Anaplan] och den valda arbetsytan. |
   | [!UICONTROL [!DNL Anaplan] Module Name] | Namnet på modulen som beskriver kampanjattributen i det valda [!DNL Anaplan] Lista. |
   | [!UICONTROL Campaign List Name] | Namnet på listan från din [!DNL Anaplan] och den valda arbetsytan och modellen. |

   {style=&quot;table-layout:auto&quot;}

   Information om hur du konfigurerar filer och processer finns i [!DNL Anaplan] installationsdokumentation.

1. Markera eller lägga till en [!DNL Anaplan] anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med [!DNL Anaplan] anslutning när du uppmanas till detta.
1. Markera eller lägga till en [!DNL Workfront] anslutningsprofil.

   När du har distribuerat mallen är det här modulen som du uppdaterar för att lägga till eller ta bort anpassade fältreferenser från värdet för fältegenskapen om du vill ändra de mappade standardfälten till [!DNL Anaplan].

1. Uppdatera alla återstående [!DNL Workfront] moduler med [!DNL Workfront] anslutning när du uppmanas till detta.

## Andra rekommenderade scenariomallar

Om du vill slutföra arbetsflödet som den här mallen representerar måste du även distribuera följande extra mall:

* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för utgiftsoptimering är:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] faktiskt antal timmars uppdateringar av en [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
