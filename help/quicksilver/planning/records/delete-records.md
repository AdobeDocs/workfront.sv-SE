---
title: Ta bort poster
description: Du kan ta bort poster som du eller någon annan användare har skapat. Du kan inte återställa borttagna poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Ta bort poster

{{planning-important-intro}}

Du kan ta bort poster som inte längre är relevanta i Adobe Workfront Planning.

## Åtkomstkrav

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
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p>
   </td>
   <td>
   <p>Nytt: Standard</p>
   <p>Aktuell: Planera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Contribute eller högre behörighet till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Att tänka på när du tar bort poster

* Du kan ta bort poster som du eller någon annan användare har skapat.
* Du kan inte återställa borttagna poster. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Om de borttagna posterna är länkade till andra poster tas de länkade posterna inte bort, men informationen från den borttagna posten tas också bort.
* Du kan inte ta bort flera poster samtidigt. <!--this will probably change-->
* Du kan inte ta bort poster från tidslinjevyn.

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
   * Håll markören över namnet på en post i tabellvyn, klicka på menyn **Mer** ![](assets/more-menu.png) och sedan på **Visa**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicka på ett postfält i en tidslinjevy.

   Postsidan öppnas.

1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om postnamnet, klicka sedan på **Ta bort** och sedan på **Ta bort** igen för att bekräfta.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Posten tas bort och kan inte återställas.

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
   * Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Ta bort**

     ![](assets/contextual-menu-for-record-row.png)

   * Klicka på ikonen **Öppna detaljer** ![](assets/open-details-icon-in-table-name-field.png) för att öppna rutan med postens detaljerade information, och klicka på **Mer** ![](assets/more-menu.png) till höger om postnamnet och sedan på **Ta bort**.

   Posten tas bort och kan inte återställas.

1. (Valfritt) Använd följande kortkommandon för att ångra eller göra om borttagning av en post:

   * CTRL + Z ( ⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) för att göra om en ändring
