---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Ta bort initiativ i scenarioplanen
description: Du kan ta bort initiativ för en plan som du har skapat eller för en plan som någon har delat med dig. Du kan inte återställa initiativ som du har tagit bort.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Ta bort initiativ i [!DNL Scenario Planner]

Du kan ta bort initiativ för en plan som du har skapat eller för en plan som någon har delat med dig. Du kan inte återställa initiativ som du har tagit bort.

## Åtkomstkrav

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] eller högre</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licens*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till funktioner som beskrivs i den här artikeln. </p> <p>Mer information om hur du får [!DNL Workfront Scenario Planner], se <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationer på åtkomstnivå*</strong> </td> 
   <td> <p>[!UICONTROL Edit] åtkomst eller högre till [!DNL Scenario Planner]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ta bort initiativ

Tänk på följande när du tar bort initiativ:

* När du tar bort ett initiativ tas mängden jobbroller och den kostnadsinformation som är kopplad till initiativet bort från planen.
* Om du tar bort ett projekt som har skapats genom att ett projekt importeras, tas inte det projekt som är kopplat till initiativet bort.
* Borttagning av ett projekt som har publicerats till ett projekt minst en gång ger följande resultat:

   * Initiativet tas bort från scenariot men [!DNL Scenario Planner] finns kvar i [!UICONTROL Project Details] -avsnitt.
   * Om det initiativ du tar bort är det enda publicerade initiativet i scenariot, tas även indikatorn för att planen har publicerats bort.

      Mer information om publicering av projekt finns i [Uppdatera eller skapa projekt genom att publicera i [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      Mer information om hur du skapar initiativ genom att importera projekt finns i [Importera projekt till planer i [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Du kan ta bort ett initiativ åt gången eller ta bort flera initiativ samtidigt.

* [Ta bort ett initiativ](#delete-one-initiative)
* [Ta bort satsningar](#delete-initiatives-in-bulk)

### Ta bort ett initiativ {#delete-one-initiative}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png)och sedan klicka [!UICONTROL Scenarios].

   En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på det initiativ du vill ta bort.
1. Gör något av följande:

   * Klicka på **[!UICONTROL More menu]** ![](assets/more-menu.png) till höger om företagsnamnet och klicka sedan på **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   * Markera rutan till vänster om initiativet och klicka sedan på **[!UICONTROL Delete]** på den flytande meny som visas längst ned i planen och klicka sedan på **[!UICONTROL Yes, delete it]**.

   Initiativet, dess befattning och kostnadsinformation tas bort från planen.

1. Klicka **[!UICONTROL Save Plan]** för att spara ändringarna.

### Ta bort satsningar {#delete-initiatives-in-bulk}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png)och sedan klicka [!UICONTROL Scenarios].

   En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på det initiativ du vill ta bort.
1. Markera rutorna till vänster om de initiativ du vill ta bort och klicka sedan på **[!UICONTROL Delete]** på den meny som visas längst ned i planen och klicka sedan på **[!UICONTROL Yes, delete them]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Initiativen och deras jobbroll och kostnadsinformation tas bort från planen.

1. Klicka **[!UICONTROL Save Plan]** för att spara ändringarna.
