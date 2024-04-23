---
title: Hantera postsidan
description: Du kan redigera layouten för postrutan och -sidan i Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Hantera postsidan

{{maestro-important-intro}}

Du kan redigera layouten för postrutan och -sidan i Adobe Workfront Planning. Du kan visa postrutan i en postvy.

Postrutan är en mindre vy av postsidan som visas i vyn av en posttyp.

När du ändrar layouten för en postruta och sida ändras rutan och sidan för alla poster av samma typ.

Du måste skapa posttyper och poster innan du kan börja redigera postsidor.

Mer information finns i följande artiklar:

* [Skapa posttyper](../architecture/create-record-types.md)

* [Skapa poster](/help/quicksilver/maestro/records/create-records.md)

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
<p>Din organisation måste vara registrerad i betaprogrammet Adobe Workfront Planning. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <p>Nytt: Ljus eller högre</p>
   eller
   <p>Aktuell: Arbete eller högre</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera eller högre behörigheter på en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när du redigerar postsidor

* Om du ordnar om fälten i postrutan eller på sidan ordnas fälten om för alla poster av den typen och för alla användare som använder dessa poster.
* Att lägga till en omslagsbild till en post ingår inte i den övergripande layouten för postens ruta eller sida. Du kan lägga till unika omslagsbilder till varje post. Mer information finns i [Lägga till en omslagsbild till en post](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

## Ordna om fält i postrutan eller på sidan

{{step1-to-maestro}}

Arbetsytan som du öppnar senast öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   I tabelltabellvyn klickar du på **Öppna detaljer** icon ![](assets/open-details-icon-in-table-name-field.png) till vänster om ett postnamn.

   Postens ruta öppnas i vyn.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Du kan visa **Öppna detaljer** ikonen till vänster om fältet Namn för en post i en tabellvy enbart när fältet Namn är primärt.

1. (Valfritt) Klicka på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postrutan för att öppna postens sida på en ny flik.

   Postsidan öppnas.

   ![](assets/details-page.png)

1. Klicka på ikonen för att ta tag i posten ![](assets/grab-icon.png) till vänster om ett fältnamn och sedan dra och släppa det på önskad plats.

   Fältets nya position uppdateras både i rutan och på sidan med alla poster av samma typ för alla användare som visar posterna.

   Alla layoutändringar för postrutan eller sidan sparas automatiskt.

