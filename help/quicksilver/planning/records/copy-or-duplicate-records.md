---
title: Duplicera poster
description: Du kan duplicera en befintlig post i tabellvyn. En identisk kopia av den befintliga posten läggs till på sidan för posttyp.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Duplicera poster

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

I Adobe Workfront Planning är en post en instans av en posttyp.

Du kan duplicera en befintlig post i tabellvyn. En identisk kopia av den befintliga posten läggs till på sidan för posttyp.

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <td>   <p>Bidra eller högre behörigheter till en arbetsyta och posttyp</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat</p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Duplicera en post <!--in a record type table (I don't think you can create them elsewhere right now)-->

Du kan skapa poster i tabellvyn för en posttypssida genom att duplicera en befintlig. En post som är identisk med den befintliga skapas och läggs till under den ursprungliga posten.


{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett kort för en posttyp. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Sidan för posttyp öppnas i den vy som du senast öppnade. Som standard öppnas en posttypssida i tabellvyn.
Alla poster av den valda typen visas i vyn.

1. (Villkorligt) Välj en tabellvy.

1. Gör något av följande:

   * Håll muspekaren över namnet på en post och klicka sedan på **menyn Mer** som är infogad i postnamnet och klicka sedan på **Duplicera** ikonen ![Duplicera ikonen grå](assets/duplicate-icon-gray.png) .

     ![Mer meny från post i tabellvy](assets/more-menu-from-record-in-table-view.png)

   * Markera en post och klicka sedan på **ikonen Duplicera**![ Duplicera ikon vit och blå](assets/duplicate-icon-white-and-blue.png) i verktygsfältet längst ner på sidan.

     ![Duplicera ikon i verktygsfältet i tabellvyn](assets/duplicate-icon-in-toolbar-in-table-view.png)

   En identisk post med ett identiskt namn skapas under den ursprungliga posten. Alla fält i den nya posten fylls i med samma information som i den ursprungliga posten.

1. (Valfritt) Börja uppdatera information om den nya posten i fälten som är tillgängliga i tabellvyn, eller klicka på posten och uppdatera informationen i förhandsgranskningen eller på sidan.

   >[!NOTE]
   >
   >  * Det finns inga obligatoriska fält för poster. Vi rekommenderar dock att du lägger till information för det primära fältet i en post, eftersom det är praktiskt att identifiera poster när du länkar poster till varandra. Mer information om primära fält finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md) och [Översikt över](/help/quicksilver/planning/fields/primary-field-overview.md) primära fält.
   >
   >  * Fält som refererar till andra posttyper eller beräknade fält är skrivskyddade fält.

   Mer information om hur du redigerar poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

1. (Valfritt) Använd följande kortkommandon för att ångra eller göra om tillägg av nya poster eller deras information när du lägger till dem i tabellvyn:

   * Ctrl + Z (⌘ + Z för Mac) för att ångra en ändring
   * Ctrl + Shift + Z (⌘ + Shift + Z för Mac) för att göra om en ändring.
