---
title: Hantera GenStudio Workspace i Adobe Workfront Planning
description: GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna och din instans av Workfront är integrerad med ditt företags instans av GenStudio. Du kan visa arbetsytan i GenStudio från Planning och uppdatera information i båda systemen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1355'
ht-degree: 0%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# Hantera GenStudio arbetsyta i Adobe Workfront Planning

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna och din instans av Workfront är integrerad med ditt företags instans av GenStudio.

Du kan visa arbetsytan i GenStudio från Planning och uppdatera information i båda systemen.

Information om hur du använder och hanterar GenStudio-arbetsytan från GenStudio Performance Marketing finns i [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/home).

Allmän information om integrationen mellan GenStudio och Workfront Planning finns i [Kom igång med Adobe Workfront Planning och Adobe GenStudio for Performance Marketing-integrering](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

>[!IMPORTANT]
>
>Stegen som beskrivs i den här artikeln visar hur du kan uppdatera arbetsytan i GenStudio från Workfront Planning när du har behörigheten Hantera.
> Alla funktioner är inte tillgängliga när du har Contribute-behörighet för GenStudio-arbetsytan.
>
>Om ditt företag har flera instanser av Workfront får alla användare Contribute-behörigheter på GenStudio-arbetsytan i Workfront Planning.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla Workfront- och Planning-paket</p>
<p>Alla arbetsflöden och alla planeringsdokument</p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
   <tr> 
<td> 
   <p> Ytterligare produkter</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing användarroller</p></td> 
   <td><p><ul><li>Alla GenStudio användarroller för att få tillgång till kampanjer, produkter och uppgifter</li>
   <li>GenSudio System Manager för att komma åt aktiveringar <!--and Events--></li></ul>
   Mer information finns i <a href="https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Användarroller och behörigheter</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  
   <p>I Workfront Planning: </p>
   <ul>
   <li><p>Hantera behörigheter på arbetsytan i GenStudio för att lägga till nya fält eller posttyper på arbetsytan i GenStudio</p></li>
   <li><p>Contribute-behörigheter på arbetsytan i GenStudio för att lägga till, uppdatera eller ta bort poster på arbetsytan i GenStudio</p> </li>  
   </ul>
   <p>Inga användare kan ta bort posttyper eller fält från GenStudio for Performance Marketing från GenStudio arbetsyta i Workfront Planning</p>
   <p>I Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Alla behörigheter i Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Skapa behörigheter i Adobe GenStudio for Performance Marketing för att skapa objekt</p></li></ul>
   </td>  
</tbody> 
</table>

Mer information om åtkomst till Adobe Workfront Planning finns i [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Mer information om Adobe GenStudio for Performance Marketing finns i [Adobe GenStudio for Performance Marketing användarhandbok](https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/home).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****** and Events*********</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Att tänka på när du hanterar en GenStudio-arbetsyta i Workfront Planning

* Din organisation måste köpa Adobe GenStudio for Performance Marketing innan du kan visa en GenStudio-arbetsyta i Workfront Planning.

* Beroende på hur många Workfront-instanser din organisation har, har du automatiskt följande behörigheter till arbetsytan i GenStudio under Planning:

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>En instans av Workfront</p></td> 
      <td> 
   <p>Arbetsytan i GenStudio visas i din instans av Workfront Planning</p>
   <p>Workfront-administratörer har behörigheten Hantera för GenStudio arbetsyta i Planning</p>
   <p>Alla andra användare har Contribute-åtkomst till GenStudio arbetsyta i Planning</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> Flera instanser av Workfront</p> </td> 
      <td> 
      <p>Arbetsytan i GenStudio är synlig från alla Workfront-instanser</p>
   <p>Alla användare med tillgång till GenStudio for Performance Marketing och Workfront Planning har Contribute-behörigheter i GenStudio vid Planning</p> </td> 
   </tr>
      </tbody> 
   </table>

* Uppdateringen av arbetsytans konfiguration, posttyper, vyer och fält för en GenStudio-arbetsyta är identisk med uppdateringen av en Workfront Planning-arbetsyta med dess element.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Hantera arbetsytan i GenStudio från Workfront Planning

>[!NOTE]
>
>Innan du hanterar arbetsytan i GenStudio bör du läsa artikeln [Kom igång med integreringen Workfront Planning och GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) för mer information.
>

1. Logga in på Workfront som användare som även har tillgång till GenStudio.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Planning]**.

   Huvudsidan för Workfront Planning öppnas.

1. Klicka på **Andra arbetsytor** och hitta en arbetsyta som har en indikation som skapades av **System** och som har **GenStudio** -taggen på kortet.

   ![GenStudio-arbetsytans kort med taggen &#x200B;](assets/genstudio-card-with-tag-highlighted.png)

1. Klicka på **arbetsytekortet för GenStudio** för att öppna arbetsytan för GenStudio i Workfront Planning.
1. Som standard skapas och visas följande posttyper för GenStudio från Workfront Planning:

   * Kampanjer
   * Produkter
   * Personas
   * Aktiveringar
   * Kanaler
   * Regioner

   Det finns en indikation på GenStudio-postens typkort att de ursprungligen skapades i GenStudio.

   <!--check screen shot-->

   ![GenStudio-posttypkort med taggen &#x200B;](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) till höger om arbetsytans namn och klicka sedan på något av följande:

   * **Redigera**

     Mer information finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. Klicka på **Dela** i det övre högra hörnet om du vill dela arbetsytan med andra.

   Mer information finns i [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)

   <!--
   >[!NOTE]
   >
   >You cannot remove GenStudio users from the GenStudio workspace, after you share that workspace with them.-->

1. Klicka på något av posttypskorten för att visa poster för den typen.

   Information om hur du hanterar posttyp, vyer och fält finns i avsnittet [Hantera GenStudio-posttyper från Workfront Planning](#manage-genstudio-record-types-from-workfront-planning) i den här artikeln.


## Hantera posttyper, vyer och poster från GenStudio arbetsyta i Workfront Planning

>[!NOTE]
>
>Innan du hanterar arbetsytan i GenStudio bör du läsa artikeln [Kom igång med integreringen Workfront Planning och GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) för mer information.
>

1. Gå till arbetsytan för GenStudio i Workfront Planning och öppna en posttypssida, enligt beskrivningen i avsnittet [Hantera arbetsytan för GenStudio från Workfront Planning](#manage-the-genstudio-workspace-from-workfront-planning) i den här artikeln.

1. Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) till höger om ett posttypsnamn och klicka sedan på något av följande:

   * **Redigera**

     Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).
   * **Hantera automatisering**

     Mer information finns i [Konfigurera Adobe Workfront Planning Automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).
   * **Hantera förfrågningsformulär**

     Du kan skapa flera frågeformulär. Ansökningsforumen finns i området Begäranden i Workfront och du kan även dela dem offentligt eller via en länk.

     Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

1. Så här delar du en vy eller posttyp:

   * Klicka på **Dela** i det övre högra hörnet på posttypsidan och klicka sedan på något av följande:
      * **Dela posttypen**
Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).
      * **Dela den aktuella vyn**
Mer information finns i [Dela vyer &#x200B;](/help/quicksilver/planning/access/share-views.md) .
      * **Kopiera vylänken**
En länk till vyn kopieras till Urklipp.
      * **Exportera den aktuella vyn**
Mer information finns i [Exportera poster från tabellvyn &#x200B;](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

        <!--
         >[!NOTE]
         >
         >You cannot remove GenStudio users from record types in the GenStudio workspace, after you share that workspace or the record types with them.-->

1. Så här hanterar du posttypsvyer:

   * Klicka på **+ Visa** för att skapa en vy för posttypen GenStudio.

     Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   * Klicka på ikonen **Helskärm** ![Öppna helskärmsikonen](assets/open-full-screen-icon.png) om du vill öppna en vy i helskärmsläge.

   * Hantera element i en vy från alla vyer.

     Du kan t.ex. ändra filtret, grupperingarna, sorteringen och inställningarna för en vy, där det är tillgängligt.

     Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

1. Gör något av följande om du vill lägga till poster:

   * Klicka på **Ny post** från valfri vy om du vill skapa poster från början

   * Importera poster med hjälp av en Excel- eller CSV-fil i tabellvyn

   * Klicka var som helst i tidslinjen eller kalendervyn för att lägga till poster.

     Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

     Poster visas både från Workfront och GenStudio.

     >[!NOTE]
     >
     >Du kan inte lägga till poster för posttypen Activations.

1. Gör något av följande om du vill redigera poster:

   * Redigera inline-poster från tabellvyn

   * Klicka på en post i valfri vy för att öppna informationssidan.

     Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

     De ändringar du gör på GenStudio arbetsyta i Planning visas direkt i GenStudio.

1. Markera en post i tabellvyn och klicka sedan på **Ta bort**.

   Mer information finns i [Ta bort poster](/help/quicksilver/planning/records/delete-records.md).

   Borttagna poster tas omedelbart bort från GenStudio.

   >[!TIP]
   >
   >Borttagna poster kan återställas från registervyn Bin i Workfront Planning har tagits bort nyligen. Poster som tas bort från GenStudio kan också återställas från behållaren för nyligen borttagna poster i Workfront Planning.

   Mer information finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md)

1. Klicka på ikonen + i tabellvyns övre högra hörn för att skapa följande:

   * Postfält

     Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md)

   * Postanslutningar

     Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md)

     Fält som skapas från arbetsytan i GenStudio visas i följande områden:

      * Workfront Planeringsvyer
      * Information om Workfront Planning-post
      * Information om GenStudio-post

     >[!TIP]
     >
     >Fält som skapas i Workfront Planning visas inte i listvyn i GenStudio.

     <!--when this releases, replace the tip above with this: 
      
      >[!NOTE]
      >
      >* Fields created in Workfront Planning are not visible in the list view in GenStudio.
      >
      >* You can connect any GenStudio record type to the Brands GenStudio record type. 
      >  Products and Personas are connected to Brands by default. -->

1. Håll pekaren över ett fält i tabellvyn och klicka sedan på listrutan för att göra något av följande:

   * Sortera efter
   * Dölj den
   * Redigera dess inställningar
     <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

     <!--GenStudio-native fields are note removed from GenStudio. -->

     >[!NOTE]
     >
     >Du kan bara redigera ett fälts konfiguration och lägga till fler fält när du har behörigheten Hantera i GenStudio.

