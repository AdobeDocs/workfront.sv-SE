---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Visa information om arbetsuppgift med Adobe Workfront plugin
description: Du kan visa information om projekt, uppgifter, problem och dokument från Adobe Creative Cloud-program.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: a53a716f-4faf-4ea7-a4fc-ad8d87634267
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Visa information om arbetsobjekt med plugin-programmet [!DNL Adobe Workfront]

Du kan visa information om projekt, aktiviteter, utgåvor och dokument från följande [!DNL Adobe Creative Cloud]-program:

{{cc-app-list}}

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td>Du måste ha en [!DNL Adobe Creative Cloud]-licens förutom en [!DNL Workfront]-licens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL View] behörighet till projekt, uppgifter eller ärenden</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till det objekt som du vill visa. </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

+++

## Förutsättningar

{{cc-install-prereq}}

## Visa information och anpassade formulärdata

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Markera den arbetsuppgift som du vill visa.

   >[!TIP]
   >
   >Använd ikonen **[!UICONTROL Menu]** för att gå till arbetsobjektets överordnade objekt.

1. Klicka på ikonen **[!UICONTROL Details]** ![Detaljer](assets/details.png) i navigeringsfältet för att visa:

   * [!UICONTROL Description]
   * [!UICONTROL Planned Completion Date]
   * [!UICONTROL Status]
   * [!UICONTROL Assigned to]
   * [!UICONTROL Project Owner] (endast projekt)
   * Anpassade formulärdata

## Visa dokumentinformation

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Markera den arbetsuppgift som du vill visa.

   >[!TIP]
   >
   >Använd ikonen **[!UICONTROL Menu]** för att gå till arbetsobjektets överordnade objekt.

1. Klicka på ikonen **[!UICONTROL Document]** ![&#x200B; Dokument &#x200B;](assets/documents.png) i navigeringsfältet och dubbelklicka sedan på ett dokument för att visa:

   * [!UICONTROL Description]
   * [!UICONTROL File Type]
   * [!UICONTROL Proof Status] (endast tillgängligt för korrektur)
   * [!UICONTROL Version]
   * [!UICONTROL Size]
   * Anpassade formulärdata

## Visa korrekturinformation

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Markera den arbetsuppgift som du vill visa.

   >[!TIP]
   >
   >Använd ikonen **[!UICONTROL Menu]** för att gå till arbetsobjektets överordnade objekt.

1. Klicka på ikonen **[!UICONTROL Document]** ![&#x200B; Dokument &#x200B;](assets/documents.png) i navigeringsfältet och dubbelklicka sedan på ett korrektur.

1. Klicka på pilikonen i det övre högra hörnet av miniatyrbilden för att öppna korrekturinformationen i [!DNL Workfront].

![öppna sidan med korrekturinformation i Workfront.](assets/go-to-proof-details.png)

## Visa status för ett bevis

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Markera den arbetsuppgift som du vill visa.

   >[!TIP]
   >
   >Använd ikonen **[!UICONTROL Menu]** för att gå till arbetsobjektets överordnade objekt.

1. Klicka på ikonen **[!UICONTROL Document]** ![&#x200B; Dokument &#x200B;](assets/documents.png) i navigeringsfältet och dubbelklicka sedan på ett korrektur.

1. Rulla längst ned för att visa korrekturets aktuella status. Mer information om skickade, öppnade, kommentarer, beslut (SOCD) finns i [Översikt över dokumentinformation](/help/quicksilver/documents/managing-documents/document-details-overview.md).

![Korrekturstatus](assets/proof-status.png)

## Visa underaktiviteter och ärenden

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Markera den arbetsuppgift som du vill visa.

   >[!TIP]
   >
   >Använd ikonen **[!UICONTROL Menu]** för att gå till arbetsobjektets överordnade objekt.

1. Klicka på ikonen **[!UICONTROL Issue]** ![Problem &#x200B;](assets/issues.png) eller **Underaktivitet** ![Underaktivitet](assets/subtasks.png).

1. Markera uppgiften eller problemet och klicka sedan på ikonen **[!UICONTROL Details]** ![Detaljer](assets/details.png) i navigeringsfältet för att visa:

   * [!UICONTROL Planned Completion Date]
   * [!UICONTROL Status]
   * [!UICONTROL Assigned to]
   * Anpassade formulärdata
