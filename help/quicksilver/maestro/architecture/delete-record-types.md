---
title: Ta bort posttyper
description: Du kan ta bort driftsposttyper eller taxonomiposttyper när de inte längre är relevanta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Ta bort posttyper

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan ta bort driftsposttyper eller taxonomiposttyper när de inte längre är relevanta.

Mer information om posttyper och taxonomier finns i [Översikt över posttyper och taxonomier](../architecture/overview-of-record-types-and-taxonomies.md).

Vi rekommenderar att du återskapar de fält och de poster som är kopplade till den posttyp eller taxonomi som du vill ta bort på en annan posttyp innan du tar bort dem.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
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

## Att tänka på när du tar bort posttyper

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Du kan ta bort alla posttyper och taxonomi som du eller någon i organisationen har skapat. <!--this will change with access levels and permissions-->
* När du tar bort posttyper tas all information som är kopplad till dem bort, inklusive fält och poster av den typen.
* Du kan inte återställa borttagna posttyper eller deras information.

## Ta bort posttyper

Att ta bort taxonomiposttyper är identiskt med att ta bort driftsposttyper.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i det övre högra hörnet av Workfront eller **Huvudmeny** icon ![](assets/main-menu-shell.png)  i det övre vänstra hörnet, om det är tillgängligt, klickar du på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill ta bort posttyper för.

   Arbetsytan öppnas och posttyperna och taxonomierna som är kopplade till den visas.
1. Klicka på kortet för den posttyp eller taxonomi som du vill ta bort.

   Då öppnas posttypens sida.
1. Klicka på **Mer** meny ![](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Ta bort**.
1. Klicka **Ta bort** för att bekräfta.

   Den valda posttypen eller taxonomin, tillsammans med fälten och tillhörande poster, tas bort.
