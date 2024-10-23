---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Skapa ett  [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] kampanjbegäran
description: Det här integreringsscenariot länkar ett [!DNL Adobe Workfront] projekt till ett [!DNL Anaplan] budgetlistobjekt.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Skapa ett [!DNL Anaplan]-listobjekt från en [!DNL Adobe Workfront]-kampanjbegäran

Det här integreringsscenariot länkar ett [!DNL Adobe Workfront]-projekt till ett [!DNL Anaplan]-budgetlisteobjekt.

Det här scenariot söker efter nya kampanjförfrågningar som lagts till i en begärandekö. Så snart en kampanjförfrågan har registrerats läggs en budgetradobjekt till i [!DNL Anaplan] för att starta finansieringsprocessen.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan*</td> 
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

&#42;&#42;Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Starthändelse

Detta scenario är schemalagt att köras var 15:e minut.

## [!DNL Workfront]-konfiguration förväntades

Du måste ha följande i [!DNL Workfront] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Workfront] med namnet **[!UICONTROL [!DNL Anaplan] Integration]** som har systemadministratörsbehörighet.

  Mer information om hur du skapar en användare i [!DNL Workfront] finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Ett **[!UICONTROL Campaign Brief]** anpassat formulär som är kopplat till objektet [!UICONTROL Request].

  Följande obligatoriska fält måste inkluderas i det anpassade formuläret för att underlätta datamappning till Anaplan:

  | Fältnamn | Fälttyp |
  |---|---|
  | [!UICONTROL Total Requested Funds] |   |
  | [!UICONTROL Requested Labor Funds] |   |
  | [!UICONTROL Requested Expense Funds] |   |
  | [!UICONTROL Sent to [!DNL Anaplan]] | Kryssruta |

  Följande valfria fält kan finnas i formuläret. Detta scenario mappar endast fälten ovan, men eventuella ytterligare fält i kampanjöversikten kan mappas.

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
     <td>Datum </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>Datum</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>Textfält för stycke</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>Textfält för stycke</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>Listruta</p> <p>Inkludera alternativ som passar era processer.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Ett projekt som har konfigurerats som en begärandekö för att hämta nya kampanjförfrågningar. Formuläret [!UICONTROL Campaign Brief] måste bifogas till dessa förfrågningar.

## [!DNL Anaplan]-konfiguration förväntades

Du måste ha följande i [!DNL Anaplan] för att kunna använda det här scenariot:

* En användarprofil i [!DNL Anaplan] med namnet **[!UICONTROL [!DNL Workfront] Integration]** som har systemadministratörsbehörighet.
* Modellen [!DNL Anaplan] som du vill använda för det här scenariot.
* Listan i modellen [!DNL Anaplan] som samlar in kampanjbudgetar.

  Listans modul måste ha stöd för följande attribut:

   * [!UICONTROL [!DNL Workfront] Request GUID]
   * [!UICONTROL [!DNL Workfront] Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Requested Expense Funds]
   * [!UICONTROL Budget Request Type]

  Den här listan och modulen måste lagra ytterligare information som är nödvändig för den normala funktionen i [!DNL Anaplan], inklusive möjligheten att ställa in en budget och meddela att budgetlistobjektet är klart att synkroniseras tillbaka till [!DNL Workfront].

Instruktioner om dessa åtgärder finns i dokumentationen för [!DNL Anaplan].

## Distribuerar till [!DNL Workfront Fusion]

Utför följande steg för att distribuera det här integreringsscenariot till ditt [!DNL Fusion]-konto. Detta bör endast göras efter att den nödvändiga [!DNL Workfront]- och [!DNL Anaplan]-konfigurationen har slutförts.

1. Navigera till menyn [!UICONTROL Templates] i [!DNL Workfront Fusion] och klicka på mallen för **[!UICONTROL Create an [!DNL Anaplan] list item from a Workfront campaign request]**-scenarier.
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

* [[!UICONTROL Apply an [!DNL Anaplan] budgetallokering till en  [!DNL Adobe Workfront] kampanjbegäran eller ett kampanjprojekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Ytterligare scenarier för utgiftsoptimering är:

* [[!UICONTROL Send [!DNL Adobe Workfront] projektuppdateringar till ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] faktiska timmars uppdateringar av ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] utgifter för ett  [!DNL Anaplan] listobjekt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
