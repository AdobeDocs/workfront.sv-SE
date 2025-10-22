---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Redigera tidrapportinformation
description: Som användare med administrativ åtkomst till tidrapporter kan du redigera information om befintliga tidrapporter i Adobe Workfront. Du kan till exempel redigera ägaren, godkännarna eller tidsramen för tidrapporten.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Redigera tidrapportinformation

Som användare med administrativ åtkomst till tidrapporter kan du redigera information om befintliga tidrapporter i Adobe Workfront. Du kan till exempel redigera ägaren, godkännarna eller tidsramen för tidrapporten.

Du kan redigera information på en enda tidrapport eller redigera flera tidrapporter samtidigt.

>[!IMPORTANT]
>
>Om användare är kopplade till tidrapportprofiler och tidrapporterna genereras automatiskt, återspeglas inte de ändringar du gör i befintliga tidrapporter på de tidrapporter som kommer att genereras för framtida datum. Alla tidrapporter som genereras automatiskt har de inställningar som har angetts i tidrapportprofilerna. Mer information finns i [Skapa tidrapportprofiler](../create-and-manage-timesheets/create-timesheet-profiles.md)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td><p>Administrativ åtkomst till tidrapporter</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera tidrapporter

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Tidrapporter**.

   Filtret **Alla** är markerat som standard, vilket visar alla tidrapporter som du har tillgång till för visning.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Klicka på ikonen **sök** ![](assets/search-icon.png) och skriv ett nyckelord och sök efter en viss tidrapport. Du kan till exempel söka efter en tidsram eller ett ägarnamn för tidrapporten.

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

1. Markera en eller flera tidrapporter och klicka sedan på ikonen **Redigera** ![](assets/edit-icon.png) längst upp i tidrapportlistan.
1. Visa eller ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ägare</strong> </td> 
      <td> <p>Detta är namnet på den användare som tidrapporten skapades för. Du kan inte redigera det här fältet. </p> <p>Fältet visas inte när du väljer flera tidrapporter. </p> </td> 
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
      <td role="rowheader"><strong>Status</strong> </td> 
      <td> Detta är status för tidrapporten.
      Följande är möjliga alternativ för tidrapportstatus: 
      <ul><li><b>Öppna</b>: Tidrapporten är öppen och timposter kan redigeras.</li>
      <li><b>Skickat</b>: Tidrapporten skickas för godkännande till de angivna godkännarna.</li>
      <li><b>Avvisad</b>: Tidrapporten godkändes inte av godkännarna och är nu tillgänglig igen så att användaren kan redigera tidsposterna.</li>
      <li><b>Stängd</b>: Tidrapporten stängs av användaren eller godkänns av godkännaren och därför är den nu stängd. Du kan inte lägga till tid i en stängd tidrapport.</li>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Godkännare</strong> </td> 
      <td> <p>Godkännare är användare som godkänner tidrapporten för användare som är kopplade till tidrapporten. Endast användare med administrativ åtkomst till tidrapporter kan anges som godkännare. </p> <p>Mer information om administratörsrättigheter för tidrapporter finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> <p>Börja skriva in namnen på tidrapportgodkännarna och markera dem när de visas i listan.</p> <p>Du kan ha flera godkännare på en tidrapport. När en av godkännarna har godkänt tidrapporten markeras tidrapporten som <strong>Stängd</strong> och försvinner från listan över tidrapportgodkännanden för alla återstående godkännare.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Kan redigera tid</strong> </td> 
      <td> <p>Välj det här alternativet om du vill tillåta godkännare att redigera timmar på tidrapporten.</p> <p>Det här alternativet är inte tillgängligt när du markerar flera tidrapporter. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Övertid</span> </td> 
      <td> <p>Du kan dölja rutan Övertid på tidrapporten.</p> <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.
