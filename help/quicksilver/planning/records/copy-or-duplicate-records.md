---
title: Duplicera poster
description: Du kan duplicera en befintlig post i tabellvyn. En identisk kopia av den befintliga posten läggs till på posttypssidan.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---


# Duplicera poster

<!--update the metadata after GA-->

{{planning-important-intro}}

I Adobe Workfront Planning är en post en instans av en posttyp.

Du kan duplicera en befintlig post i tabellvyn. En identisk kopia av den befintliga posten läggs till på posttypssidan.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Nytt: Standard</p>
   <p>Aktuell: Planera</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Adobe Workfront Planning </p>  
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

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Duplicera en post <!--in a record type table (I don't think you can create them elsewhere right now)-->

Du kan skapa poster i tabellvyn för en posttypsida genom att duplicera en befintlig post. En post som är identisk med den befintliga skapas och läggs till under den ursprungliga posten.


{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.
Alla poster av den valda typen visas i vyn.

1. (Villkorligt) Välj en tabellvy.

1. Gör något av följande:

   * Håll muspekaren över namnet på en post och klicka sedan på menyn **Mer** bredvid postnamnet. Klicka sedan på ikonen **Duplicera** ![](assets/duplicate-icon-gray.png) .

     ![](assets/more-menu-from-record-in-table-view.png)

   * Markera en post och klicka sedan på ikonen **Duplicera** ![](assets/duplicate-icon-white-and-blue.png) i verktygsfältet längst ned på sidan.

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   En identisk post med samma namn skapas under den ursprungliga posten. Alla fält i den nya posten fylls i med samma information som i den ursprungliga posten.

1. (Valfritt) Börja uppdatera information om den nya posten i de fält som är tillgängliga i tabellvyn eller klicka på posten och uppdatera informationen i postförhandsgranskningen eller på sidan.

   >[!NOTE]
   >
   >  * Det finns inga obligatoriska fält för poster. Vi rekommenderar dock att du lägger till information för det primära fältet i en post, eftersom det är praktiskt att identifiera poster när du länkar poster till varandra. Mer information om primära fält finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md) och [Översikt över primära fält](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Fält som refererar till andra posttyper eller beräknade fält är skrivskyddade fält.

   Mer information om hur du redigerar poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

1. (Valfritt) Använd följande kortkommandon om du vill ångra eller göra om tillägg av nya poster eller deras information när du lägger till dem i tabellvyn:

   * CTRL + Z ( ⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) om du vill göra om en ändring.