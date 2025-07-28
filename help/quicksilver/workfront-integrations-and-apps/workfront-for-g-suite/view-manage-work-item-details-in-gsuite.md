---
product-area: workfront-integrations;projects
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Visa och hantera  [!DNL Adobe Workfront] objektinformation från Google Workspace
description: Du kan visa och hantera information om en arbetsuppgift utan att behöva lämna Google Workspace. Du kan till exempel läsa en uppgifts beskrivning, visa dess överordnade objekt, ändra dess status och markera den som fullständig, allt inom [!DNL Adobe Workfront] för Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 0f15b05f-3b4a-4f0b-9d9a-21a0f97de1ea
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Visa och hantera information om [!DNL Adobe Workfront]-objekt från [!DNL Google Workspace]

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
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Google Workspace finns i [Gmail-moduler](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) och [Google Calendar-moduler](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Du kan visa och hantera information om en arbetsuppgift utan att lämna [!DNL Google Workspace]. Du kan till exempel läsa en uppgifts beskrivning, visa dess överordnade objekt, ändra dess status och markera den som fullständig, allt i [!DNL Adobe Workfront for Google Workspace].

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

Innan du kan visa och hantera information om arbetsobjekt i [!DNL Google Workspace] måste du

* Installera [!DNL Workfront for Google Workspace]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Visa och hantera information om arbetsobjekt i [!DNL Google Workspace]

1. Om panelen [!UICONTROL Workfront for Google Workspace] inte visas klickar du på ikonen [!DNL Workfront] ![Workfront ](assets/wf-lion-icon.png) i sidofältet för [!DNL Google Workspace]-tillägg längst till höger på sidan.
1. Gå till aktiviteten [!DNL Workfront] eller problemet i [!DNL Google Workspace], enligt beskrivningen i [Åtkomst [!DNL Adobe Workfront] [!UICONTROL Home] från  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md).

   När du väljer en uppgift eller ett problem öppnas fliken **[!UICONTROL Details]**. I området ovanför fliken **[!UICONTROL Details]** visas namnet på det överordnade objektet, namnet på uppgiften eller utgåvan och [!UICONTROL Due date] (om det är en uppgift) eller [!UICONTROL Priority date] (om det är ett problem).


   Du kan utföra olika åtgärder på den här fliken utan att lämna [!DNL Google Workspace], bland annat:

   * Visa objektets **[!UICONTROL Description]** och annan information, t.ex. vilka användare som har tilldelats objektet, **[!UICONTROL Priority]**, den som gjorde begäran, **[!UICONTROL Planned completion date]** samt anpassade fält och formulär som har kopplats till objektet.

     Anpassade formulär visar bara fält där information har lagts till.

   * Klicka i området **[!UICONTROL Parent project]** för att visa information om det överordnade objektet.

     >[!TIP]
     >
     >Detta kan vara praktiskt när du har uppgifter och problem med samma namn och behöver skilja ut dem.

   * Acceptera arbete som tilldelats dig genom att klicka på **[!UICONTROL Work on it]**.
   * Redigera olika alternativ, till exempel alternativet **[!UICONTROL Done]**, **[!UICONTROL Status]** och **[!UICONTROL Percent complete]**.

     Under **[!UICONTROL Percent complete]** anger du nummer och (valfritt) procenttecknet % för att ange förloppet för ett objekt.
   * Visa information om en godkännandebegäran, inklusive ägare, storlek och eventuella bilagor.
   * **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** godkännandebegäranden och dokument.

   * **[!UICONTROL Grant]** eller **[!UICONTROL Ignore]** åtkomstbegäranden.

1. (Valfritt) Klicka på **[!UICONTROL View in [!DNL Workfront]]** om du vill gå till den aktuella arbetsposten i [!DNL Workfront].

* Mer information om hur du använder fliken [!UICONTROL Updates] i [!DNL Workfront for Google Workspace] finns i [Uppdatera ett [!DNL Adobe Workfront] objekt från [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md).
* Mer information om hur du använder fliken [!UICONTROL Documents] i [!DNL Workfront for Google Workspace] finns i [Visa och hantera dokument från [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md).
