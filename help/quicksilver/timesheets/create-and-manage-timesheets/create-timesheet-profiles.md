---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Skapa, redigera och tilldela tidrapportprofiler
description: Du kan skapa, redigera och tilldela tidrapportprofiler som genererar återkommande tidrapporter för dina användare utan att du behöver göra något mer. Detta sparar tid och säkerställer enhetlighet mellan användarna.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 395a7788ddfda71264b7b964953435affd7761e9
workflow-type: tm+mt
source-wordcount: '1597'
ht-degree: 0%

---

# Skapa, redigera och tilldela tidrapportprofiler

<!--Audited: 06/2025-->

Du kan skapa, redigera och tilldela tidrapportprofiler som genererar återkommande tidrapporter för dina användare utan att du behöver göra något mer. Detta sparar tid och säkerställer att följande är konsekventa för användarna:

* Tidsram för tidrapport
* Godkännare
* Allmänna timtyper

Mer information om hur du skapar en tidrapport manuellt finns i [Skapa en tidrapport för engångsbruk](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard </p>
 <p>eller</p> 
<p>Aktuell: Planera </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha administrativ åtkomst till tidrapporter. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information om informationen i den här tabellen finns i [Åtkomstkraven i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa eller redigera en tidrapportprofil

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Om du vill aktivera ändringar av tidrapportprofilen i aktuella tidrapporter måste du ta bort de befintliga tidrapporterna innan du gör ändringarna i tidrapportprofilerna och sedan generera nya tidrapporter. Instruktioner finns i [Ta bort tidrapporter i Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) och [Generera tidrapporter manuellt](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Om du skapar eller redigerar en tidrapportprofil som ska användas i hela systemet klickar du på **Tidrapport och timmar**.

   eller

   Om du skapar eller redigerar en tidrapportprofil för en grupp klickar du på **Grupper** och sedan på gruppens namn.

1. Klicka på **Tidrapportprofiler**.
1. Om du vill skapa en tidrapportprofil klickar du på **Ny profil**.

   eller

   Om du vill redigera en befintlig tidrapportprofil markerar du den tidrapportprofil som du vill redigera och klickar sedan på **Redigera**.

   Den nya eller befintliga profilsidan för tidrapport visas.

1. Uppdatera följande information:

   * **Namn**: Lägg till ett namn för tidrapportprofilen. Det kan vara namnet på ett team eller en grupp vars personer delar samma tidsram för sina tidrapporter. Detta är ett obligatoriskt fält.
   * **Beskrivning**: Lägg till mer information om tidrapportprofilen.
   * **Grupp med administrationsåtkomst**: Om du skapar en tidrapportprofil på systemnivå lämnar du det här fältet tomt.

     Alla användare som kan redigera användarkonton kan bifoga en tidrapport på systemnivå till andra användare.

     Endast en Workfront-administratör kan redigera en tidrapportprofil på systemnivå.

     Identifiera gruppen här om du skapar en tidrapportprofil för en grupp som du administrerar.

     Detta tilldelar inte tidrapportprofilen till användarna i gruppen utan bara gruppens administratörer möjlighet att ändra tidrapportprofilen. Du tilldelar profilen till användare i steg 6.

     >[!NOTE]
     >
     >När användare utanför gruppen kopplar tidrapportprofiler till andra användare kan de inte se eller bifoga den här tidrapportprofilen.

   * **Skapa tidrapporter**: Ange när tidrapportprofilen ska generera tidrapporterna. En tidrapport kan ställas in så att den automatiskt genereras varje vecka, varannan vecka, halvår eller månad. Välj den veckodag då du vill att tidrapporten ska skapas.

     En veckotidrapport börjar det datum då den skapas. Om du t.ex. skapar veckotidrapporter varje torsdag är den första dagen i veckan på tidrapporten torsdag.

     >[!NOTE]
     >
     >Workfront skapar alltid två tidrapporter i taget: den första tidrapporten innehåller alltid det aktuella datumet och den andra tidrapporten startar när tidsramen för den första är slut.

   * **Godkännare**: Godkännare är användare som godkänner tidrapporten för användarna som är kopplade till tidrapporten. Du kan identifiera upp till 7 användare som godkännare på en tidrapport. Det är praktiskt att identifiera flera användare för att se till att en godkännare är tillgänglig när någon inte är på kontoret. Alla godkännare meddelas när en användare skickar tidrapporten för godkännande. Endast en användare behöver godkänna tidrapporten för att den ska godkännas.

     Endast användare med administratörsbehörighet för tidrapport kan anges som godkännare. Mer information om administratörsrättigheter för tidrapporter finns i [Bevilja användare administrativ åtkomst till vissa områden](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Använd listrutan för att välja godkännare för tidrapporten (om en godkännare krävs). Du kan välja mellan följande alternativ:

      * **Ingen**: Tidrapporten behöver inte godkännas.
      * **Deras hanterare**: Det här är standardgodkännaren som ställs in av systemet. I det här fallet godkänner den användare som är utsedd som sin chef tidrapporten när den skickas för godkännande.
      * **Specifika personer**: Du kan ange specifika användare efter namn som tidrapportgodkännare. Du kan ha flera godkännare på en tidrapport. När en av godkännarna har godkänt tidrapporten markeras tidrapporten som **Stängd** och försvinner från listan över tidrapportgodkännanden för alla återstående godkännare.

   * **Kan redigera tid**: Välj det här alternativet om du vill tillåta godkännarna att redigera timmar på tidrapporten.

     Det här alternativet fungerar tillsammans med inställningen **Begränsa redigering av tidrapporter till ägare och administratörer** i området Inställningar > Tidrapport och timmar > Inställningar. Mer information finns i [Konfigurera tidrapport och timinställningar](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     Följande scenarier finns:

     När alternativet **Begränsa redigering av tidrapport till ägare och administratörer** är aktiverat:

      * Godkännare kan bara godkänna och avvisa tidrapport, oavsett om knappen Kan redigera tid är aktiverad eller inte.
      * Tidrapportsägarnas chefer kan bara visa sina direkt rapporters tidrapporter.

     När alternativet **Begränsa redigering av tidrapport till ägare och administratörer** är inaktiverat:

      * När **Kan redigera tid** är aktiverat kan godkännare skicka, öppna igen eller stänga tidrapporten och redigera tiden.
      * När **Kan redigera tid** är inaktiverat kan godkännarna inte skicka, öppna igen eller stänga tidrapporten och kan inte redigera tiden. Godkännare kan bara godkänna eller avvisa tidrapporten.
      * Tidrapportsägarnas chefer kan skicka, återkalla, öppna och redigera sina direkt underställda tidrapporter.

     >[!NOTE]
     >
     >När du har skickat in en tidrapport för godkännande kan du inte längre redigera timmarna. Om du vill returnera en inskickad tidrapport till ett redigerbart tillstånd måste du återkalla tidrapporten eller låta godkännaren avvisa tidrapporten. Mer information finns i [Skicka en tidrapport för godkännande](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) och [Godkänn en tidrapport](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md).

   * **Övertid**: Du kan dölja rutan Övertid i tidrapporter. Det här alternativet är inaktiverat som standard.
   * **Tillgängliga timtyper**: Den här inställningen avser endast allmänna timtyper och inte projektspecifika timtyper.

     Som standard ser användare alla allmänna timmar på en tidrapport. Om din organisation bara vill att specifika allmänna timmar ska visas för en viss uppsättning användare, kan du välja de allmänna timmar som de behöver se i sina tidrapporter genom att markera dem i sin tidrapportprofil i det här fältet. Om du vill inaktivera alla allmänna timmar avmarkerar du alla timtyper för att generera tidrapporten utan ett avsnitt för allmänna timmar.

   * **Påminnelsemeddelanden**: Lägg till ett påminnelsemeddelande. Workfront skickar påminnelser till användare som ombeds att fylla i eller godkänna sina tidrapporter. Du måste skapa påminnelsemeddelanden innan du kan koppla dem till en tidrapportprofil.

1. Om du vill associera tidrapportprofilen med specifika användare, grupper eller (om du är Workfront-administratör) team bläddrar du mot sidans nederkant och hittar avsnittet **Tilldela personer**.

   Börja skriva namnet på användaren, gruppen eller teamet och klicka sedan på det när det visas i listrutan.

   <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   Om du är gruppadministratör kan du tilldela tidrapportprofilen till grupper som du administrerar, men inte till team. Mer information finns i [Begränsningar för en gruppadministratör som tilldelar en tidrapportprofil](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) i den här artikeln.

   >[!NOTE]
   >
   >* Du kan även associera en användare med en tidrapportprofil genom att redigera användarprofilen. Mer information finns i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* När du lägger till en grupp visas bara gruppnamnet på fliken Tilldela personer, inte på listan med gruppmedlemmar. Om du vill visa gruppmedlemmarna som listas här klickar du på Spara ändringar och sedan på namnet på den tidrapportprofil som du just skapade.
   >* När du är klar med de här stegen genererar tidrapportprofilen endast tidrapporter för de tilldelade användarna eller gruppmedlemmarna som inte har några befintliga tidrapporter för den aktuella perioden.

1. Klicka på **Spara**.

1. Klicka på ikonen **Mer** ![Mer](assets/more-icon.png) överst i listan över tidrapportprofiler och klicka sedan på **Generera tidrapporter**.

   En bekräftelse visas längst ned på skärmen om att tidrapporterna har skapats. Nya tidrapporter genereras baserat på de nya profiler du har skapat.

   Mer information finns i [Generera tidrapporter manuellt](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   Första gången som tidrapportprofilen genererar tidrapporter skapas två tidrapporter för varje användare, både för den tidsram som innehåller den aktuella tiden och för nästa tidsram.

   Därefter skapas en tidrapport per användare varje gång nya tidrapporter skapas.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Begränsningar för en gruppadministratör som tilldelar en tidrapportprofil {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Om du är gruppadministratör och det administrativa åtkomstalternativet Tidrapporter och timmar är inaktiverat på din åtkomstnivå kan du skapa tidrapportprofiler, men du kan bara tilldela dem till:

* Grupper som du administrerar
* Enskilda användare som du har behörighet att redigera och som finns i en grupp som du administrerar

För dessa grupper och användare har du inte tillgång till de tidrapporter som tidrapportprofilen genererar.

Om alternativet Användaradministratör (gruppanvändare) också är inaktiverat på din åtkomstnivå kan du tilldela tidrapportprofilen till en grupp som du administrerar, men det påverkar bara de användare i gruppen som du har behörighet att redigera. Om gruppen innehåller användare som du inte har behörighet att redigera tilldelas de inte tidrapportprofilen tillsammans med resten av gruppen.

Information om alternativet Tidrapporter och timmar på din åtkomstnivå finns i [Bevilja användare administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Mer information om alternativet Användaradministratör (gruppanvändare) på din åtkomstnivå finns i [Bevilja åtkomst till användare](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Flera återkommande tidrapportprofiler

Du kan ha fler än en tidrapportprofil för din organisation om det finns:

* Unika löneperioder för olika användaruppsättningar
* Unika godkännare för olika användaruppsättningar
* Unika allmänna timmeskrav för olika användaruppsättningar

En användare kan inte associeras med mer än en tidrapportprofil åt gången.

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->