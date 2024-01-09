---
title: Dela poster
description: Du kan dela poster med andra för att öka samarbetet.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Dela poster

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Om du vill samarbeta med andra användare kan du dela poster med andra.

Du kan dela en Maestro-post på följande sätt:

* Kopiera länken till detaljsidan för en post från webbläsaren när sidan är öppen.

* Kopiera en länk till postens informationssida när du visar poster i posttypens tabellvy.

<!-- Update with this when we release permissions: 

* You can share all records in a workspace with other users by sharing the workspace. For more information, see [Grant access to Adobe Maestro](../access/grant-access.md).
-->

I den här artikeln beskrivs hur du kan kopiera en länk till en posts detaljsida från tabellvyn för en posttyp.

<!-- add information about permissions, like:
- in the table below, you must have at least View permissions to the record
- the user you're sharing with must have at least View permissions to the record to view it
- etc - others???-->

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
After permissions - replace the table with - below
****AND - see more above, another bullet point to update when permissions are released****

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
   <td> <p>View or higher permissions to a workspace</a> </p>  
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

## Dela postlänkar från posttypstabellvyn

{#step1-to-maestro}

Arbetsytan som du senast öppnade öppnas.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Från **Visa** Välj en tabellvy i den nedrullningsbara menyn i tabellens övre högra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Högerklicka på en postrad

   eller

   Håll muspekaren över en posts namn och klicka på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Kopiera länk**.

   ![](assets/contextual-menu-for-record-row.png)

   Länken kopieras till Urklipp.

1. Klistra in länken i ett e-postmeddelande eller i ett chattfönster om du vill dela den med andra användare. När användarna får länken öppnas postens informationssida.

   >[!TIP]
   >
   >Fälten för posten på detaljsidan är samma fält som är tillgängliga i postens tabellvy.


   <!--add there when it will be available: if they have access to this record-->
