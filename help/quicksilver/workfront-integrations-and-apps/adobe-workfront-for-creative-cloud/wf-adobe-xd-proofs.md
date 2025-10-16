---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Ladda upp ritytor från XD som korrektur till Workfront
description: Du kan överföra ritytorna som korrektur direkt till Adobe Workfront för granskning och godkännande.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---

# Överför [!DNL XD] ritytor som korrektur till [!DNL Workfront]

Du kan överföra dina ritytor som korrektur direkt till [!DNL Adobe Workfront] för en grundlig granskning och godkännande.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td>Alla </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Standard</p> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ytterligare produkter</td> 
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

* Du måste installera plugin-programmet [!DNL Adobe Workfront for XD] innan du kan överföra korrektur i [!DNL Adobe XD].

  Instruktioner finns i [Installera [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Överför ett statiskt korrektur

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Menyikon](assets/menu-350x440.png)

1. Gå till arbetsuppgiften där du vill överföra ett statiskt korrektur.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument ](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New File]** längst ned i plugin-programmet.
1. Markera de ritytor som du vill överföra.

   >[!TIP]
   >
   >* Ritytorna visas i korrekturet i den ordning som de markerats. Den första markerade ritytan blir den första sidan i korrekturet och så vidare.
   >* Om du snabbt vill markera flera ritytor klickar du och drar musen över de ritytor du vill använda. Det gör att du inte kan styra ordningen på ritytorna i korrekturet.

1. Aktivera **[!UICONTROL Create a Proof]**.

1. Ge korrekturet ett namn.

1. Välj vilken typ av korrekturgodkännande du vill ha:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>De grundläggande godkännandeprocesserna är tillfälliga och kan omfatta olika granskare efter behov: </p> 
       <ul> 
        <li> <p>(Valfritt) Lägg till <strong>godkännare</strong> i rutan.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Automatiska godkännandeprocesser är färdiga av administratörer och innehåller specifika granskare och faser. Mer information finns i <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Översikt över automatiserat arbetsflöde</a>.</p> 
       <ul> 
        <li> <p>Välj en [!UICONTROL Workflow Template] i listrutan.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

   ![Bevis på godkännanden i XD](assets/proof-approvals-xd-350x396.png)

1. Välj exportformat i listrutan **[!UICONTROL Asset Type]**.


1. (Valfritt) Om du väljer PDF som resurstyp och har markerat mer än en rityta väljer du om du vill exportera ritytorna som **[!UICONTROL Single PDF file]s** eller **M[!UICONTROL ultiple PDF files]**.

1. (Valfritt) Ge PDF ett namn.

   ![PDF-alternativ](assets/pdf-options.png)

1. Klicka på **[!UICONTROL Upload]**.\
   Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.

## Överför ett interaktivt korrektur {#upload-an-interactive-proof}

Du kan skapa ett interaktivt korrektur för ritytorna med plugin-programmet [!DNL Workfront for Adobe]. Det är en tvåstegsprocess. Först måste du skapa en interaktiv länk, sedan måste du överföra korrekturet till en arbetsuppgift.

### Skapa en interaktiv länk för ritytan  {#create-an-interactive-link-for-your-art-board}

1. Öppna ritytan och klicka sedan på **[!UICONTROL Share]** i skärmens övre vänstra del.
1. Ange länkinställningarna:

   1. Namnge länken.
   1. Välj en visningsinställning.
   1. Kontrollera att **[!UICONTROL Link Access]** är markerat i avsnittet **[!UICONTROL Anyone with this link]**.

      Du måste aktivera den här typen av åtkomst för att kunna generera ett interaktivt korrektur.

   1. Klicka på **[!UICONTROL Create Link]**.

1. Klicka tillbaka till **[!UICONTROL Design]** i skärmens övre vänstra del. Fortsätt till avsnittet [Överför ett interaktivt korrektur](#upload-an-interactive-proof) nedan.

   >[!NOTE]
   >
   >Du kan behöva öppna plugin-panelen igen i det nedre vänstra hörnet av skärmen.

### Överför ett interaktivt korrektur

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Menyikon](assets/menu-350x440.png)

