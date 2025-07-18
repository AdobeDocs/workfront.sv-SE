---
title: Ta bort poster
description: Du kan ta bort poster som du eller en annan användare har skapat.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# Ta bort poster

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Du kan ta bort poster som inte längre är relevanta i Adobe Workfront Planning. Du kan återställa borttagna poster i 30 dagar efter att de har tagits bort. Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <li><p> Planering av Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Någon av följande Workfront-planer:</p> 
<ul><li>Utvald</li> 
<li>Primtal</li> 
<li>Sist</li></ul> 
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td> 
   <td> 
<p>Någon </p> 
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad i Adobe Unified Experience för att kunna komma åt Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td>   <p>Bidra eller högre behörigheter till en arbetsyta och posttyp </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat</p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du tar bort poster

* Du kan ta bort poster som du eller en annan användare har skapat.
* Du kan återställa borttagna poster som du eller andra har tagit bort.
* Om de borttagna posterna är länkade till andra poster tas inte de länkade posterna bort, utan informationen från den borttagna posten tas också bort.
* Du kan inte ta bort poster från tidslinjen eller kalendervyerna.

## Ta bort poster

Du kan ta bort en post från följande områden:

* [Från postens sida](#delete-a-record-from-the-records-page)
* [Från tabellvyn för en posttyp](#delete-a-record-from-the-record-type-table-view)

### Ta bort en post från postens sida

{{step1-to-planning}}

1. Klicka på den arbetsyta vars poster du vill ta bort.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett kort för en posttyp.

   Sidan för posttyp öppnas.
1. Gör något av följande:

   * I en tabellvy klickar du på namnet på en post.
   * Håll muspekaren över namnet på en post i tabellvyn, klicka sedan på **menyn Mer**![ på menyn](assets/more-menu.png) Mer och klicka sedan på **Visa**

     ![Kontextuell meny för postrad](assets/contextual-menu-for-record-row.png)
   * Från en tidslinjevy klickar du på en poststapel.

   Postsidan öppnas.

1. **Klicka på menyn** Mer![ på menyn](assets/more-menu.png) Mer till höger om postens namn och klicka sedan på **Ta bort** och sedan **på Ta bort** igen för att bekräfta.

   ![Fler menyalternativ från sidan](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed--> med postinformation
Posten tas bort.
1. (Valfritt) Gå till tabellvyn på postsidan och klicka på **ikonen Ångra**![ ](assets/undo-icon.png)i det övre högra hörnet av vyn och klicka sedan på **Nyligen raderade** för att återställa de raderade posterna.

Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).

### Ta bort en post från tabellvyn för posttyp

{{step1-to-planning}}

1. Klicka på den arbetsyta vars poster du vill ta bort.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett kort för en posttyp.

   Sidan för posttyp öppnas.
1. (Villkorligt) **** I listrutan Visa i det övre vänstra hörnet av tabellen väljer du en tabellvy. Detta bör vara standardvyn, såvida du inte visade posttypen i tidslinjevyn när du öppnade den senast.

   De poster som är associerade med den valda posttypen visas i tabellvyn.
1. Gör något av följande:

   * Högerklicka på en postrad och klicka sedan på **Ta bort**.
   * **Klicka på menyn Mer** på menyn![ ](assets/more-menu.png)Mer till höger om postens namn och klicka sedan på **Ta bort**.

     ![Kontextuell meny för postrad](assets/contextual-menu-for-record-row.png)

   * **Klicka på ikonen**&#x200B;Öppna detaljer![ ikonen Öppna detaljer i fältet](assets/open-details-icon-in-table-name-field.png) för tabellnamn för att öppna rutan med detaljerad information om posten och klicka sedan på menyn Mer **** Mer![ till höger om postnamnet och sedan ](assets/more-menu.png)**på Ta bort**.

   Posten tas bort.

1. (Valfritt) Gör något av följande om du vill ångra eller göra om borttagningen av en post:

   * Klicka på **ikonen Ångra** ![](assets/undo-icon.png)och sedan **på Nyligen raderade** för att återställa de raderade posterna. Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Använd följande kortkommandon för att ångra eller göra om borttagningen av en post:

      * CTRL + Z (⌘ + Z för Mac) för att ångra borttagning av en post
      * Ctrl + Shift + Z (⌘ + Shift + Z för Mac) för att göra om raderingen av posten




