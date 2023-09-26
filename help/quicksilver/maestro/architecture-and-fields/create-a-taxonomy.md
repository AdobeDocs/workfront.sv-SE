---
title: Skapa taxonomiposttyper
description: Taxonomier är en typ av återanvändbara posttyper som hämtar attribut om en operativ posttyp i Adobe Workfront Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Skapa taxonomiposttyper

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Taxonomier är posttyper som hämtar attribut om operativa posttyper i Adobe Maestro.

Campaign kan till exempel vara en operativ posttyp. Följande är taxonomier som samlar in attribut om posttypen Campaign: Region, Audience, Country.

Mer information om posttyper i Maestro finns i [Översikt över posttyper och taxonomier](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
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

## Att tänka på när du skapar taxonomier

* Du måste skapa en arbetsyta innan du kan skapa taxonomier på arbetsytan.

  Mer information om arbetsytor finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).
* Du kan skapa en taxonomiposttyp genom att göra något av följande:
   * Skapa dem automatiskt när du skapar en arbetsyta med hjälp av en mall. Mer information finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).
   * Skapa dem manuellt, från grunden.
   * Skapa dem manuellt genom att klistra in information från en extern lista.

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* Alla nya taxonomier innehåller följande fält:

   * Namn <!--if there won't be any more fields, consider rephrasing this-->

  Dessutom kan du lägga till anpassade fält i taxonomier. Mer information finns i [Skapa fält](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    Taxonomier som skapas när en arbetsytemall används har ytterligare fält.

## Skapa en taxonomi

Att skapa taxonomier påminner om att skapa en operativ posttyp från grunden eller från en arbetsytemall.

Mer information finns i avsnittet&quot;Skapa en posttyp från grunden&quot; i artikeln [Skapa posttyper](../architecture-and-fields/create-record-types.md).

Mer information om hur du skapar taxonomier automatiskt när du skapar en arbetsyta från en mall finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).
