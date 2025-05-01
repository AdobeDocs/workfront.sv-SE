---
title: Ta bort poster
description: Du kan ta bort poster som du eller någon annan användare har skapat.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 0%

---


# Ta bort poster

<!--take Preview and Production references out at release-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan ta bort poster som inte längre är relevanta i Adobe Workfront Planning. Du kan återställa borttagna poster i 30 dagar efter att de tagits bort. Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Contribute eller högre behörighet till en arbetsyta <span class="preview">och posttyp</span> </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning.</p>
<p><span class="preview">I förhandsvisningsmiljön har standardanvändare och systemadministratörer Planering aktiverat som standard.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du tar bort poster

* Du kan ta bort poster som du eller någon annan användare har skapat.
* Du kan inte återställa borttagna poster i produktionsmiljön. Du kan återställa borttagna poster i förhandsgranskningsmiljön.
* Om de borttagna posterna är länkade till andra poster tas de länkade posterna inte bort, men informationen från den borttagna posten tas också bort.
* Du kan inte ta bort poster från tidslinjen eller kalendervyer.

## Ta bort poster

Du kan ta bort en post från följande områden:

* [Från postens sida](#delete-a-record-from-the-records-page)
* [Från tabellvyn för en posttyp](#delete-a-record-from-the-record-type-table-view)

### Ta bort en post från postens sida

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill ta bort.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. Gör något av följande:

   * Klicka på en posts namn i en tabellvy.
   * Håll markören över namnet på en post i tabellvyn, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Visa**

     ![Sammanhangsbaserad meny för postrad](assets/contextual-menu-for-record-row.png)
   * Klicka på ett postfält i en tidslinjevy.

   Postsidan öppnas.

1. Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om postnamnet, klicka sedan på **Ta bort** och sedan på **Ta bort** igen för att bekräfta.

   ![Fler menyalternativ från postinformationssidan](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Posten tas bort.
1. (Valfritt och villkorligt) Om du tar bort posten i förhandsvisningsmiljön går du till postsidans tabellvy och klickar på ikonen **Ångra** ![Ångra ](assets/undo-icon.png) i vyns övre högra hörn. Klicka sedan på **Senast borttagen** för att återställa de borttagna posterna.

Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).

### Ta bort en post från posttyptabellvyn

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill ta bort.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Välj en tabellvy på den nedrullningsbara menyn **Visa** i tabellens övre vänstra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Gör något av följande:

   * Högerklicka på en postrad och klicka sedan på **Ta bort**.
   * Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Ta bort**.

     ![Sammanhangsbaserad meny för postrad](assets/contextual-menu-for-record-row.png)

   * Klicka på ikonen **Öppna detaljer** ![Öppna detaljikonen i tabellnamnsfältet](assets/open-details-icon-in-table-name-field.png) för att öppna rutan med postens detaljerade information. Klicka sedan på **Mer** ![Mer-menyn](assets/more-menu.png) till höger om postnamnet och sedan på **Ta bort**.

   Posten tas bort.

1. (Valfritt) Gör något av följande om du vill ångra eller göra om borttagning av en post:

   * Klicka på ikonen **Ångra** ![Ångra ](assets/undo-icon.png) och sedan på **Senast borttagen** för att återställa de borttagna posterna. Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Använd följande kortkommandon för att ångra eller göra om borttagning av en post:

      * CTRL + Z ( ⌘ + Z för Mac) för att ångra borttagning av en post
      * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) för att göra om radering av post




