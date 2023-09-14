---
title: Redigera poster
description: Du kan redigera postinformation i Adobe Maestro. Du måste skapa posttyper innan du kan börja skapa och redigera poster.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Redigera poster

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan redigera postinformation i Adobe Maestro. Du måste skapa posttyper innan du kan börja skapa och redigera poster.
Mer information finns i [Skapa posttyper](../architecture-and-fields/create-record-types.md).

&lt;!— här anger du att fälten i detaljvyn är desamma som fälten i tabellvyn - den här artikeln är länkad från vyerna Hantera post för att referera till den här informationen—>

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

## Att tänka på när du redigerar poster

* Du kan redigera poster som du eller någon annan användare har skapat. <!--will change with access levels-->
* Om de redigerade posterna är länkade till andra poster återspeglas den nya informationen om de poster som du redigerar på de länkade posterna.
* Du kan inte redigera flera poster samtidigt. <!--this will probably change-->

## Redigera poster

Du kan redigera en post i följande områden:

* [Från detaljsidan för en post](#edit-a-record-from-the-records-details-page)
* [Från tabellvyn för en posttyp](#edit-a-record-from-the-record-type-table-view)

### Redigera en post från postens informationssida

1. Klicka på **Huvudmeny** ![](assets/main-menu-workfront.png) i det övre högra hörnet eller **Huvudmeny** ![](assets/main-menu-shell.png) i det övre vänstra hörnet, om det är tillgängligt, klickar du på Makestro.

   Arbetsytan som du öppnar senast öppnas.
1. Gör något av följande:

   * Klicka på en posts namn i en tabellvy.
   * Håll markören över namnet på en post i tabellvyn och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Visa**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicka på ett postfält i en tidslinjevy.

   Posten **Information** sidan öppnas.

1. Klicka på **Mer** meny ![](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Redigera**

   eller

   Klicka i ett redigerbart fält på detaljsidan för att redigera informationen.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

   >[!NOTE]
   >
   >    Länkade fält eller fält som innehåller beräkningar eller som genereras av systemet kan inte redigeras.


1. Klicka **Spara ändringar**. <!--logged a bug for this - this needs to be "Save"-->

### Redigera en post från posttyptabellvyn

1. Klicka på **Huvudmeny** ![](assets/main-menu-workfront.png) i det övre högra hörnet, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> klicka sedan på **Maestro** ![](assets/maestro-icon.png).

   Arbetsytan som du senast öppnade öppnas.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Från **Visa** Välj en tabellvy i den nedrullningsbara menyn i tabellens övre högra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Klicka inuti en post för att börja redigera information om posten och tryck sedan på **Retur** på tangentbordet för att spara ändringarna. Ändringarna sparas automatiskt.

   >[!TIP]
   >
   >Länkade fält kan inte redigeras. Informationen för dessa fält fylls i automatiskt från de länkade posterna. Mer information finns i [Koppla posttyper](../architecture-and-fields/connect-record-types.md).



