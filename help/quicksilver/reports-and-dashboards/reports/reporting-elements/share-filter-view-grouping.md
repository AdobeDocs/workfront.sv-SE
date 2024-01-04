---
product-area: reporting
navigation-topic: reporting-elements
title: Dela ett filter, en vy eller en grupp
description: Du kan dela filter, vyer och grupperingar som du har tillgång till för att visa med andra användare.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# Dela ett filter, en vy eller en grupp

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera objekt när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till objekt finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller redigera specifika objekt som du har skapat eller har åtkomst till att dela. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Du kan dela filter, vyer och grupperingar som du har tillgång till för att visa med andra användare.

När ett filter, en vy eller en gruppering delas med dig, kan du använda filtret, vyn eller grupperingen i dina listor. Beroende på vilken åtkomst du har kan du eventuellt ändra den och dela den med andra användare.

Mer information om hur du skapar ett filter, en vy eller en gruppering finns i följande artiklar:

* [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Visa eller ge senare åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa eller högre behörigheter med åtkomst till delning till en vy, filter eller gruppering</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Dela ett filter, en vy eller en grupp

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

Delningsfiltren i valda listor skiljer sig åt beroende på vilket gränssnitt du använder för att dela filtret från: standard eller äldre. Mer information om olika typer av gränssnitt för filteruppbyggnad finns i [Skapa eller redigera filter i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Du kan bara dela vyer och grupperingar i det äldre gränssnittet.

### Dela filter med standardgränssnittet i Builder

Du kan dela ett filter i standardgränssnittet från listor med projekt, uppgifter, utgåvor, portfolior, program, användare, mallar eller grupper. Standardbygggränssnittet för filter är inte tillgängligt för andra objekt eller för vyer eller grupperingar.

Dela ett filter med standardgränssnittet i Builder:

1. Gå till en lista med projekt, uppgifter eller problem.
1. Klicka på **Filter** icon ![Filterikon](assets/filter-nwepng.png).

   ![Standardfilterverktyg](assets/new-filters-all-filter-types.png)

1. Granska följande filterlistor:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Favoriter</strong></td>
   <td>Filter som du markerade som favoriter. När du väljer ett filter visas dess ursprungliga plats under filternamnet och den döljs i den ursprungliga listan om du inte tar bort den som favorit.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Sparad</strong></td>
   <td>Filter som du har skapat och sparat själv. Som standard visas sparade filter i den här listan i den ordning som de senast sparades, men filternamnen kan dras för att ändra ordningen på listan manuellt.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Systemstandard</strong></td>
   <td>Workfront standardfilter, liksom filter som Workfront-administratören har lagt till i din filterlista, antingen på systemnivå eller i din layoutmall.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Delas med mig</strong></td>
   <td>Filter som andra har skapat och delat med dig eller som är gemensamma för hela systemet.</td>
   </tr>
   </tbody>
   </table>

1. Håll muspekaren över ett filter som du har tillgång till, åtminstone visa och dela, och klicka sedan på **Mer** meny ![Menyn Mer](assets/more-icon-spectrum.png)och sedan klicka **Dela**.

   ![Fler menyalternativ](assets/new-filters-more-menu-options-with-delete.png)

   Rutan Filterdelning visas.

1. Aktivera **Visa hela systemet** inställning. Detta ger alla i Workfront behörighet att visa filtret.

   >[!IMPORTANT]
   >
   >Använd den här inställningen med försiktighet. Om du lägger till många filter för alla användare blir det svårare att hitta filtren.

   Eller börja skriva namnen på användare, team, roller, grupper eller företag som du vill dela med i **Ge åtkomst till** fält.

   ![Filterdelningsruta](assets/new-filters-share-filter.png)

1. (Valfritt) Klicka på högerpilen bredvid namnet på en enhet för att redigera deras behörigheter till filtret och aktivera sedan antingen **Visa** eller **Hantera** alternativ. **Visa** är standard.

   ![Delningsbehörigheter](assets/new-filters-sharing-permissions.png)

1. (Valfritt) Aktivera eller inaktivera ytterligare behörigheter för en enhet genom att göra något av följande:

   1. Klicka **Visa** och inaktivera **Dela** alternativ. Den är aktiverad som standard.
   1. Klicka **Hantera** och inaktivera antingen **Dela** eller **Ta bort** alternativ. De är aktiverade som standard.

      >[!NOTE]
      >
      >Om du aktiverar Hantera-åtkomst med alternativet Ta bort kan dessa användare ta bort filtret från alla användare, även om de inte äger filtret.

   >[!TIP]
   >
   >Användare kan inte få en högre behörighet än deras åtkomstnivå. Om de inte har åtkomst till redigeringsfilter på åtkomstnivån kan de inte få behörighet att hantera ett filter. Workfront inaktiverar alternativet Hantera för dessa användare och alternativet är nedtonat.

1. Klicka **Dela**. Filtret delas med de enheter som du har angett.

   >[!TIP]
   >
   >När du delar med grupper får filtret behörigheter till medlemmarna i gruppen och alla undergrupper.

   Filtren som du delade visas i **Delas med mig** i filterpanelen för dessa enheter.

   ![Filter som delas med mig](assets/new-filters-shared-with-me.png)

### Dela filter, vyer och grupperingar med det äldre gränssnittet

Delningsfilter, vyer och grupperingar i det äldre gränssnittet är identiska.

1. Gå till en lista med objekt eller en rapport.
1. (Villkorligt) Klicka på **Filter**, **Visa**, eller **Gruppering** och för muspekaren över det filter, den vy eller gruppering som du vill dela. **Mer** icon ![Mer-ikon](assets/more-icon.png)sedan **Dela**.

   Klicka på **Filter**, **Visa**, eller **Gruppering** och sedan välja det filter, den vy eller grupp som du vill dela.

1. (Villkorligt) Om du delar från en rapport klickar du på **Filter**, **Visa**, eller **Gruppering** nedrullningsbar meny igen och klicka sedan på **Dela filter**, **Dela vy**, eller **Dela gruppering**.\
   The **Filteråtkomst**, **Visa åtkomst**, eller **Grupperingsåtkomst** visas.

   ![Delningsfilter](assets/share-filter-people-box-nwe-350x458.png)

1. Fyll i något av följande, beroende på vem du vill dela med:

   **Så här delar du med enskilda användare, team, roller, grupper eller företag:** I det angivna fältet börjar du skriva namnet på användaren, teamet, rollen, gruppen eller företaget som du vill dela med och klickar sedan på namnet i listrutan.\
   Upprepa den här processen om du vill dela åtkomst med flera användare, team, roller, grupper eller företag.

   >[!TIP]
   >
   >När du delar med grupper får du behörighet till filtret, vyn eller grupperingen till medlemmarna i gruppen och till alla undergrupper.

   **Så här delar du med alla användare i systemet:** Klicka på **Inställningar** ikonen och klicka sedan på **Gör detta synligt för hela systemet**.\
   Administratören måste markera alternativet Dela hela systemet för att det här alternativet ska vara tillgängligt. Mer information finns i artiklarna [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) och [Dela rapporter, kontrollpaneler och kalendrar](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Villkorligt) Om du delar med enskilda användare, team, roller, grupper eller företag, klickar du på den nedrullningsbara menyn för att definiera den åtkomstnivå som du vill bevilja.

   Du kan välja mellan följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Se det</strong></td> 
      <td> <p>Välj det här alternativet om du bara vill tillåta delningsmottagare att använda det delade filtret, vyn eller grupperingen. När det här alternativet är markerat kan mottagarna inte göra några ändringar i det delade objektet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Hantera det</strong></td> 
      <td> <p>Välj det här alternativet om du vill tillåta att delningsmottagare använder och ändrar det delade filtret, vyn eller grupperingen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dela</strong></td> 
      <td> <p>Klicka <strong>Avancerade inställningar</strong>markerar eller rensar du <strong>Dela</strong> beroende på om du vill att mottagarna ska kunna dela med andra.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara**.

   Användare som du har delat filtret, vyn eller gruppen med kan komma åt den genom att klicka på **Filter**, **Visa**, eller **Gruppering** nedrullningsbar meny eller ikon och rullar nedåt till **Delas med mig** -avsnitt.


