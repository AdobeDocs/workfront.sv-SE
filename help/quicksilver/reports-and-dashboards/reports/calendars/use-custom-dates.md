---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Använd anpassade datumfält i en kalenderrapport
description: En kalenderrapport är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda anpassade datumfält i en kalenderrapport för uppgifter, utgåvor och projekt.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Använd anpassade datumfält i en kalenderrapport

A [!UICONTROL calendar] är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda anpassade datumfält i en kalenderrapport för följande objekt:

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
   <td> <p>[!UICONTROL Edit] behörighet till [!UICONTROL Reports], [!UICONTROL Dashboards]och [!UICONTROL Calendars]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage] åtkomst till kalenderrapporten</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Förutsättningar

1. Du måste ha anpassade datumfält och ett värde i fältet tillgängligt i [!DNL Workfront] -instans. Om du inte har skapat något anpassat formulär med anpassade datum följer du instruktionerna i de två första avsnitten i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Bifoga det anpassade formuläret till ett projekt, en uppgift eller ett ärende som du tänker lägga till i kalendern och ange ett datum. Mer information finns i [Lägga till ett anpassat formulär i ett objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Ställ in artikelgruppen

Du kan välja hur du vill att gruppen med objekt ska visas i din kalender.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Calendars]**.

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
      <td>Välj <strong>[!UICONTROL Custom dates]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Välj hur du vill att datumen ska visas:</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: I kalendern visas objektet på ett enda datum.</li>
        <li><strong>[!UICONTROL Duration] (Från början till slut)</strong>: I kalendern visas objektet över ett antal dagar.<br><p>Obs! Om du väljer <strong>[!UICONTROL Duration]</strong>måste slutdatumet som anges vara efter startdatumet, annars visas inte objektet i kalendern.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>Ange det anpassade datumnamnet som är kopplat till objektet som du vill spåra.</p><p><strong>OBS!</strong> Sökningen efter det anpassade datumnamnet är begränsad till 50 resultat för att undvika prestandaproblem.</td>
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

1. I listrutan börjar du skriva fältnamnet och väljer sedan fältkällan för det objekt som du vill visa i kalendern (till exempel **[!UICONTROL Late Tasks]**).
1. Ange en villkorssats för kalendergrupperingen.

   ![Villkorssats](assets/condition-statement-calendar.png)

   Mer information om hur du ställer in villkor finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Valfritt) Ange ytterligare objekt för kalendergrupperingen genom att upprepa steg 1-4.
1. I **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** väljer du hur objekten i den här kalendergruppen ska märkas i kalendern.

   >[!NOTE]
   >
   >Om standardetikettalternativen inte är tillgängliga för ett visst objekt visas objektnamnet i stället. När [!UICONTROL Parent Task] etiketten är markerad och det finns ingen överordnad uppgift kopplad till objektet, [!DNL Adobe Workfront] visar objektnamnet som du visar i kalendern.

1. Klicka på **[!UICONTROL Save]**.
