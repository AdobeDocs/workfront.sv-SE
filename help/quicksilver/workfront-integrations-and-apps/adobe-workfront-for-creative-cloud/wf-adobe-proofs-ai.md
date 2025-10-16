---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Ladda upp korrektur från Illustrator
description: Du kan ladda upp ritytorna som dokument för snabb granskning och godkännande eller helt enkelt lagra dem i Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: e98f27d4-7c07-44cc-8df5-e04472ec946e
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---

# Överför korrektur från [!DNL Illustrator]

Du kan överföra dina ritytor som korrektur direkt till [!DNL Adobe Workfront] för en grundlig granskning och godkännande.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Standard</p> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha en [!DNL Adobe Creative Cloud]-licens förutom en [!DNL Workfront]-licens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>[!UICONTROL Manager] eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till [!UICONTROL Documents]</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

* Du måste installera [!DNL Adobe Workfront for design and video] innan du kan överföra korrektur från [!DNL Illustrator].

  Instruktioner finns i [Installera [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Överför ett grundläggande korrektur

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Gå till arbetsuppgiften där du vill överföra ett korrektur.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument &#x200B;](assets/documents.png) i navigeringsfältet.
1. Klicka på **[!UICONTROL New File]** längst ned i plugin-programmet.
1. Aktivera växlingsknappen **[!UICONTROL Create a proof]**.
1. (Valfritt) Skriv ett namn på korrekturet i textrutan **[!UICONTROL Proof Name]**.
1. Välj **[!UICONTROL Proof Approvals]** i avsnittet **[!UICONTROL Basic]**.
1. (Valfritt) Lägg till godkännare.
1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

   ![Lägg till en kommentar](assets/add-comment.png)

1. Välj **[!UICONTROL Asset Type]** i listrutan.

1. (Valfritt) Välj **[!UICONTROL Add outside file]** om du vill lägga till en fil från datorn.
1. Klicka på **[!UICONTROL Upload]** och konfigurera sedan önskade exportalternativ baserat på den resurstyp som valts ovan.

   ![Filer i plugin-programmet](assets/plugin-files-350x307.png)\
   Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.


## Överför ett automatiskt korrektur

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Gå till arbetsuppgiften där du vill överföra ett korrektur.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument &#x200B;](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New File]** längst ned i plugin-programmet.
1. Aktivera växlingsknappen **[!UICONTROL Create a proof]**.
1. (Valfritt) Skriv ett namn på korrekturet i textrutan **[!UICONTROL Proof Name]**.
1. Välj **[!UICONTROL Proof Approvals]** i avsnittet **[!UICONTROL Automated]**.
1. (Valfritt) Skriv namnet på en korrekturarbetsflödesmall i rutan **[!UICONTROL Workflow Template]**.

{{adjust-proof-settings}}

>[!NOTE]
>
> Om det finns tomma obligatoriska fält i arbetsflödesmallen öppnas de automatiska korrekturinställningarna automatiskt och du måste fylla i fälten för att kunna överföra korrekturet.


1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

   ![Lägg till kommentar i automatiskt godkännande](assets/add-comment-automated-approval.png)

1. Välj **[!UICONTROL Asset Type]** i listrutan.
1. (Valfritt) Välj **[!UICONTROL Add outside file]** om du vill lägga till en fil från datorn.
1. Klicka på **[!UICONTROL Upload]** och konfigurera sedan önskade exportalternativ baserat på den resurstyp som valts ovan.
Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.

## Överför en ny korrekturversion

Du kan överföra en ny version av ett korrektur. Plugin-programmet kommer ihåg det korrekturinställda arbetsflödet som angetts i den tidigare versionen, men du kan ändra det om du vill.

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Gå till den arbetsuppgift som du behöver överföra ett dokument till.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument &#x200B;](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New Version]** längst ned i plugin-programmet.
1. Aktivera växlingsknappen **[!UICONTROL Create a proof]**.

1. Välj *[!UICONTROL *Proof approvals]* eller **[!UICONTROL Basic]** i avsnittet **[!UICONTROL Automated]***.

1. Lägg till **[!UICONTROL Reviewers]** eller en **[!UICONTROL Workflow template]** baserat på den godkännandetyp som du valde i steg 7.

1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.
1. Välj **[!UICONTROL Asset Type]** i listrutan.
1. Klicka på **[!UICONTROL Upload]** och konfigurera sedan önskade exportalternativ baserat på den resurstyp som valts ovan.
Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.
