---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Använd planerade datum i en kalenderrapport
description: En kalenderrapport är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda fälten för projektdatum i en kalenderrapport för uppgifter, utgåvor och projekt.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Använd [!UICONTROL Projected Dates] i en kalenderrapport

En kalenderrapport är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda fälten för projektdatum i en kalenderrapport för följande objekt:

* Uppgifter
* Problem
* Projekt

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL ]Redigera åtkomst till [!UICONTROL Reports], [!UICONTROL Dashboards]och [!UICONTROL Calendars]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage] åtkomst till kalenderrapporten</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Ställ in artikelgruppen

Du kan välja hur du vill att objektgruppen ska visas i kalendern.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Calendars]**.

1. Markera den kalender som du vill lägga till en ny grupp med objekt i.\
   eller\
   Klicka **[!UICONTROL + New Calendar]** och ange kalendernamnet.

   >[!NOTE]
   >
   >Du måste ha [!UICONTROL Edit] behörighet till [!UICONTROL Reports], [!UICONTROL Dashboards]och [!UICONTROL Calendars] på din åtkomstnivå för att skapa en kalenderrapport.

1. Till vänster klickar du på **[!UICONTROL Add to Calendar]** och sedan klicka **[!UICONTROL Add advanced items]**.

1. Ange följande:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Ange ett namn för gruppen med objekt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Välj en färg för gruppen med objekt. Alla objekt visas i den valda färgen i kalenderrapporten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Välj <strong>[!UICONTROL Projected dates]</strong>. Mer information om planerade datum finns i </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Översikt över projektets planerade startdatum</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Välj hur du vill att datumen ska visas:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: I kalendern visas objektet på ett enda datum.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: I kalendern visas objektet på ett enda datum.</li>
        <li><strong>[!UICONTROL Duration] (Från början till slut)</strong>: I kalendern visas objektet över ett antal dagar.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to Actual Dates when available]</strong></td>
      <td><p>Kalendern växlar automatiskt till faktiska datum när de är tillgängliga. <br>Välj <strong>[!UICONTROL Yes]</strong> eller <strong>[!UICONTROL No]</strong> för att växla till faktiska datum när det är tillgängligt. Mer information om faktiska datum finns i</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Översikt över projektets faktiska startdatum </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Översikt över projektets faktiska slutförandedatum </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Fortsätt till följande avsnitt.

## Lägga till objekt i objektgruppen

När du har ställt in hur du vill att objekten ska visas måste du lägga till de objekt som du vill se i kalendern i grupperingen.

1. I **[!UICONTROL What would you like to add to the calendar?]** avsnitt, markera

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Klicka **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, eller **[!UICONTROL Add Issues]**, beroende på vilken objekttyp du lägger till i kalendern.\
   ![Välj objekt för kalender](assets/field-name.png)

1. I listrutan börjar du skriva fältnamnet och väljer sedan fältkällan för objektet som du vill visa i kalendern (till exempel **[!UICONTROL Late Tasks]**).
1. Ange en villkorssats för kalendergrupperingen.

   ![Villkorssats](assets/condition-statement-calendar.png)

   Mer information om hur du ställer in villkor finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Valfritt) Ange ytterligare objekt för kalendergrupperingen genom att upprepa steg 1-4.
1. I **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** väljer du hur objekten i den här kalendergruppen ska märkas i kalendern.

   >[!NOTE]
   >
   >Om standardetikettalternativen inte är tillgängliga för ett visst objekt visas objektnamnet i stället. När etiketten Överordnad aktivitet är markerad och det inte finns någon överordnad uppgift kopplad till objektet, [!DNL Adobe Workfront] visar objektnamnet som du visar i kalendern.

1. Klicka på **[!UICONTROL Save]**.