1. Gå till arbetsuppgiften där du vill ladda upp ett interaktivt korrektur.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument ](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New File]** längst ned i plugin-programmet.
1. Aktivera **[!UICONTROL Create a Proof]**.

1. Välj vilken typ av korrekturgodkännande du vill ha:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>De grundläggande godkännandeprocesserna är tillfälliga och kan omfatta olika granskare efter behov: </p> 
       <ul> 
        <li> <p>(Valfritt) Lägg till <strong>godkännare</strong> i rutan.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Automatiska godkännandeprocesser är färdiga av administratörer och innehåller specifika granskare och faser. Mer information finns i <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Översikt över automatiserat arbetsflöde</a>.</p> 
       <ul> 
        <li> <p>Välj en [!UICONTROL Workflow Template] i listrutan.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

   ![Bevis på godkännanden i XD](assets/proof-approvals-xd-350x396.png)

1. I listrutan **[!UICONTROL Asset Type]** väljer du länken som du nyss skapade på fliken **Delade länkar**. Mer information finns i [Skapa en interaktiv länk för ritytan](#create-an-interactive-link-for-your-artboard).\
   ![Delade länkar i XDS](assets/shared-links-xd-350x870.png)

1. Klicka på **[!UICONTROL Upload]**.

   Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.

   >[!IMPORTANT]
   >
   >Användarna måste ha tillgång till [!UICONTROL Desktop Proofing Viewer] för att kunna granska och godkänna interaktiva korrektur. Mer information finns i [Installera [!UICONTROL Desktop Proofing Viewer]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Överför en ny korrekturversion

Du kan överföra en ny version av ett korrektur. Plugin-programmet kommer ihåg det korrekturinställda arbetsflödet som angetts i den tidigare versionen, men du kan ändra det om du vill.

1. Klicka på ikonen **[!UICONTROL Menu]** i det övre högra hörnet och välj sedan **[!UICONTROL Work List]**. Du kan också använda menyn för att navigera till överordnade objekt.

   ![Menyikon](assets/menu-350x440.png)

1. Gå till den arbetsuppgift som du behöver överföra ett dokument till.
1. Klicka på ikonen **[!UICONTROL Document]** ![Dokument ](assets/documents.png) i navigeringsfältet.

1. Klicka på **[!UICONTROL New Version]** längst ned i plugin-programmet.
1. Aktivera **[!UICONTROL Create a Proof]**.
1. Markera de ritytor som du vill överföra.

   >[!NOTE]
   >
   >Om du vill överföra en ny version av en svg-, png- eller jpg-fil kan du bara överföra en rityta.

1. Välj vilken typ av korrekturgodkännande du vill ha:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>De grundläggande godkännandeprocesserna är tillfälliga och kan omfatta olika granskare efter behov: </p> 
       <ul> 
        <li> <p>(Valfritt) Lägg till <strong>godkännare</strong> i rutan.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Automatiska godkännandeprocesser är färdiga av administratörer och innehåller specifika granskare och faser. Mer information finns i <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Översikt över automatiserat arbetsflöde</a>.</p> 
       <ul> 
        <li> <p>Välj en [!UICONTROL Workflow Template] i listrutan.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Välj exportformat i listrutan **[!UICONTROL Asset Type]**.

   ![Skapa ett korrektur i XD](assets/create-a-proof-xd-350x202.png)

1. (Valfritt) Skriv en kommentar i området **[!UICONTROL Updates]**.

   ![Bevis på godkännanden i XD](assets/proof-approvals-xd-350x396.png)

1. (Valfritt) Om du väljer PDF som resurstyp och har markerat mer än en rityta väljer du om du vill exportera ritytorna som **[!UICONTROL Single PDF file]s** eller **M[!UICONTROL ultiple PDF files]**.

1. (Valfritt) Ge PDF ett namn.

   PDF-alternativ

1. Klicka på **[!UICONTROL Upload]**.\
   Dokumentet visas i området [!UICONTROL Documents] i plugin-programmet och skrivbordsappen.
