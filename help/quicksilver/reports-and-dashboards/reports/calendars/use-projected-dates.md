---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Använd planerade datum i en kalenderrapport
description: En kalenderrapport är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda fälten för projektdatum i en kalenderrapport för uppgifter, utgåvor och projekt.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: 5c0278607faf65b58abeb9b813e403f97032a965
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Använd [!UICONTROL Projected Dates] i en kalenderrapport

En kalenderrapport är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda fälten för projektdatum i en kalenderrapport för följande objekt:

* Uppgifter
* Problem
* Projekt

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!UICONTROL Reports], [!UICONTROL Dashboards] och [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>[!UICONTROL Manage] åtkomst till kalenderrapporten</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ställ in artikelgruppen

Du kan välja hur du vill att gruppen med objekt ska visas i din kalender.

{{step1-to-calendars}}

1. Välj den kalender som du vill lägga till en ny grupp med objekt, klicka på menyn Mer och sedan **Redigera**.
eller
Klicka på **[!UICONTROL + New Calendar]**, ange projektnamnet och klicka sedan på **[!UICONTROL Add advanced items]**.

   >[!NOTE]
   >
   >Du måste ha [!UICONTROL Edit] åtkomst till [!UICONTROL Reports], [!UICONTROL Dashboards] och [!UICONTROL Calendars] på din åtkomstnivå för att skapa en kalenderrapport.

1. Klicka på **[!UICONTROL Add to Calendar]** till vänster och sedan på **[!UICONTROL Add advanced items]**.

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
        <li><strong>[!UICONTROL Duration] (från början till slut)</strong>: I kalendern visas objektet över ett antal dagar.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to Actual Dates when available]</strong></td>
      <td><p>Kalendern växlar automatiskt till faktiska datum när de är tillgängliga. <br>Välj <strong>[!UICONTROL Yes]</strong> eller <strong>[!UICONTROL No]</strong> om du vill växla till faktiska datum när det är tillgängligt. Mer information om faktiska datum finns i</p>
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

1. I avsnittet **[!UICONTROL What would you like to add to the calendar?]** väljer du

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**
   * **[!UICONTROL Time Off]**
1. Klicka på **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]** eller **[!UICONTROL Add Issues]**, beroende på vilken objekttyp du lägger till i kalendern.

1. I listrutan börjar du skriva fältnamnet och väljer sedan fältkällan för objektet som du vill visa i kalendern (till exempel **[!UICONTROL Late Tasks]**).
1. Ange en villkorssats för kalendergrupperingen.


   ![Välj objekt för kalendern](assets/calendar-field-name.png)
Mer information om hur du ställer in villkor finns i [Filter och villkorsmodifierare ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md) .

1. (Valfritt) Ange ytterligare objekt för kalendergrupperingen genom att upprepa steg 1-4.
1. I fältet **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** väljer du hur objekten i den här kalendergruppen ska märkas i kalendern.

   >[!NOTE]
   >
   >Om standardetikettalternativen inte är tillgängliga för ett visst objekt visas objektnamnet i stället. Om etiketten [!UICONTROL Parent Task] till exempel är markerad och det inte finns någon överordnad aktivitet kopplad till objektet, visar [!DNL Adobe Workfront] objektnamnet som du visar i kalendern.

   ![ange aktivitetsetiketter](assets/set-task-labels.png)

1. Klicka på **[!UICONTROL Save]**.

