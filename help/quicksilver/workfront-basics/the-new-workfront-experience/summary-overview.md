---
content-type: overview
title: Sammanfattning
description: Du kan använda panelen Sammanfattning för att granska och uppdatera information om arbetsobjekt direkt från en lista med uppgiftsproblem, dokument eller från andra områden i [!DNL Adobe Workfront] som visar uppgifter och problem.
feature: Get Started with Workfront
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: d8ca244e430f8a0e96b201bf09eba8b83b774a57
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# [!UICONTROL Summary] översikt

Du kan använda [!UICONTROL Summary] för att granska och uppdatera information om arbetsobjekt direkt från en lista med uppgiftsproblem, dokument eller andra områden i [!DNL Adobe Workfront] som visar uppgifter och problem.

I följande tabell visas de områden där du kan söka efter och använda [!UICONTROL Summary] panel:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Uppgifter</td> 
  </tr> 
  <tr> 
   <td> <p>Uppgiftslistor i en</p> 
    <ul> 
     <li>Projekt</li> 
     <li>Underuppgift</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Uppgifter i [!UICONTROL Unassigned] och [!UICONTROL Assigned] Arbetsytor i [!DNL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problem</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Ärendelistor i en</p> 
    <ul> 
     <li>Projekt</li> 
     <li>Uppgift</li> 
     <li>Underuppgift</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problem i [!UICONTROL Assigned Work] området på [!DNL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problem i [!UICONTROL Submitted] i [!UICONTROL Requests] area</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Dokument</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Documents] area</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Documents] del av ett objekt (projekt, uppgift, utgåva, program, portfölj, mall, malluppgift, användare)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

I den här artikeln beskrivs hur du får åtkomst till och använder [!UICONTROL Summary] för uppgifter och problem i listor.

Mer information om åtkomst till [!UICONTROL Summary] i [!DNL Workload Balancer], se [Uppdatera arbetsobjekt i [!DNL Workload Balancer] med [!UICONTROL Summary]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Mer information om åtkomst till [!UICONTROL Summary] för dokument, se [[!UICONTROL Summary] för dokumentöversikt](../../documents/managing-documents/summary-for-documents.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] eller högre tillgång till uppgifter, ärenden, dokument</p> <p>[!UICONTROL View] eller senare åtkomst till objekt som du vill visa dokumentets [!UICONTROL Summary]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL View] eller högre behörighet till en uppgift, ett problem eller ett dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Visa [!UICONTROL Summary] i en lista med uppgifter eller problem

1. Gå till en uppgift eller ett ärende och välj ett objekt i listan.
1. Klicka på **[!UICONTROL Summary]** icon ![](assets/qs-summary-in-new-toolbar-small.png)

   eller

   Klicka på **[!UICONTROL Open Summary]** icon ![](assets/open-summary-with-text-nwe.png) i [!UICONTROL Submitted] i [!UICONTROL Requests] område.

   När du har öppnat sammanfattningen förblir den öppen när du klickar på eller väljer andra uppgifter eller ärenden och är öppen tills du stänger den manuellt.

   >[!TIP]
   >
   >Du kan bara välja en aktivitet eller en utgåva åt gången för att visa informationen om dem i [!UICONTROL Summary] -panelen.

   ![](assets/summary-overview--open-task-from-summary-icon-350x112.png)

1. (Valfritt) Stäng [!UICONTROL Summary] gör du något av följande:

   * Klicka på **[!UICONTROL Open Summary]** icon ![](assets/summary-panel-icon.png)

      eller

      Klicka på **X** ikonen i det övre högra hörnet av [!UICONTROL Summary] -panelen.

   * I [!UICONTROL Submitted] i [!UICONTROL Requests] klickar du på **[!UICONTROL Close Summary]** icon ![](assets/close-summary-with-text-nwe.png)

      eller

      Klicka på **X** i det övre högra hörnet av panelen Sammanfattning.

