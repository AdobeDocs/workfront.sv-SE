---
product-area: workfront-integrations
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Få åtkomst till [!DNL Adobe Workfront] heminnehåll från Google Workspace
description: Du kan komma åt ditt [!DNL Adobe Workfront] Home-innehåll, inklusive alla uppgifter, utgåvor, godkännanden och åtkomstbegäranden som tilldelats dig, utan att lämna Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: da2ecaf1-5cfb-470e-90a1-fbb386db8670
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Åtkomst till [!DNL Adobe Workfront] [!UICONTROL Home]-innehåll från [!DNL Google Workspace]

>[!NOTE]
>
>Den senaste versionen av Adobe Workfront-pluginprogrammet för Google släpptes den 26 juni 2023.

Du kan komma åt ditt [!DNL Adobe Workfront] [!UICONTROL Home]-innehåll, inklusive alla uppgifter, ärenden, godkännanden och åtkomstbegäranden som tilldelats dig, utan att lämna Google Workspace.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du kan komma åt [!UICONTROL Home]-innehåll från [!DNL Google Workspace] måste du

* Installera [!DNL Workfront for Google Workspace]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Åtkomst till [!DNL Workfront] [!UICONTROL Home] från [!DNL Google Workspace]

1. Kontrollera att du är inloggad på [!DNL Workfront].
1. Om panelen [!UICONTROL Workfront for Google Workspace] inte visas klickar du på ikonen [!DNL Workfront] ![Workfront ](assets/wf-lion-icon.png) i sidofältet för [!DNL Google Workspace]-tillägg längst till höger på sidan.
1. Om du ser en vänsterpil högst upp i [!DNL Workfront] för [!DNL Google Workspace] klickar du på pilen för att gå till området [!UICONTROL Home].

1. Klicka på den expanderade pilen ![Expandera pil](assets/dropdown-arrow.png) i området **[!UICONTROL Sort by]** och klicka sedan på ett alternativ för att ange hur du vill gruppera dina arbetsobjekt så att du kan hitta det du söker.

   När du sorterar efter **[!UICONTROL Commit date]** eller **[!UICONTROL Planned completion]** datum är de äldsta arbetsobjekten högst upp.

   När du sorterar efter **[!UICONTROL Project]** visas arbetsobjekt i ordningen för deras överordnade projekt, i bokstavsordning från A till Z. Arbetsobjekt utan ett överordnat projekt visas under **[!UICONTROL No Project]**.

1. Klicka på den expanderade pilen ![Expandera pil](assets/dropdown-arrow.png) för den gruppering som du vill visa.

   Antalet objekt i varje grupp visas inom parentes. När du klickar på pilen [!UICONTROL expand] visas alla arbetsobjekt i gruppen.

   Arbetsobjekt visas enligt följande:

   * ![Aktivitetsikonen](assets/task-icon.png) **Aktiviteter** visar det överordnade projektnamnet, aktivitetsnamnet och planerat slutförandedatum.

   * ![Utfärdningsikonen](assets/issue-icon.png) **Problem** visar det överordnade projektnamnet, namnet på utgåvan och datumet för det planerade slutförandet.

   * ![Dokumentikonen](assets/document-icon.png) **Godkännanden** visar den sökandes namn, dokumentnamn och överföringsdatum.
   * **Åtkomstbegäranden** visar den begärandes namn, objektnamn och överföringsdatum. Ikonen för objekttypen visas till vänster.

1. Klicka var som helst på en arbetsuppgift för att se information, uppdateringar och dokument.
