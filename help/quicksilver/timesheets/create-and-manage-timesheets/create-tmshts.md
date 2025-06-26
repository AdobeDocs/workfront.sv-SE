---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Skapa en tidrapport för engångsbruk
description: Du kan skapa en tidrapport för engångsbruk manuellt om du vill ha en tidrapport som inte är återkommande. När slutdatumet för tidrapporten nås och du behöver fler tidrapporter måste du skapa nya.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 0%

---

# Skapa en tidrapport för engångsbruk

<!--Audited: 6/2025-->

Du kan skapa en tidrapport för engångsbruk manuellt om du vill ha en tidrapport som inte är återkommande. När slutdatumet för tidrapporten nås och du behöver fler tidrapporter måste du skapa nya.

Mer information om hur du skapar en tidrapportprofil som genererar återkommande tidrapporter för dina användare utan att du behöver göra något (rekommenderas) finns i [Skapa, redigera och tilldela tidrapportprofiler](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Mer information om hur du manuellt genererar tidrapporter för alla användare i systemet som är kopplade till en tidrapportprofil finns i [Generera tidrapporter manuellt](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

>[!NOTE]
>
>* Det går inte att skapa engångstidrapporter för grupper.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* När du skapar en enskild tidrapport kan du inte välja specifika allmänna timtyper att inkludera i tidrapporten. Alla allmänna timtyper som aktiveras i systemet visas i tidrapporter som skapas manuellt.
>
>  Om du bara vill välja vissa allmänna timtyper att visa i tidrapporterna använder du en tidrapportprofil. Mer information om tidrapportprofiler finns i [Skapa, redigera och tilldela tidrapportprofiler](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> <p>Du måste ha administrativ åtkomst till tidrapporter. </p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en tidrapport för engångsbruk

{{step1-to-timesheets}}

Filtret **Alla** är markerat som standard. Då visas alla tidrapporter som du har tillgång till.

![Lista över tidrapporter med en tidrapport vald](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Uppdatera filtret i listan över tidrapporter genom att göra något av följande:

   * Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du godkänner

     eller

     Välj **Mina tidrapporter** om du bara vill visa dina tidrapporter.

     Detta tillämpar filtren Mina tidrapportgodkännanden eller Min tidrapport på listan med tidrapporter.

     ![Mina filterknappar för tidrapporter på listsidan för tidrapporter](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicka på ikonen **Filter** ![Filter ](assets/filter-nwepng.png) om du vill använda ett annat filter eller skapa ett nytt. Mer information om hur du skapar eller uppdaterar filter finns i [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Alternativen Mina tidrapportgodkännanden och Mina tidrapporter visas inte högst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtren Mina tidrapportgodkännanden och Mina tidrapporter från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   > 
   >   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Valfritt) Klicka på ikonen **Sök** ![Sök ](assets/search-icon.png) om du vill skriva ett nyckelord och söka efter en viss tidrapport. Du kan t.ex. söka efter en tidsram för tidrapporten med ägarnamnet.

1. (Valfritt) Klicka på ikonerna **Visa** ![Visa](assets/view-icon.png) eller **Gruppera** ![Gruppera](assets/grouping.png) om du vill använda en annan vy eller gruppering eller skapa en ny.

   Mer information om hur du skapar filter, vyer och grupperingar finns i följande artiklar:

   * [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Skapa eller redigera vyer i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Skapa grupperingar i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Klicka på **Ny tidrapport** högst upp i listan över tidrapporter.

   Ange följande information:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Skapa tidrapport för</strong> </td> 
      <td>Börja ange namnet på användaren, en jobbroll eller ett team som du skapar tidrapporten för och klicka på dem när de visas i listan.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Startdatum</strong> </td> 
      <td>Detta är startdatumet för tidrapporten.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Slutdatum</strong> </td> 
      <td> Detta är slutdatumet för tidrapporten.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Godkännare</strong> </td> 
      <td>Godkännare är användare som godkänner tidrapporten för användare som är kopplade till tidrapporten. Endast användare med administratörsbehörighet för tidrapport kan anges som godkännare. Mer information om administratörsrättigheter för tidrapporter finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.<br>Börja ange namnen på tidrapportgodkännarna och klicka på dem när de visas i listan.<br>Du kan ha flera godkännare på en tidrapport. När en av godkännarna har godkänt tidrapporten markeras tidrapporten som <strong>Stängd</strong> och försvinner från listan över tidrapportgodkännanden för alla återstående godkännare.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Kan redigera tid</strong> </td>

   <td> <p>Välj det här alternativet om du vill tillåta godkännare att redigera timmar på tidrapporten.</p>

   Det här alternativet fungerar tillsammans med inställningen **Begränsa redigering av tidrapporter till ägare och administratörer** i området Inställningar > Tidrapport och timmar > Inställningar. Mer information finns i <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Konfigurera tidrapport och timinställningar</a>.

   Följande scenarier finns:

   <ul>
      <li>När alternativet <b>Begränsa redigering av tidrapport till ägare och administratörer</b> är aktiverat:</li>
   <ul><li>Godkännare kan bara godkänna och avvisa tidrapport, oavsett om <b>Kan redigera tid</b> är aktiverat eller inte. </li>
   <li>Tidrapportsägarnas chefer kan bara visa sina direkt rapporters tidrapporter.</li></ul>
   <li>När alternativet <b>Begränsa redigering av tidrapport till ägare och administratörer</b> är inaktiverat:</li>
   <ul><li>När <b>Kan redigera tid</b> är aktiverat kan godkännare skicka, öppna igen eller stänga tidrapporten och redigera tiden.</li>
   <li>När <b>Kan redigera tid</b> är inaktiverat kan godkännarna inte skicka, öppna igen eller stänga tidrapporten och kan inte redigera tiden. Godkännare kan bara godkänna eller avvisa tidrapporten. </li>
   <li>Tidrapportsägarnas chefer kan skicka, återkalla, öppna och redigera sina direkt underställda tidrapporter.</li></ul>
   </ul>

   <p><b>ANMÄRKNING</b>

   När du har skickat in en tidrapport för godkännande kan du inte längre redigera timmarna. Om du vill returnera en inskickad tidrapport till ett redigerbart tillstånd måste du återkalla tidrapporten eller låta godkännaren avvisa tidrapporten. Mer information finns i <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Skicka en tidrapport för godkännande</a> och <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Godkänn en tidrapport</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Övertid</span> </td> 
      <td>Du kan dölja rutan Övertid på tidrapporten. Det här alternativet är inaktiverat som standard.</td> 
      </tr> 
      </tbody> 
   </table>

1. Klicka på **Skapa tidrapport**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## När uppgifter och problem visas på användarnas tidrapporter

En uppgift eller ett ärende som tilldelats en användare visas automatiskt på tidrapporten för en användare om uppgiften eller problemet uppfyller något av följande kriterier:

* Användaren har loggat timmar på uppgiften eller problemet
* Planerade datum för uppgiften eller utgåvan ligger inom datumen för tidrapporten
* Aktiviteten eller utleveransen har ett faktiskt startdatum (aktiviteten eller utgivningsstatusen är Pågår)
* Aktiviteten eller problemet är fäst på tidrapporten
* Planerat slutförandedatum ligger inom datumintervallet för tidrapporten och statusen Pågår

Om **förifylla tidrapporter med ...**-inställningar (som finns i tidrapporter och timinställningar) är avmarkerade visas problem och uppgifter med statusen Pågår i tidrapporten. Mer information om tidrapporter och timinställningar finns i [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
