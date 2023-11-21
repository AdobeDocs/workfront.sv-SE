---
title: Lista över arbetsytemallar
description: En arbetsyta är en samling driftsposttyper och taxonomier som används av ett team och som representerar teamets arbetslivscykel. Maestro har en uppsättning mallar som hjälper dig att komma igång med grundläggande posttyper, taxonomier och fält när du skapar arbetsytan.
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: c4758b87-45dc-4ffd-b086-5e2e907bdf34
source-git-commit: 6d1d3d82e15f4232ff81294d9094c2683b01ca89
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: List of available workspace templates
description: You can use templates to create workspaces. This article provides a list of available workspace templates
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
---

-->

# Lista över arbetsytemallar

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

I Adobe Maestro är en arbetsyta en samling posttyper och taxonomier som används av ett team och som representerar teamets arbetslivscykel.

Maestro har en uppsättning mallar som hjälper dig att komma igång med grundläggande posttyper, taxonomier och fält när du skapar arbetsytan. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

I den här artikeln beskrivs de arbetsytemallar som finns i Maestro.

## Att tänka på när det gäller Maestro-mallar

* Varje mall innehåller en uppsättning driftsposttyper och taxonomier. Mer information finns i [Översikt över posttyper och taxonomier](../architecture/overview-of-record-types-and-taxonomies.md).
* Varje driftsposttyp och taxonomi innehåller en uppsättning fält. Vissa av dessa fält är anslutningar till andra Maestro-posttyper.
* Du kan anpassa alla mallar.

<!-- I modeled this article by the "List of available Blueprints" and that articles does not have an Access area

## Access requirements

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

-->

## Mallar för maestro-arbetsytan

Här följer några exempel på arbetsytemallar i Maestro och antalet fält de innehåller:

* **Marknadsföringshantering**: Ni kan hantera alla era marknadsföringskampanjer med den här mallen. Mallen innehåller följande:

   * Operativa posttyper:

      * **Marknadsföringsplan**: 7 fält och 5 länkade fält
      * **Campaign**: 9 fält och 7 länkade fält
      * **Program**: 9 fält och 5 länkade fält
      * **Aktivitet**: 6 fält och 5 länkade fält
   * Taxonomier:
      * **Målgrupp**: 3 fält och 3 länkade fält
      * **Segment**: 5 fält och 1 länkat fält
      * **Kundresa**: 4 fält
      * **Erbjudande**: 3 fält och 1 länkat fält
      * **Län**: 1 fält
      * **Taktisk**: 1 fält
      * **Kanaler**: 1 fält och 1 länkat fält
      * **Affärsenhet**: 1 fält
      * **Funktion**: 1 fält

* **Försäljningshantering**: Du kan skapa ett omfattande säljsystem som effektiviserar säljprocessen och ökar effektiviteten. Mallen innehåller följande:

   * Operativa posttyper:

      * **Möjligheter**: 7 fält och 4 länkade fält
      * **Aktivitet**: 4 fält och 5 länkade fält
      * **Campaign**: 5 fält och 3 länkade fält
   * Taxonomier:
      * **Konto**: 4 fält och 3 länkade fält
      * **Lead**: 12 fält och 2 länkade fält
      * **Kontakt**: 10 fält och 2 länkade fält
      * **Län**: 1 fält och 2 länkade fält
      * **Bransch**: 1 fält
      * **Buying Center**: 1 fält
      * **Produkt/tjänst**: 1 fält
      * **Konkurrens**: 1 fält

* **Produkthantering**: Du kan skapa en effektiv och strukturerad produkthanteringsprocess med den här mallen. Mallen innehåller följande:

   * Operativa posttyper:

      * **Tema**: 8 fält och 2 länkade fält
      * **Initiative**: 8 fält och 2 länkade fält
      * **Epic**: 9 fält och 3 länkade fält
      * **Användarberättelse**: 9 fält och 2 länkade fält

   * Taxonomier:

      * **Kund**: 6 fält och 1 länkat fält
      * **Sprint**: 7 fält och 1 länkat fält
      * **Produktgrupp**: 3 fält
      * **Funktionsförfrågningar**: 8 fält och 1 länkat fält
      * **Bransch**: 1 fält och 1 länkat fält
