---
title: Åtkomstöversikt
description: Alla användare i en organisation har tillgång till Adobe Maestro. För närvarande finns det inga åtkomstnivåer eller behörigheter kopplade till användare eller informationen i Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 50e6b09d626325ee2836dc0ebaf79fc1e8cc9da9
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

# Åtkomstöversikt

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att få tillgång till Maestro.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Adobe Maestro har inga åtkomstnivåbegränsningar.

Alla användare i organisationen kan ha tillgång till Maestro, oavsett åtkomstnivå.

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

## Åtkomstkrav

Du måste ha följande för att kunna använda Adobe Maestro:

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt.  </p>
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
   <td role="rowheader"><p>Åtkomstnivå</p></td>
   <td> <p>Alla</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Din Workfront-administratör måste lägga till Maestro-området på huvudmenyn i din layoutmall.</p> 
   <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Anpassa huvudmenyn med hjälp av en layoutmall</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--After we enable permissions, replace the section content above with this:

There are license and sharing permission restrictions to use Adobe Maestro capabilities. (*********** this should be the intro right under the title; also update the metadata with this when live*******)

You must have the following settings to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement*</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p>
   To create workspaces, users must have the following license: 
   <ul><li><p>New: Standard</p> </li>
   <li><p>Current: Worker or higher</p> </li></ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Maestro objects</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Contribute or higher permissions to workspaces and views that you did not create to edit, delete, and share them</p>
    <p>System Administrators can manage workspaces and views they did not create </p>
   <p>For information about sharing permissions for Maestro objects, see  
   <a href="../access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Maestro</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your system administrator must add the Maestro area in the Main Menu to your layout template.</p> 
   <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*To find out your Workfront plan, license, or access level, contact your Workfront administrator. 

-->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Dela Maestro-området på huvudmenyn med andra

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

När din organisation har registrerats i betaprogrammet för Maestro kan du lägga till Maestro-området på huvudmenyn för alla användare med hjälp av en layoutmall.

1. Logga in på **Workfront** som Workfront-administratör.

1. Lägg till **Maestro** icon ![](assets/maestro-icon.png) till **Huvudmeny** med **Layoutmall**.

   Mer information finns i [Anpassa huvudmenyn med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Tilldela layoutmallen till de användare som du vill ska ha tillgång till Maestro.

   Mer information finns i [Tilldela användare till en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alla användare som är tilldelade mallen kan nu komma åt Maestro på huvudmenyn.

   Användare kan börja skapa arbetsytor, posttyper, poster och fält.

## Ge åtkomst

Det finns inga åtkomstkontroller för Maestro.

Användare med alla typer av licenser har tillgång till Maestro.

## Bevilja behörigheter

Det finns inga behörigheter associerade med Maestro-objekt.

Alla användare som har Maestro aktiverat i sin miljö kan visa, redigera och ta bort all information som andra användare lägger till i Maestro.

<!--
Take out the text above and replace with this: 

For more information, see [Access overview](/help/quicksilver/maestro/access/access-overview.md)-->


