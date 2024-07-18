---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Ta bort tidrapporter i Adobe Workfront
description: De ändringar du gör i en tidrapportprofil gäller inte direkt för de befintliga tidrapporterna, vilket förklaras i Skapa, redigera och tilldela tidrapportprofiler. Om du vill göra ändringarna synliga på befintliga tidrapporter måste du ta bort de tidrapporter som har skapats och generera nya. Detta gäller endast tidrapporter som har skapats genom att tidrapportprofiler associeras med användare.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Ta bort tidrapporter i Adobe Workfront

De ändringar du gör i en tidrapportprofil gäller inte direkt för de befintliga tidrapporterna, vilket förklaras i [Skapa, redigera och tilldela tidrapportprofiler](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Om du vill göra ändringarna synliga på befintliga tidrapporter måste du ta bort de tidrapporter som har skapats och generera nya. Detta gäller endast tidrapporter som har skapats genom att tidrapportprofiler associeras med användare.

>[!NOTE]
>
>Tidrapporter som har skapats manuellt kan inte återskapas genom att tidrapporter genereras om, såvida inte användarna har kopplats till en tidrapportprofil sedan tidrapporten skapades manuellt. Om du tar bort en manuellt skapad tidrapport kan data gå förlorade. Mer information om hur du skapar enskilda tidrapporter finns i [Skapa en tidrapport för engångsbruk](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Adobe Workfront-administratörer eller gruppadministratörer kan generera tidrapporter för alla i systemet. Mer information om hur du genererar tidrapporter manuellt finns i:

* [Generera tidrapporter manuellt](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Skapa och hantera en grupps tidrapportprofiler](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* Du kan inte återställa en borttagen tidrapport.
>* Vi rekommenderar att du inte tar bort tidigare tidrapporter eftersom de inte genereras automatiskt baserat på tidrapportprofiler. Du kan ta bort aktuella och framtida tidrapporter och generera dem manuellt om du vill att ändringarna i tidrapportprofilerna ska vara omedelbart synliga i de nya tidrapporterna.
>* När du tar bort tidrapporter tas inte de timmar som är loggade mot uppgifter, utleveranser och projekt bort. Endast Allmänna timmar tas bort med tidrapporten. I en separat textredigerare anger du vilka allmänna timmar som är kopplade till tidrapporten. När tidrapporten har tagits bort kan du logga dem i den nya tidrapporten.
>

## Åtkomstkrav

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste ha administrativ åtkomst till tidrapporter. </p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Ta bort tidrapporter i en lista

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Tidrapporter**. Filtret **Alla** är markerat som standard och visar alla tidrapporter som du har tillgång till för visning.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Uppdatera filtret i listan över tidrapporter genom att göra något av följande:

   * Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du godkänner

     eller

     Välj **Mina tidrapporter** om du bara vill visa dina tidrapporter.

     Detta tillämpar filtren Mina tidrapportgodkännanden eller Min tidrapport på listan med tidrapporter.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicka på Filterikonen ![](assets/filter-nwepng.png) om du vill använda ett annat filter eller skapa ett nytt. Mer information om hur du skapar eller uppdaterar filter finns i [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Alternativen Mina tidrapportgodkännanden och Mina tidrapporter visas inte högst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtren Mina tidrapportgodkännanden och Mina tidrapporter från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   >
   >   
   >   
   >   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Valfritt) Klicka på ikonerna **Visa** ![](assets/view-icon.png) eller **Gruppera** ![](assets/grouping.png) om du vill använda en annan vy eller gruppering eller skapa en ny.

   Mer information om hur du skapar filter, vyer och grupperingar finns i följande artiklar:

   * [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Skapa eller redigera vyer i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Skapa grupperingar i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Markera en eller flera tidrapporter som du vill ta bort och klicka på ikonen **Ta bort** ![](assets/delete.png) längst upp i listan med tidrapporter.

1. Klicka på **Ta bort**.

   De valda tidrapporterna tas bort och kan inte återställas.

   Om du vill generera nya tidrapporter måste du se till att användarna är kopplade till en tidrapportprofil och be Workfront-administratören eller en gruppadministratör att generera nya tidrapporter.

   Mer information finns i följande:

   * [Skapa, redigera och tilldela tidrapportprofiler](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Generera tidrapporter manuellt](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Skapa och hantera en grupps tidrapportprofiler](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Ta bort en tidrapport från tidrapportsidan

1. Klicka på ikonen [!UICONTROL **Huvudmeny**] ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.
1. Klicka på den tidrapport som du vill ta bort för att öppna den.
1. Klicka på ikonen [!UICONTROL **Mer**] ![](assets/more-icon.png) till höger om tidrapportnamnet och klicka sedan på **Ta bort**.

   ![Ta bort tidrapport från tidrapportsida](assets/delete-timesheet-from-timesheet-page.png)
1. Bekräfta genom att klicka på [!UICONTROL **Ta bort**].

   Tidrapporten tas bort och kan inte återställas.
