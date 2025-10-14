---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Ladda upp korrektur från Adobe Photoshop
description: Du kan överföra förinställningar för fotodokument som korrektur direkt till  [!DNL Adobe Workfront] för en grundlig granskning och godkännande.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: 9cbf1706e6c535ff7f52627d2c6e13de65ec76d0
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 0%

---

# Överför korrektur från [!DNL Photoshop]

Du kan överföra vissa förinställningstyper för Photoshop-dokument som korrektur direkt till [!DNL Adobe Workfront] för en grundlig granskning och godkännande.

>[!IMPORTANT]
>
>Filen måste vara en fotodokumentförinställning enligt beskrivningen i [Mallar och förinställningar i Photoshop](https://helpx.adobe.com/se/photoshop/using/create-documents.html).



## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td>Du måste ha en [!DNL Adobe Creative Cloud]-licens förutom en [!DNL Workfront]-licens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>[!UICONTROL Manager] eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till [!UICONTROL Documents]</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Förutsättningar

* Du måste installera [!DNL Adobe Workfront for Photoshop] innan du kan överföra korrektur från [!DNL Adobe Photoshop].

  Instruktioner finns i [Installera [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Överför ett grundläggande korrektur

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Gå till arbetsuppgiften där du vill överföra ett korrektur.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument &#x200B;](assets/documents.png) i navigeringsfältet.
1. Klicka på **[!UICONTROL New File]** längst ned på panelen [!DNL Workfront].
1. Aktivera växlingsknappen **[!UICONTROL Create a proof]**.
1. (Valfritt) Skriv ett namn på korrekturet i textrutan **[!UICONTROL Proof Name]**.
1. Välj **[!UICONTROL Basic]** i avsnittet **[!UICONTROL Proof Approvals]**.
1. (Valfritt) Lägg till godkännare.
1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

   ![Lägg till en kommentar](assets/add-comment.png)

1. Välj **[!UICONTROL Asset Type]** i listrutan.

1. (Valfritt) Välj **[!UICONTROL Add outside file]** om du vill lägga till en fil från datorn.
1. Klicka på **[!UICONTROL Upload]** och konfigurera sedan önskade exportalternativ baserat på den resurstyp som valts ovan.

   ![Filer i plugin-programmet](assets/plugin-files-350x307.png)\
   Dokumentet visas i området [!UICONTROL Documents] på panelen [!DNL Workfront] i [!DNL Photoshop] och i skrivbordsappen [!DNL Workfront].


## Överför ett automatiskt korrektur

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Gå till arbetsuppgiften där du vill överföra ett korrektur.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument &#x200B;](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New File]** längst ned på panelen [!DNL Workfront].
1. Aktivera växlingsknappen **[!UICONTROL Create a proof]**.
1. (Valfritt) Skriv ett namn på korrekturet i textrutan **[!UICONTROL Proof Name]**.
1. Välj **[!UICONTROL Automated]** i avsnittet **[!UICONTROL Proof Approvals]**.
1. (Valfritt) Skriv namnet på en korrekturarbetsflödesmall i rutan **[!UICONTROL Workflow Template]**.

{{adjust-proof-settings}}

>[!NOTE]
>
> Om det finns tomma obligatoriska fält i arbetsflödesmallen öppnas de automatiska korrekturinställningarna automatiskt och du måste fylla i fälten för att kunna överföra korrekturet.


1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

   ![Lägg till automatiskt godkännande av kommentar](assets/add-comment-automated-approval.png)

1. Välj **[!UICONTROL Asset Type]** i listrutan.
1. (Valfritt) Välj **[!UICONTROL Add outside file]** om du vill lägga till en fil från datorn.
1. Klicka på **[!UICONTROL Upload]** och konfigurera sedan önskade exportalternativ baserat på den resurstyp som valts ovan.
Dokumentet visas i området [!UICONTROL Documents] på panelen [!DNL Workfront] i [!DNL Photoshop] och i skrivbordsappen [!DNL Workfront].

## Överför en ny korrekturversion

Du kan överföra en ny version av ett korrektur. Plugin-programmet kommer ihåg det korrekturinställda arbetsflödet som angetts i den tidigare versionen, men du kan ändra det om du vill.

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Återgå till arbetslistan](assets/go-back-to-work-list-350x314.png)

1. Gå till den arbetsuppgift som du behöver överföra ett dokument till.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument &#x200B;](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New Version]** längst ned på panelen [!DNL Workfront].
1. Aktivera växlingsknappen **[!UICONTROL Create a proof]**.

1. Välj **[!UICONTROL Basic]** eller **[!UICONTROL Automated]** i avsnittet *[!UICONTROL *Proof approvals]**.

1. Lägg till **[!UICONTROL Reviewers]** eller en **[!UICONTROL Workflow template]** baserat på den godkännandetyp som du valde i steg 7.

1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.
1. Välj **[!UICONTROL Asset Type]** i listrutan.
1. Klicka på **[!UICONTROL Upload]** och konfigurera sedan önskade exportalternativ baserat på den resurstyp som valts ovan.
Dokumentet visas i området [!UICONTROL Documents] på panelen [!DNL Workfront] i [!DNL Photoshop] och i skrivbordsappen [!DNL Workfront].
