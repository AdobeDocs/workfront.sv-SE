---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Konfigurera tidrapport och timinställningar
description: Som  [!DNL Adobe Workfront] administratör kan du ange inställningar för tidrapporter och timmar i [!DNL Workfront] för att definiera vilka objekt tidrapporterna kan förifyllas med och vilka objekt användarna kan logga tid på.
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '1261'
ht-degree: 0%

---

# Konfigurera tidrapport och timinställningar

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Som [!DNL Adobe Workfront]-administratör kan du ange inställningar för tidrapporter och timmar i [!DNL Workfront] för att definiera vilka objekt tidrapporterna kan förifyllas med och vilka objekt användare kan logga tid på.

>[!IMPORTANT]
>
>Förutom de objekt som förifyller en tidrapport enligt villkoren som beskrivs i den här artikeln, visas följande objekt även på tidrapporter som standard:
>
>* Objekt som du loggade tid för under tidsramen i tidrapporten
>* Objekt som är fästa på tidrapporten
>* Objekt som du söker efter och lägger till manuellt i tidrapporten. Manuellt tillagda objekt fästs som standard.
>
>Mer information finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md) och [Översikt över tidrapporten](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).

Alla ändringar du gör i tidrapporter påverkar alla tidrapporter som skapas i framtiden.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Aktuell:[!UICONTROL Plan]</p>
   eller
   <p>Nytt: Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör.</p>  </td>
</tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ange inställningar för tidrapport och timme

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Timesheet & Hours]** > **[!UICONTROL Preferences]**.

   Sidan Inställningar för tidrapporter och timmar visas.

1. (Valfritt) I sökrutan **Systemtidrapporter och timinställningar** börjar du skriva namnet på en grupp och markerar den när den visas i listan.

   ![](assets/search-for-group-box-in-timesheets-preferences-page.png)

   Sidan Inställningar för tidrapport och timmar uppdateras med inställningarna för den valda gruppen. Inställningarna på systemnivå måste vara olåsta för att du ska kunna ändra inställningarna på gruppnivå. Mer information finns i avsnittet [Lås upp tidrapport och timinställningar för grupper](#unlock-timesheet-and-hour-preferences-for-groups) i den här artikeln.

1. Konfigurera något av följande alternativ i avsnittet **[!UICONTROL General preferences]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Log time for future dates]</td> 
      <td> <p>Tillåter användare att logga tid för framtida datum i hela systemet i:</p> 
       <ul> 
        <li>Projekt, uppgifter och problem där de har åtkomst till loggtiden</li> 
        <li>Deras tidrapporter som allmän tid</li> 
       </ul> <p>Detta är användbart när användare tänker vara borta från kontoret och vill logga in den tiden i förväg.</p> <p><b>OBS</b>:</p> 
       <p>Du kan inte hindra användare från att logga in på uppgifter eller problem som har stängts eller avbrutits. Du kan bara hindra användare från att logga in på fullständiga eller döda projekt. Vi rekommenderar att du använder filter i listor med uppgifter och problem för att utesluta de som har slutförts eller avbrutits från att vara synliga för användarna.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Assign Job Roles to hour entries manually]</td> 
      <td> <p>Tillåt användare att manuellt välja en jobbroll som tilldelats i deras användarprofil eller tilldelats till objektet.</p> <p><b>VIKTIGT</b>:  
        <ul> 
         <li>Om du inaktiverar den här inställningen efter att du har tilldelat jobbroller till timposter, måste användarna justera timmar som loggats under olika roller på fliken [!UICONTROL Hours] i projektet, aktiviteten eller problemet.</li> 
         <li>Om användaren inte har tilldelats någon jobbroll i sin profil och det finns en uppgift tilldelad som [!UICONTROL Task Owner] i dialogrutan [!UICONTROL Advanced Assignments], visas den jobbrollen när användaren loggar tid på uppgiften.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict timesheet editing to owners and administrators]</td> 
      <td> <p>Begränsa redigering till tidrapportägare och [!DNL Workfront] administratörer. När det här alternativet är inaktiverat kan tidrapporter även redigeras av:</p> 
       <ul> 
        <li> <p>Användare med administrativ åtkomst till tidrapporter och timmar på åtkomstnivå</p> </li> 
        <li> <p>Tidrapporten godkänner om"Kan redigera timmar" är aktiverat på tidrapporten</p> </li> 
        <li> <p>Chefen för tidrapportägaren</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict hour editing to owners and administrators]</td> 
      <td>Begränsa redigering till den användare som anger timmar och [!DNL Workfront] administratörer. Den här inställningen gäller för fliken [!UICONTROL Hours] i ett projekt eller i en timrapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurera något av följande alternativ i avsnittet **[!UICONTROL Where users can log time]**:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Directly on projects]</td>
        <td>Tillåter användare att logga tid på projektet (både på fliken [!UICONTROL Updates] och i tidrapporten). Om användare inte registrerar tid på projektnivå bör dessa alternativ vara avmarkerade.</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are complete]</td>
        <td>Tillåter användare att registrera tid i ett projekt som har markerats som slutfört. Om det här alternativet är inaktiverat kan användare inte registrera tid för det arbete de har slutfört i projekt med statusen [!UICONTROL Complete].</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are dead]</td>
        <td>När det här alternativet är aktiverat kan användare logga timmar i projekt med statusen [!UICONTROL Dead].</td>
    </tr>
   </table>

