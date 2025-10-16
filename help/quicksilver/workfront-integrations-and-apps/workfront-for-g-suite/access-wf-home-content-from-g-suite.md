---
product-area: workfront-integrations
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Få åtkomst till [!DNL Adobe Workfront] heminnehåll från Google Workspace
description: Du kan komma åt ditt [!DNL Adobe Workfront] Home-innehåll, inklusive alla uppgifter, utgåvor, godkännanden och åtkomstbegäranden som tilldelats dig, utan att lämna Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: da2ecaf1-5cfb-470e-90a1-fbb386db8670
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Åtkomst till [!DNL Adobe Workfront] [!UICONTROL Home]-innehåll från [!DNL Google Workspace]

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Under den här övergångsprocessen kommer följande Workfront för Google Workspace-funktioner inte att vara tillgängliga efter **28 februari 2026**:
>
>* Åtkomst till Google Workspace-funktioner inifrån Workfront
>
>* Visa och hantera Workfront-uppgifter från Gmail eller Google Calendar-webbplatspanelen
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Google Workspace.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Google Workspace finns i [Gmail-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) och [Google Calendar-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Du kan komma åt ditt [!DNL Adobe Workfront] [!UICONTROL Home]-innehåll, inklusive alla uppgifter, ärenden, godkännanden och åtkomstbegäranden som tilldelats dig, utan att lämna Google Workspace.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p><p>Arbeta eller högre</p>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du kan komma åt [!UICONTROL Home]-innehåll från [!DNL Google Workspace] måste du

* Installera [!DNL Workfront for Google Workspace]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Åtkomst till [!DNL Workfront] [!UICONTROL Home] från [!DNL Google Workspace]

1. Kontrollera att du är inloggad på [!DNL Workfront].
1. Om panelen [!UICONTROL Workfront for Google Workspace] inte visas klickar du på ikonen [!DNL Workfront] ![Workfront ](assets/wf-lion-icon.png) i sidofältet för [!DNL Google Workspace]-tillägg längst till höger på sidan.
1. Om du ser en vänsterpil högst upp i [!DNL Workfront] för [!DNL Google Workspace] klickar du på pilen för att gå till området [!UICONTROL Home].

1. Klicka på den expanderade pilen **[!UICONTROL Sort by]** Expandera pil![ i området ](assets/dropdown-arrow.png) och klicka sedan på ett alternativ för att ange hur du vill gruppera dina arbetsobjekt så att du kan hitta det du söker.

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
