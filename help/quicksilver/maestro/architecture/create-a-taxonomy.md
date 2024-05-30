---
title: Skapa taxonomiposttyper
description: När du använder en mall för att skapa en arbetsyta skapas posttyper i avsnitten operativa posttyper och taxonomier.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Skapa taxonomiposttyper

{{planning-important-intro}}

När du använder en mall för att skapa en arbetsyta skapas posttyper i följande avsnitt:

* Operativa posttyper
* Taxonomier

Posttyperna i avsnittet Taxonomier på en arbetsyta hämtar attribut om posttyper i avsnittet Operativa posttyper på samma arbetsyta.

Campaign kan till exempel vara en operativ posttyp. Följande är taxonomier som samlar in attribut om posttypen Campaign: Region, Audience, Country.

Mer information om posttyper finns i [Översikt över posttyper](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Om du vill ansluta posttyper till Experience Manager Assets måste du ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade
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

## Att tänka på när du skapar taxonomier

* Du måste skapa en arbetsyta med hjälp av en mall innan du kan skapa posttyper i avsnittet Taxonomier på arbetsytan.

  Mer information om arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).
* Du kan skapa en posttyp i avsnittet Taxonomier på en arbetsyta genom att göra något av följande:
   * Skapa dem automatiskt när du skapar en arbetsyta med hjälp av en mall. Mer information finns i [Skapa arbetsytor](../architecture/create-workspaces.md).
   * Skapa dem manuellt, från grunden, i taxonomiavsnittet på en arbetsyta.

* Alla nya taxonomier har som standard följande fält:

   * Namn
   * Beskrivning
   * Startdatum
   * Slutdatum
   * Status

  Dessutom kan du lägga till anpassade fält i taxonomier. Mer information finns i [Skapa fält](../fields/create-fields.md).

  >[!NOTE]
  >
  >    Taxonomiposttyper som skapas när en arbetsytemall används har ytterligare fält.

## Skapa en taxonomiposttyp

Att skapa taxonomiposttyper liknar att skapa posttyper.

Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).
