---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Visa information om arbetsuppgift med Adobe Workfront plugin
description: Du kan visa information om projekt, uppgifter, problem och dokument från Adobe Creative Cloud-program.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: a53a716f-4faf-4ea7-a4fc-ad8d87634267
source-git-commit: fc3eb30cef2e17524b5cbd50219861f293a2ea9d
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Visa information om arbetsuppgift med [!DNL Adobe Workfront] plugin

Du kan visa information om projekt, uppgifter, ärenden och dokument från följande [!DNL Adobe Creative Cloud] program:

{{cc-app-list}}

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <!--<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha en [!DNL Adobe Creative Cloud] utöver en [!DNL Workfront] licens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL View] behörighet till projekt, uppgifter eller ärenden</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till det objekt som du vill visa. </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

{{cc-install-prereq}}

## Visa information och anpassade formulärdata

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Markera arbetsposten som du vill visa.

   >[!TIP]
   >
   >Använd **[!UICONTROL Menu]** om du vill gå till det överordnade objektet för arbetsposten.

1. Klicka på **[!UICONTROL Details]** icon ![](assets/details.png) i navigeringsfältet för att visa:

   * [!UICONTROL Description]
   * [!UICONTROL Planned Completion Date]
   * [!UICONTROL Status]
   * [!UICONTROL Assigned to]
   * [!UICONTROL Project Owner] (Endast projekt)
   * Anpassade formulärdata

## Visa dokumentinformation

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Markera arbetsposten som du vill visa.

   >[!TIP]
   >
   >Använd **[!UICONTROL Menu]** om du vill gå till det överordnade objektet för arbetsposten.

1. Klicka på **[!UICONTROL Document]** icon ![](assets/documents.png) i navigeringsfältet dubbelklickar du på ett dokument för att visa:

   * [!UICONTROL Description]
   * [!UICONTROL File Type]
   * [!UICONTROL Proof Status] (endast tillgängligt för korrektur)
   * [!UICONTROL Version]
   * [!UICONTROL Size]
   * Anpassade formulärdata

## Visa korrekturinformation

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Markera arbetsposten som du vill visa.

   >[!TIP]
   >
   >Använd **[!UICONTROL Menu]** om du vill gå till det överordnade objektet för arbetsposten.

1. Klicka på **[!UICONTROL Document]** icon ![](assets/documents.png) dubbelklicka på ett korrektur i navigeringsfältet.

1. Klicka på pilikonen i miniatyrbildens övre högra hörn för att öppna korrekturinformationen i [!DNL Workfront].

![öppna sidan med korrekturinformation i Workfront.](assets/go-to-proof-details.png)

## Visa status för ett korrektur

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Markera arbetsposten som du vill visa.

   >[!TIP]
   >
   >Använd **[!UICONTROL Menu]** om du vill gå till det överordnade objektet för arbetsposten.

1. Klicka på **[!UICONTROL Document]** icon ![](assets/documents.png) dubbelklicka på ett korrektur i navigeringsfältet.

1. Rulla längst ned för att visa korrekturets aktuella status. Mer information om Skickat, Öppnat, Kommentar, Beslut (SOCD) finns i [Översikt över dokumentinformation](/help/quicksilver/documents/managing-documents/document-details-overview.md).

![](assets/proof-status.png)

## Visa underaktiviteter och ärenden

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Markera arbetsposten som du vill visa.

   >[!TIP]
   >
   >Använd **[!UICONTROL Menu]** om du vill gå till det överordnade objektet för arbetsposten.

1. Klicka på **[!UICONTROL Issue]** icon ![](assets/issues.png) eller **Underuppgift** icon ![](assets/subtasks.png).

1. Välj uppgift eller problem och klicka sedan på **[!UICONTROL Details]** icon ![](assets/details.png) i navigeringsfältet för att visa:

   * [!UICONTROL Planned Completion Date]
   * [!UICONTROL Status]
   * [!UICONTROL Assigned to]
   * Anpassade formulärdata
