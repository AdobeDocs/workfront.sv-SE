---
title: Duplicera poster
description: Du kan duplicera en befintlig post i tabellvyn. En identisk kopia av den befintliga posten läggs till på posttypssidan.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Duplicera poster

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

I Adobe Workfront Planning är en post en instans av en posttyp.

Du kan duplicera en befintlig post i tabellvyn. En identisk kopia av den befintliga posten läggs till på posttypssidan.

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
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
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
   <td>   <p>Contribute eller högre behörighet till en arbetsyta <span class="preview">och posttyp</span></a> </p>  
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

   * Håll muspekaren över namnet på en post och klicka sedan på menyn **Mer** bredvid postnamnet. Klicka sedan på ikonen **Duplicera** ![Duplicera, grå](assets/duplicate-icon-gray.png) .

     ![Mer meny från post i tabellvy](assets/more-menu-from-record-in-table-view.png)

   * Markera en post och klicka sedan på ikonen **Duplicera** ![Duplicera (vit och blå)](assets/duplicate-icon-white-and-blue.png) i verktygsfältet längst ned på sidan.

     ![Duplicera ikon i verktygsfältet i tabellvyn](assets/duplicate-icon-in-toolbar-in-table-view.png)

   En identisk post med samma namn skapas under den ursprungliga posten. Alla fält i den nya posten fylls i med samma information som i den ursprungliga posten.

1. (Valfritt) Börja uppdatera information om den nya posten i de fält som är tillgängliga i tabellvyn eller klicka på posten och uppdatera informationen i postförhandsgranskningen eller på sidan.

   >[!NOTE]
   >
   >  * Det finns inga obligatoriska fält för poster. Vi rekommenderar dock att du lägger till information för det primära fältet i en post, eftersom det är praktiskt att identifiera poster när du länkar poster till varandra. Mer information om primära fält finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md) och [Översikt över primära fält](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Fält som refererar till andra posttyper eller beräknade fält är skrivskyddade fält.

   Mer information om hur du redigerar poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

1. (Valfritt) Använd följande kortkommandon om du vill ångra eller göra om tillägg av nya poster eller deras information när du lägger till dem i tabellvyn:

   * CTRL + Z (⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z (⌘ + Skift + Z för Mac) om du vill göra om en ändring.
