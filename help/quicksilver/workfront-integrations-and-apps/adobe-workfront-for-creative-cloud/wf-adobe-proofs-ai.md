---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Ladda upp korrektur från Illustrator
description: Du kan ladda upp ritytorna som dokument för snabb granskning och godkännande eller helt enkelt lagra dem i Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: e98f27d4-7c07-44cc-8df5-e04472ec946e
source-git-commit: 66186bb8af14e7ce86b3fb5e8bb1b07fe32dca7a
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# Överför korrektur från [!DNL Illustrator]

Du kan ladda upp ritytorna som korrektur direkt till [!DNL Adobe Workfront] för en grundlig granskning och godkännande.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Aktuell plan: [!UICONTROL Pro] eller högre</p> <p>eller</p> <p>Äldre plan: [!UICONTROL Premium]</p> <p>Mer information om åtkomst till korrektur med olika planer finns i .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>Aktuell plan: [!UICONTROL Work] eller [!UICONTROL Proof]</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha en [!DNL Adobe Creative Cloud] utöver en [!DNL Workfront] licens.</td> 
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

&#42;Om du vill veta vilken plan, roll eller behörighetsprofil för korrektur du har kontaktar du [!DNL Workfront] eller [!DNL Workfront Proof] administratör.

## Förutsättningar

* Du måste installera [!DNL Adobe Workfront for design and video] innan du kan ladda upp korrektur från [!DNL Illustrator].

  Instruktioner finns i [Installera [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Överför ett grundläggande korrektur

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Gå till arbetsuppgiften där du vill överföra ett korrektur.
1. Klicka på **[!UICONTROL Document]** icon ![](assets/documents.png) i navigeringsfältet.
1. Klicka **[!UICONTROL New File]** nära plug-ins nederkant.
1. Aktivera **[!UICONTROL Create a proof]** växla.
1. (Valfritt) Skriv ett namn på korrekturet i dialogrutan **[!UICONTROL Proof Name]** textruta.
1. I **[!UICONTROL Proof Approvals]** avsnitt, markera **[!UICONTROL Basic]**.
1. (Valfritt) Lägg till godkännare.
1. (Valfritt) Skriv en kommentar i **[!UICONTROL Updates]** område.

   ![](assets/add-comment.png)

1. Välj **[!UICONTROL Asset Type]** i listrutan.

1. (Valfritt) Välj **[!UICONTROL Add outside file]** för att lägga till en fil från datorn.
1. Klicka **[!UICONTROL Upload]** konfigurerar du önskade exportalternativ baserat på den resurstyp som valts ovan.

   ![](assets/plugin-files-350x307.png)\
   Dokumentet visas i [!UICONTROL Documents] i plugin-programmet och datorprogrammet.


## Överför ett automatiskt korrektur

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Gå till arbetsuppgiften där du vill överföra ett korrektur.
1. Klicka på **[!UICONTROL Document]** icon ![](assets/documents.png) i navigeringsfältet.

1. Klicka **[!UICONTROL New File]** nära plug-ins nederkant.
1. Aktivera **[!UICONTROL Create a proof]** växla.
1. (Valfritt) Skriv ett namn på korrekturet i dialogrutan **[!UICONTROL Proof Name]** textruta.
1. I **[!UICONTROL Proof Approvals]** avsnitt, markera **[!UICONTROL Automated]**.
1. (Valfritt) I dialogrutan **[!UICONTROL Workflow Template]** anger du namnet på en korrekturarbetsflödesmall.

{{adjust-proof-settings}}

>[!NOTE]
>
> Om det finns tomma obligatoriska fält i arbetsflödesmallen öppnas de automatiska korrekturinställningarna automatiskt och du måste fylla i fälten för att kunna överföra korrekturet.


1. (Valfritt) Skriv en kommentar i **[!UICONTROL Updates]** område.

   ![](assets/add-comment-automated-approval.png)

1. Välj **[!UICONTROL Asset Type]** i listrutan.
1. (Valfritt) Välj **[!UICONTROL Add outside file]** för att lägga till en fil från datorn.
1. Klicka **[!UICONTROL Upload]**konfigurerar du önskade exportalternativ baserat på den resurstyp som valts ovan.
Dokumentet visas i [!UICONTROL Documents] i plugin-programmet och datorprogrammet.

## Överför en ny korrekturversion

Du kan överföra en ny version av ett korrektur. Plugin-programmet kommer ihåg det korrekturinställda arbetsflödet som angetts i den tidigare versionen, men du kan ändra det om du vill.

1. Klicka på **[!UICONTROL Menu]** ikonen i det övre högra hörnet och välj **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![](assets/go-back-to-work-list-350x314.png)

1. Gå till den arbetsuppgift som du behöver överföra ett dokument till.
1. Klicka på **[!UICONTROL Document]** icon ![](assets/documents.png)i navigeringsfältet.

1. Klicka **[!UICONTROL New Version]** nära plug-ins nederkant.
1. Aktivera **[!UICONTROL Create a proof]** växla.

1. I *[!UICONTROL *Proof approvals]** väljer du **[!UICONTROL Basic]** eller **[!UICONTROL Automated]**.

1. Lägg till **[!UICONTROL Reviewers]** eller en **[!UICONTROL Workflow template]** baserat på den godkännandetyp du valde i steg 7.

1. (Valfritt) Skriv en kommentar i **[!UICONTROL Updates]** område.
1. Välj **[!UICONTROL Asset Type]** i listrutan.
1. Klicka **[!UICONTROL Upload]**konfigurerar du önskade exportalternativ baserat på den resurstyp som valts ovan.
Dokumentet visas i [!UICONTROL Documents] i plugin-programmet och datorprogrammet.
