---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Skapa, redigera och tilldela tidrapportprofiler
description: Du kan skapa, redigera och tilldela tidrapportprofiler som genererar återkommande tidrapporter för dina användare utan att du behöver göra något mer. Detta sparar tid och säkerställer enhetlighet mellan användarna.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 939407f56b39617441f669d11b9439e445ceaf6e
workflow-type: tm+mt
source-wordcount: '1641'
ht-degree: 0%

---

# Skapa, redigera och tilldela tidrapportprofiler

{{highlighted-preview}}

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

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Namn</strong> </td> 
      <td> <p> Lägg till ett namn för tidrapportprofilen. Det kan vara namnet på ett team eller en grupp vars personer delar samma tidsram för sina tidrapporter. </p> <p>Detta är ett obligatoriskt fält.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td> <p> Lägg till mer information om tidrapportprofilen.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Gruppera med administrationsåtkomst</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Om du skapar en tidrapportprofil på systemnivå lämnar du det här fältet tomt.</p> <p>Alla användare som kan redigera användarkonton kan bifoga en tidrapport på systemnivå till andra användare.</p> <p>Endast en Workfront-administratör kan redigera en tidrapportprofil på systemnivå.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Identifiera gruppen här om du skapar en tidrapportprofil för en grupp som du administrerar.</p> <p>Detta tilldelar inte tidrapportprofilen till användarna i gruppen utan bara gruppens administratörer möjlighet att ändra tidrapportprofilen. Du tilldelar profilen till användare i steg 6.</p>

   <p><b>Obs!</b> När användare utanför gruppen kopplar tidrapportprofiler till andra användare kan de inte se eller koppla den här tidrapportprofilen.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Skapa tidrapporter</strong> </td> 
      <td> <p> <p>Ange när tidrapportprofilen ska generera tidrapporterna. En tidrapport kan ställas in så att den automatiskt genereras varje vecka, varannan vecka, halvår eller månad. Välj den veckodag då du vill att tidrapporten ska skapas.</p>
      <p>En veckotidrapport börjar det datum då den skapas. Om du t.ex. skapar veckotidrapporter varje torsdag är den första dagen i veckan på tidrapporten torsdag.</p>


   <p><b>Obs!</b> Workfront skapar alltid två tidrapporter i taget: den första tidrapporten innehåller alltid det aktuella datumet och den andra tidrapporten startar när tidsramen för den första är slut.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Godkännare</strong></p> </td> 
      <td> <p> <p>Godkännare är användare som godkänner tidrapporten för användare som är kopplade till tidrapporten. Du kan identifiera upp till 7 användare som godkännare på en tidrapport. Det är praktiskt att identifiera flera användare för att se till att en godkännare är tillgänglig när någon inte är på kontoret. Alla godkännare meddelas när en användare skickar tidrapporten för godkännande. Endast en användare behöver godkänna tidrapporten för att den ska godkännas.</p> <p>Endast användare med administratörsbehörighet för tidrapport kan anges som godkännare. Mer information om administratörsrättigheter för tidrapporter finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> <p>Använd listrutan för att välja godkännare för tidrapporten (om en godkännare krävs). Du kan välja mellan följande alternativ:</p> 
      <ul> 
      <li><strong>Ingen</strong>: Tidrapporten behöver inte godkännas.</li> 
      <li><strong>Deras hanterare</strong>: Det här är standardgodkännaren som ställs in av systemet. I det här fallet godkänner den användare som är utsedd som sin chef tidrapporten när den skickas för godkännande.</li> 
      <li><strong>Specifika personer:</strong> Du kan ange specifika användare efter namn som tidrapportgodkännare. Du kan ha flera godkännare på en tidrapport. När en av godkännarna har godkänt tidrapporten markeras tidrapporten som <strong>Stängd</strong> och försvinner från listan över tidrapportgodkännanden för alla återstående godkännare.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Det går att redigera tid </strong> </td> 
      <td> <p> <p>Välj det här alternativet om godkännarna ska kunna redigera timmar på tidrapporten.

   <p>Det här alternativet fungerar tillsammans med inställningen **Begränsa redigering av tidrapporter till ägare och administratörer** under Inställningar &gt; Tidrapport och timmar &gt; Inställningar. Mer information finns i <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Konfigurera tidrapport och timinställningar</a>.</p>

   <p>Följande scenarier finns: </p>

   <ul>
      <li>När alternativet <b>Begränsa redigering av tidrapport till ägare och administratörer</b> är aktiverat:</li>
      <ul><li>Godkännare kan bara godkänna och avvisa tidrapport, oavsett om <b>Kan redigera tid</b> är aktiverat eller inte. </li>
      <li>Tidrapportsägarnas chefer kan bara visa sina direkt rapporters tidrapporter.</li></ul>
      <li>När alternativet <b>Begränsa redigering av tidrapport till ägare och administratörer</b> är inaktiverat:</li>
    <ul><li>När <b>Kan redigera tid</b> är aktiverat kan godkännare skicka, öppna igen eller stänga tidrapporten och redigera tiden.</li>
      <li>När <b>Kan redigera tid</b> är inaktiverat kan godkännarna inte skicka, öppna igen eller stänga tidrapporten och kan inte redigera tiden. Godkännare kan bara godkänna eller avvisa tidrapporten. </li>
      <li>Tidrapportsägarnas chefer kan skicka, återkalla, öppna och redigera sina direkt underställda tidrapporter.</li></ul>
      </ul>

   <p>

   <b>Obs!</b> När du har skickat in en tidrapport för godkännande kan du inte längre redigera timmarna. Om du vill returnera en inskickad tidrapport till ett redigerbart tillstånd måste du återkalla tidrapporten eller låta godkännaren avvisa tidrapporten. Mer information finns i <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Skicka en tidrapport för godkännande</a> och<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Godkänn en tidrapport</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Övertid</strong> </td> 
      <td>Du kan dölja rutan Övertid i tidrapporter. Det här alternativet är inaktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tillgängliga timtyper</strong> </td> 
      <td><p>Den här inställningen avser endast allmänna timtyper och inte projektspecifika timtyper. </p>
      <p>Som standard ser användare alla allmänna timmar på en tidrapport. Om din organisation bara vill att specifika allmänna timmar ska visas för en viss uppsättning användare, kan du välja de allmänna timmar som de behöver se i sina tidrapporter genom att markera dem i sin tidrapportprofil i det här fältet. Om du vill inaktivera alla allmänna timmar avmarkerar du alla timtyper för att generera tidrapporten utan ett avsnitt för allmänna timmar.</p></td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Påminnelsemeddelanden</strong> </td> 
      <td> <p> Lägg till ett påminnelsemeddelande. Workfront skickar påminnelser till användare som ombeds att fylla i eller godkänna sina tidrapporter. Du måste skapa påminnelsemeddelanden innan du kan koppla dem till en tidrapportprofil.  </p> </td> 
     </tr>

1. När du skapar tidrapportprofiler på gruppnivå i produktion klickar du på fliken **Tilldela personer** för att associera tidrapportprofilen med specifika användare, grupper eller (om du är Workfront-administratör) team. <!--Keep the reference to the group upon release to Prod, for now, until they unshim the group Timesheet Profiles-->

   <span class="preview">När du skapar tidrapportprofiler på gruppnivå i förhandsgranskningen bläddrar du mot sidans nederkant och hittar avsnittet **Tilldela personer**.</span>

   När du skapar tidrapportprofiler för systemet bläddrar du mot sidans nederkant och hittar avsnittet **Tilldela personer**. <!--Keep the reference to the system when releasing to Prod, until they unshim the group Timesheet Profile-->

   Börja skriva namnet på användaren, gruppen eller teamet och klicka sedan på det när det visas i listrutan.

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