1. Konfigurera något av följande alternativ i avsnittet **[!UICONTROL Pre-populate timesheets]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Work that is within] &lt;antal veckor&gt; [!UICONTROL of the timesheet's work range]</td> 
      <td> <p>Definierar antalet veckor före och efter datumintervallet för tidrapporten som innehåller datum för uppgifter och ärenden som tilldelats användaren.</p> 
      <p>Standardinställningen är 1 vecka, och du kan utöka intervallet till 4 veckor.</p> 
      <p>Det innebär att tidrapporten är förifylld med uppgifter och ärenden som har datum var som helst mellan fyra veckor före datumintervallet i tidrapporten upp till fyra veckor efter datumintervallet i tidrapporten, om du väljer 4 veckor för intervallet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have been completed]</td> 
      <td>Om flera resurser vanligtvis tilldelas till en enskild uppgift rekommenderar vi den här inställningen. Detta innebär att när en resurs registrerar tid mot aktiviteten och markerar den som slutförd, kan de andra resurser som tilldelats aktiviteten fortfarande hitta uppgiften eller problemet i sin tidrapport för att registrera sina timmar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have Planned Dates in timesheet's date range]</td> 
      <td> <p>När det här alternativet är markerat innehåller tidrapporten uppgifter och utgåvor som har antingen ett planerat startdatum eller ett slutförandedatum som ligger inom datumintervallet för tidrapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tasks that have Projected Dates in timesheet's date range]</td> 
      <td> <p>När det här alternativet är markerat innehåller tidrapporten uppgifter som antingen har ett planerat startdatum eller ett slutförandedatum som ligger inom tidsramen för projektet, även om det planerade datumet för utleveransen eller uppgiften ligger utanför tidsintervallet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ange följande i avsnittet **[!UICONTROL Deleted projects, tasks, and issues]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> När projekt tas bort</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Keep logged time already added to timesheets as general time]</strong>: Om projektet återställs vid ett senare tillfälle finns tiden kvar på tidrapporten.</li> 
        <li><strong>[!UICONTROL Delete any logged time]</strong>: Om projektet återställs vid ett senare tillfälle återställs den tid som redan är loggad till projektet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">När uppgifter eller problem tas bort</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Move any logged time to the project]</strong> där uppgiften eller problemet finns: Om den här uppgiften eller problemet återställs senare, återstår tiden för projektet.<br></li> 
        <li> <p><strong>[!UICONTROL Delete any logged time]</strong>: Om uppgiften eller problemet återställs senare återställs loggad tid till uppgiften eller problemet.</p> <p>Mer detaljerad information om de här alternativen finns i <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configure affect] om timmar när ett objekt tas bort och återställs </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Save]**.

## Lås upp tidrapport och timinställningar för grupper

Grupper i organisationen kan behöva tidrapporter eller timinställningar som har konfigurerats på olika sätt för sina unika arbetsflöden. Du kan låsa upp inställningarna för alla grupper i hela organisationen så att de kan konfigurera dem själva.

När en inställning är olåst och en gruppadministratör ändrar den, påverkas tidrapportsägarna om gruppen är deras hemgrupp.

Mer information om hur en gruppadministratör konfigurerar tidrapport och timinställningar för en grupp finns i [Konfigurera tidrapport- och timinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>När en [!DNL Workfront]-administratör har låst upp en inställning på systemnivå kan alla gruppadministratörer konfigurera den och sedan låsa den för att se till att alla i gruppen och undergrupperna nedan använder samma konfiguration. Detta är parallellt med möjligheten för en [!DNL Workfront]-administratör att konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Lås eller lås upp en grupptidrapport och timinställning](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Så här låser du upp en projektinställning så att grupper kan konfigurera den:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Timesheets & Hours]** i den vänstra panelen och sedan på **[!UICONTROL Preferences]**.

1. Gör något av följande:

   * Om du vill att gruppadministratörer ska kunna konfigurera en inställning för sina grupper klickar du på **låset** för att låsa upp den. ![](assets/unlock-toggle-button.png)
   * Om du vill att alla grupper ska använda din konfiguration för en inställning måste du se till att växlingen är låst ![](assets/locked-preference-toggle.png) (detta är standardinställningen).

     >[!IMPORTANT]
     >
     >Vi rekommenderar att du kommunicerar med administratörer och användare i grupper i hela systemet för att säkerställa att alla behov beaktas när du konfigurerar en låst inställning.
     >
     >När du låser den ärvs konfigurationen för den av alla grupper i systemet. Om inställningen har låsts upp under en viss tid ersätter konfigurationen de som gruppadministratörer kan ha gjort.

1. Klicka på **[!UICONTROL Save]**.
