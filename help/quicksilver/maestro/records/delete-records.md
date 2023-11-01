---
title: Ta bort poster
description: Du kan ta bort poster som du eller någon annan användare har skapat. Du kan inte återställa borttagna poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 1dcc267f04242782efea4a219410380ca5a01e1d
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Ta bort poster

>[!IMPORTANT]
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan ta bort poster som inte längre är relevanta i Adobe Maestro.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Alla</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när du tar bort poster

* Du kan ta bort poster som du eller någon annan användare har skapat.
* Du kan inte återställa borttagna poster. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Om de borttagna posterna är länkade till andra poster tas de länkade posterna inte bort, men informationen från den borttagna posten tas också bort.
* Du kan inte ta bort flera poster samtidigt. <!--this will probably change-->
* Du kan inte ta bort poster från tidslinjevyn.
* Du kan inte ta bort en posttyp som är länkad från ett annat program. Om du t.ex. länkar en Maestro-post till ett Workfront-objekt kan du inte ta bort Workfront-objektet från Workfront objektpostsida.

## Ta bort poster

Du kan ta bort en post från följande områden:

* [Från detaljsidan för en post](#delete-a-record-from-the-records-details-page)
* [Från tabellvyn för en posttyp](#delete-a-record-from-the-record-type-table-view)

### Ta bort en post från postens informationssida

1. Klicka på **Huvudmeny** ![](assets/main-menu-workfront.png) i det övre högra hörnet eller **Huvudmeny** ![](assets/main-menu-shell.png) i det övre vänstra hörnet, om det är tillgängligt, klickar du på Makestro.

   Arbetsytan som du öppnar senast öppnas.
1. Klicka på en posttyp.

   Posttypssidan öppnas.
1. Gör något av följande:

   * Klicka på en posts namn i en tabellvy.
   * Håll markören över namnet på en post i tabellvyn och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Visa**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicka på ett postfält i en tidslinjevy.

   Posten **Information** sidan öppnas.

1. Klicka på **Mer** meny ![](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Ta bort** sedan **Ta bort** igen för att bekräfta.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Posten tas bort och kan inte återställas.

### Ta bort en post från posttyptabellvyn

1. Klicka på **Huvudmeny** ![](assets/main-menu-workfront.png) i det övre högra hörnet eller **Huvudmeny** ![](assets/main-menu-shell.png) i det övre vänstra hörnet, om det är tillgängligt, klickar du på **Maestro**.

   Arbetsytan som du senast öppnade öppnas.
1. Klicka på en posttyp.

   Posttypssidan öppnas.
1. (Villkorligt) Från **Visa** Välj en tabellvy i den nedrullningsbara menyn i tabellens övre högra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Högerklicka på en postrad och klicka sedan på **Ta bort**.

   ![](assets/contextual-menu-for-record-row.png)

   Posten tas bort och kan inte återställas.
