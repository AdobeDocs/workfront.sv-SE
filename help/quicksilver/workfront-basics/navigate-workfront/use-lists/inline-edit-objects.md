---
product-area: projects
navigation-topic: use-lists
title: Redigera objekt i en lista i [!DNL Adobe Workfront]
description: Du kan redigera objekt textbundet när de visas i en lista eller rapport. När du redigerar informationen om objekt som visas i en lista eller rapport uppdateras objektet omedelbart.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: f0912e4ef29d682ae3e6dd0e543b8e77fb7f29b6
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Redigera objekt i en lista i [!DNL Adobe Workfront]

Du kan redigera objekt textbundet när de visas i en lista eller rapport. När du redigerar informationen om objekt som visas i en lista eller rapport uppdateras objektet omedelbart.

När du infogar redigering av ett fält i ett anpassat formulär som inte är kopplat till objektet, läggs det anpassade formuläret automatiskt till objektet. Om fältet finns i flera anpassade formulär bifogas det anpassade formulär som uppdaterades senast till objektet.

Mer information om listor finns i [Kom igång med listor i [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

De flesta objekt som visas i listor eller rapporter kan redigeras i [!DNL Adobe Workfront], finns det några begränsningar, som:

* Du kan inte redigera beräknade fält eller [!DNL Workfront] inbyggda fält som är beräkningar.
* Du kan bara redigera fält som är direkt kopplade till objekten i listan. Du kan inte redigera fält som tillhör objekt som är kopplade till objekten i listan.\
   Du kan till exempel redigera status för en uppgift i en uppgiftsrapport, men du kan inte redigera namnet på projektet som uppgiften är kopplad till i samma rapport. Du kan bara redigera namnet på projektet i en projektrapport.
* Du kan inte infoga redigeringsfält när vyn för en lista inte visar standardvalutan.\
   Mer information om hur du visar standardvalutan finns i avsnittet [Redigera rapporter med unika valutor](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) i artikeln [Skapa rapporter om finansiella data med unika valutakurser](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* Du kan inte redigera flaggor och ikoner som visas i en lista.
* Du kan inte infoga redigeringsrapportfält som har hämtats från andra rapporter.

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
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Edit] behörighet till området som listan finns i</p> <p>Om du till exempel vill infoga redigeringsuppgifter i ett projekt måste du [!UICONTROL Edit] behörighet till projekt.</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå.<br>För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage]</p> <p>Du måste också ha behörighet att redigera vissa fält, t.ex. anpassade fält, status.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Redigera objekt textbundet

1. Gå till en lista med objekt som du vill redigera.

   Listan ska visa fält som tillhör de objekt eller fält som tillhör de objekt som är kopplade till objekten i listan.

1. Leta reda på objektet som du vill redigera och klicka sedan i ett fält i listan.

   >[!TIP]
   >
   >Om du har flera sidor kan du söka efter ett objekt med:
   >
   >   
   >   
   >   * **Sidnumrering**: Klicka på bakåt- och framåtpilarna för att navigera mellan sidorna.\
   >     längst ned till höger i listan, [!UICONTROL pagination] när du bläddrar igenom listan förblir området klisterlöst.
   >   * **Snabbfilter**: Klicka på filterikonen eller skriv Alt+F för att öppna snabbfiltret och ange sedan text för att endast visa objekt som innehåller den angivna texten.\
   >     Snabbfiltret finns i listverktygsfältet. Mer information finns i [Använda snabbfiltret på en lista](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).


   Om fältet kan redigeras blir fältet och alla andra fält som visas i listan redigerbara celler.

   ![](assets/nwe-editable-cells-350x131.png)

1. Redigera informationen i cellen och tryck sedan på [!UICONTROL Enter].

   >[!NOTE]
   >
   >Om ett anpassat fält har konfigurerats för att tillåta formatering kan du fet, kursiv eller understruken text när fältet redigeras i en uppdaterad lista.\
   >Information om hur du konfigurerar formatering för ett anpassat fält finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >Mer information om uppdaterade listor finns i avsnittet&quot;Skillnaden mellan de uppdaterade och de äldre listorna&quot; i artikeln [Kom igång med listor i [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Tryck [!UICONTROL Tab] för att gå till nästa redigerbara cell.
1. (Villkorligt) Om du inte kan spara redigeringarna och cellen visas med röda konturer, klickar du i fältet för att granska valideringsmeddelandet som visas bredvid cellen och gör lämpliga uppdateringar.

   Det här inträffar oftast när fel format används eller när ett obligatoriskt fält har lämnats tomt.

1. När du har ändrat alla celler trycker du på [!UICONTROL Enter] för att spara ändringarna.
