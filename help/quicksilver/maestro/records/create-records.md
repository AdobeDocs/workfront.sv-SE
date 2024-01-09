---
title: Skapa poster
description: I Adobe Maestro är en post en instans av en posttyp. Du måste skapa posttyper innan du kan skapa enskilda poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Skapa poster

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

I Adobe Maestro är en post en instans av en posttyp.

Du kan ha följande typer av poster:

* **Driftsregister**: De representerar arbetsrelaterade objekt. För en operativ post med namnet&quot;Campaign&quot; kan du till exempel ha namngett poster som&quot;Monthly Newsletter&quot; eller&quot;Sommarförsäljning&quot;.
* **Taxonomiposter**: De representerar attribut som kan kopplas till operativa poster. För en taxonomiposttyp som heter &quot;Kanal&quot; kan du till exempel ha namngett taxonomier som &quot;E-post&quot;, &quot;Sociala media&quot; eller &quot;Annonsering&quot;.

Att skapa driftsposter är detsamma som att skapa taxonomiposter eller taxonomier.

Du kan skapa poster i Maestro genom att göra något av följande:

* Skapa dem manuellt för Maestro-posttyper
* Koppla dem till Maestro-poster från andra program.
* Skapa poster genom att kopiera och klistra in information från en extern lista.

I den här artikeln beskrivs hur du skapar Maestro-poster. Mer information om hur du hanterar poster i tabell- och tidslinjevyer finns i följande artiklar:

* [Hantera tabellvyn](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Hantera tidslinjevyn](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Skapa poster genom att lägga till dem manuellt till en posttyp <!--in a record type table (I don't think you can create them elsewhere right now)-->

Du kan skapa poster i tabellvyn för en posttypssida.

{#step1-to-maestro}

Arbetsytan som du senast öppnade öppnas som standard. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).
1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.
Alla poster av den valda typen visas i tabellvyn.

1. (Villkorligt) Om posttypsidan inte öppnas i tabellvyn klickar du på **Visa** och välj en befintlig **Tabellvy** ![](assets/table-view-icon.png) eller klicka **Skapa vy > Tabell** för att skapa en tabellvy.

1. Om du vill lägga till nya poster klickar du **Nytt &lt; Posttypnamn >** i tabellens sista rad

   eller

   Klicka **Skift + Retur** på tangentbordet från en kolumn eller rad i tabellen. Det här annonserar en tom rad.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Börja skriva information på den nya raden om den nya posten.

   >[!NOTE]
   >
   >  * Det finns inga obligatoriska fält för poster. Vi rekommenderar dock att du lägger till ett namn för posten, eftersom det är praktiskt att identifiera poster när du länkar poster till varandra.
   >
   >  * Fält som refererar till andra posttyper eller beräknade fält är skrivskyddade fält.

1. Fortsätt lägga till information på varje rad och klicka sedan på **Retur** på tangentbordet för att spara ändringarna.

<!--1. (Optional) Use the following keyboard shortcuts to undo or redo adding new records: 

    * **Undo**: CTRL/CMD + Z
    * **Redo**: CTRL/CMD + Shift + Z-->

## Skapa poster genom att ansluta dem från ett annat program

Du kan importera poster från andra program genom att länka dem till poster som är länkade till Maestro. Detta skapar en Maestro-posttyp för det anslutna objektet från tredjepartsprogrammet. Poster som du ansluter till de ursprungliga Maestro-posterna visas i det tredjepartsprogram som är anslutet till objektet Maestro-posttyptabellvy.

1. Skapa en Maestro-posttyp enligt beskrivningen i [Skapa posttyper](../architecture/create-record-types.md).

1. Skapa Maestro-poster för den posttyp du skapade i föregående steg. Mer information finns i avsnittet [Skapa poster genom att lägga till dem manuellt till en posttyp](#create-records-by-manually-adding-them-to-a-record-type) i den här artikeln.

1. Skapa en anslutning till en objekttyp från ett tredjepartsprogram för den Maestro-posttyp som du har skapat. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).

1. Lägg till poster från tredjepartsprogrammet i de Maestro-poster som du skapade ovan med hjälp av det länkade postfältet som du skapade i föregående steg. Mer information finns i [Koppla poster](../records/connect-records.md).

   Följande objekt skapas i Maestro:

   * En skrivskyddad Maestro-posttyp som refererar till den posttyp från tredje part som du länkade till i det anslutna postfältet.

     Om du t.ex. ansluter en Maestro-posttyp till Workfront-projekt skapas en skrivskyddad posttyp med namnet&quot;Workfront projects&quot; i samma arbetsyta.
   * Skrivskyddade poster på posttypssidan från tredje part. Posterna som importeras från tredjepartsprogrammet förblir skrivskyddade och kan bara uppdateras i det ursprungliga programmet.

## Skapa poster genom att kopiera och klistra in information från en extern lista

1. Börja skapa poster i tabellvyn i maestro, vilket beskrivs i avsnittet [Skapa poster genom att lägga till dem manuellt till en posttyp](#create-records-by-manually-adding-them-to-a-record-type) i den här artikeln.

   Kontrollera att tabellvyn i maestro innehåller kolumnerna (eller fälten) som du vill fylla med den nya postinformationen i.

1. Klicka **Nytt &lt; Posttypnamn >** i den sista raden i tabellen för att lägga till så många nya rader i tabellen som du vill att de nya posterna ska vara.

   Lägg till exempel till 10 rader i tabellvyn om du vill klistra in informationen för 10 nya poster från ett annat program.

1. Skapa en lista med poster som du vill importera i Maestro i ett annat program.

   Du kan t.ex. använda ett Excel-kalkylblad för att skapa en lista.

   Listan bör innehålla information i tabellformat.

   >[!TIP]
   >
   > Kolumnerna i listan bör innehålla information om de fält du har i Maestro.
   >
   > Se till att du redan har skapat önskade fält i Maestro och att informationen i bladet visas i rätt format som matchar fälten i Maestro.

1. I tredjepartsprogrammet markerar du flera rader och kolumner och klistrar sedan in informationen i posttypstabellvyn, med början från den första nya posten.

   Följande information importeras till Maestro:

   * Raderna innehåller de nya posterna
   * Kolumnerna fyller i information för posternas fält.
