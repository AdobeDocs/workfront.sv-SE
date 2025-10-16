---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skapa ett  [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan
description: Det här integreringsscenariot länkar ett [!DNL Adobe Workfront] projekt (kampanj) med ett [!DNL Anaplan] budgetlistobjekt. Detta uppnås genom att en budgetförfrågan läggs till i  [!DNL Workfront] projektet som behöver få finansiering. Det här scenariot söker efter obearbetade budgetbegäranden och kör sedan en process för att skapa ett tomt budgetlistobjekt i  [!DNL Anaplan]  för att starta budgetallokeringsprocesser i Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Skapa ett [!DNL Anaplan]-listobjekt från en [!DNL Adobe Workfront]-budgetförfrågan

Det här integreringsscenariot länkar ett [!DNL Adobe Workfront]-projekt (kampanj) med ett [!DNL Anaplan]-budgetlistobjekt. Detta uppnås genom att en budgetförfrågan läggs till i projektet [!DNL Workfront] som behöver få finansiering. Det här scenariot söker efter obearbetade budgetbegäranden och kör sedan en process för att skapa ett tomt budgetlistobjekt i [!DNL Anaplan] för att starta budgetallokeringsprocesser i [!DNL Anaplan].

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

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## [!DNL Workfront]-konfiguration förväntades

Du måste ha följande i [!DNL Workfront] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Workfront] med namnet **[!DNL Anaplan]Integration** som har systemadministratörsbehörighet.

  Mer information om hur du skapar en användare i [!DNL Workfront] finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ett **[!UICONTROL Budget Request]** anpassat formulär som är kopplat till objektet [!UICONTROL Request].

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

  Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Projektmallar som representerar kampanjer och andra projekt som behöver finansieras, konfigurerade med ett [!UICONTROL Budget Request]-kötema. Köämnet [!UICONTROL Budget Request] har tilldelats till det anpassade formuläret [!UICONTROL Budget Request].
* Ett **[!UICONTROL Campaign Brief]**-formulär för projektobjektet.

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

  Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## [!DNL Anaplan]-konfiguration förväntades

Du måste ha följande i [!DNL Anaplan] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Anaplan] med namnet **[!UICONTROL [!DNL Workfront] Integration]** som har systemadministratörsbehörighet.
* Modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* Listan i modellen [!DNL Anaplan] som samlar in kampanjbudgetar.

  Listans modul måste ha stöd för följande attribut:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Requested Expense Funds]
   * [!UICONTROL Budget Request Type]
   * [!UICONTROL Reason for Funding Adjustment]

  Den här listan och modulen måste lagra ytterligare information som är nödvändig för den normala funktionen i [!DNL Anaplan], inklusive möjligheten att ställa in en budget och meddela att budgetlistobjektet är klart att synkroniseras tillbaka till [!DNL Workfront].

Instruktioner om dessa åtgärder finns i dokumentationen för [!DNL Anaplan].

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera det här integreringsscenariot till ditt [!DNL Fusion]-konto. Detta bör endast göras efter att den nödvändiga [!DNL Workfront]- och [!DNL Anaplan]-konfigurationen har slutförts.

1. Navigera till menyn [!UICONTROL Templates] i [!DNL Workfront Fusion] och klicka på mallen för **[!UICONTROL Create an [!DNL Anaplan] list item from a Workfront budget request]**-scenarier.
1. Ersätt variabelvärdena för följande [!DNL Anaplan]-variabler:

   | Variabelnamn | Ersätt värde med |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | ID för en arbetsyta från ditt [!DNL Anaplan]-konto. |
   | [!UICONTROL [!DNL Anaplan] Model ID] | ID:t för en modell från ditt [!DNL Anaplan]-konto och den valda arbetsytan. |
   | [!UICONTROL [!DNL Anaplan] Module Name] | Namnet på modulen som beskriver kampanjattributen i den valda [!DNL Anaplan]-listan. |
   | [!UICONTROL Campaign List Name] | Namnet på listan från ditt [!DNL Anaplan]-konto och den valda arbetsytan och modellen. |

   {style="table-layout:auto"}

   Information om hur du konfigurerar filer och processer finns i installationsdokumentationen för [!DNL Anaplan].

1. Välj eller lägg till en [!DNL Anaplan]-anslutningsprofil.
1. Uppdatera alla återstående [!DNL Anaplan] moduler med en [!DNL Anaplan]-anslutning när du uppmanas till det.
1. Välj eller lägg till en [!DNL Workfront]-anslutningsprofil.

   När du har distribuerat mallen är det här modulen som du uppdaterar för att lägga till eller ta bort anpassade fältreferenser från värdet för fältegenskapen om du vill ändra de mappade standardfälten till [!DNL Anaplan].

1. Uppdatera alla återstående [!DNL Workfront] moduler med en [!DNL Workfront]-anslutning när du uppmanas till det.

## Andra rekommenderade scenariomallar

Om du vill slutföra arbetsflödet som den här mallen representerar måste du även distribuera följande extra mall:

* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till ett [!DNL Adobe Workfront] projekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Ytterligare scenarier för utgiftsoptimering är:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] faktiska timmars uppdateringar av ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