## [!UICONTROL Percent Complete]

Använd förloppsindikatorn högst upp i [!UICONTROL Summary] om du vill uppdatera procentandelen färdigt för den uppgift eller utgåva som du har valt. Ange ett tal eller dra fältet till rätt procentvärde.

![](assets/summary-overview-percent-complete-350x395.png)

## [!UICONTROL Updates]

Använd [!UICONTROL Updates] i [!UICONTROL Summary] om du vill visa de senaste uppdateringarna och göra uppdateringar för den uppgift eller utgåva du har valt. Klicka **[!UICONTROL See all]** för att gå direkt till [!UICONTROL Updates] -fliken för uppgiften.

![](assets/summary-updates-with-block-quote-350x290.png)

## [!UICONTROL Documents]

Använd [!UICONTROL Documents] i [!UICONTROL Summary] om du vill visa dokument som är kopplade till den uppgift eller det problem du valde. Klicka på miniatyrbilden för att öppna en dokumentförhandsvisning. Gå direkt till [!UICONTROL Documents] klickar du på **[!UICONTROL Documents]** titel.

![](assets/summary-overview-documents-350x84.png)

## [!UICONTROL Details]

Använd [!UICONTROL Details] i [!UICONTROL Summary] om du vill visa detaljer om arbetsuppgift på hög nivå, göra uppdrag eller lägga till startdatum. Klicka **[!UICONTROL See all]** för att gå direkt till [!UICONTROL Details] -fliken för uppgiften eller problemet.

>[!NOTE]
>
>Fälten som visas i det här avsnittet är samma fält som visas på den högra panelen i Hem. Du kan anpassa dessa fält [Anpassa [!UICONTROL Home] och [!UICONTROL Summary] använda en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![](assets/summary-overview-details-new-350x278.png)

## [!UICONTROL Subtasks]

Det här avsnittet är bara tillgängligt för uppgifter. Använd [!UICONTROL Subtasks] i [!UICONTROL Summary] visa [!UICONTROL New], [!UICONTROL In Progress]och [!UICONTROL Closed] underuppgifter för den valda uppgiften. Klicka på **[!UICONTROL Status]** för att växla mellan olika lägen. Gå direkt till [!UICONTROL Subtasks] klickar du på **[!UICONTROL Subtasks]**&#x200B;.

Om du inte har lagt till några underaktiviteter till uppgiften klickar du på **[!UICONTROL Add one here]** för att gå direkt till [!UICONTROL Subtasks] -fliken för uppgiften.

![](assets/summary-overview-subtasks-350x140.png)

## [!UICONTROL Hours]

Använd [!UICONTROL Hours] i [!UICONTROL Summary] om du vill logga timmar på den uppgift eller det problem du valde. Klicka **[!UICONTROL Log Time]** och ange dina timmar. Om du vill gå direkt till fliken Timmar för uppgiften eller problemet klickar du på **[!UICONTROL Hours]** titel.

Timantal i [!UICONTROL Summary] visar de timmar du loggar. Andra användare har olika timsummor i [!UICONTROL Summary] beroende på när de loggar in.

Om det inte finns några planerade [!UICONTROL hours] på uppgiften eller problemet och du har loggat tid visas timfältet med rött.

![](assets/summary-overview-hours-350x96.png)

## Godkännanden

Använd [!UICONTROL Approvals] i [!UICONTROL Summary] om du vill visa godkännanden som är kopplade till den uppgift eller det ärende du valde. Om du inte har lagt till några godkännanden väljer du ett befintligt godkännande i listrutan eller klickar på **[!UICONTROL Create single-use approval process]** för att gå direkt till [!UICONTROL Approvals] -fliken för uppgiften eller problemet.

Gå direkt till [!UICONTROL Approvals] klickar du på **[!UICONTROL Approvals]** titel.

![](assets/summary-overview-approvals-350x122.png)
