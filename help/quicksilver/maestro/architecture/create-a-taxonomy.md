---
title: Skapa taxonomiposttyper
description: Taxonomier är en typ av återanvändbara posttyper som hämtar attribut om en operativ posttyp i Adobe Workfront Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Skapa taxonomiposttyper

{{maestro-important-intro}}

Posttyper i taxonomi hämtar attribut om operativa posttyper i Adobe Maestro.

Campaign kan till exempel vara en operativ posttyp. Följande är taxonomier som samlar in attribut om posttypen Campaign: Region, Audience, Country.

Mer information om posttyper i Maestro finns i [Översikt över posttyper och taxonomier](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Om du vill ansluta Maestro-posttyper till Experience Manager Assets måste du ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Din Workfront- eller gruppadministratör måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
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

* Du måste skapa en arbetsyta innan du kan skapa taxonomiposttyper på arbetsytan.

  Mer information om arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).
* Du kan skapa en taxonomiposttyp genom att göra något av följande:
   * Skapa dem automatiskt när du skapar en arbetsyta med hjälp av en mall. Mer information finns i [Skapa arbetsytor](../architecture/create-workspaces.md).
   * Skapa dem manuellt, från grunden.

* Alla nya taxonomiposttyper har följande fält:

   * Namn <!--if there won't be any more fields, consider rephrasing this-->

  Dessutom kan du lägga till anpassade fält i taxonomier. Mer information finns i [Skapa fält](../fields/create-fields.md).

  >[!NOTE]
  >
  >    Taxonomiposttyper som skapas när en arbetsytemall används har ytterligare fält.

## Skapa en taxonomiposttyp

Att skapa taxonomiposttyper påminner om att skapa operativa posttyper från grunden eller från en arbetsytemall.

Mer information finns i avsnittet&quot;Skapa en posttyp från grunden&quot; i artikeln [Skapa posttyper](../architecture/create-record-types.md).

Mer information om hur du skapar taxonomier automatiskt när du skapar en arbetsyta från en mall finns i [Skapa arbetsytor](../architecture/create-workspaces.md).
