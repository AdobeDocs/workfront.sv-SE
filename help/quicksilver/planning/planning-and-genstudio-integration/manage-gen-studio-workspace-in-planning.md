---
title: Hantera GenStudio Workspace i Adobe Workfront Planning
description: GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna och din instans av Workfront är integrerad med ditt företags instans av GenStudio. Du kan visa arbetsytan i GenStudio från Planning och uppdatera information i båda systemen.
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '928'
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

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Adobe GenStudio for Performance Marketing arbetsyta är tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna och din instans av Workfront är integrerad med ditt företags instans av GenStudio.

Du kan visa arbetsytan i GenStudio från Planning och uppdatera information i båda systemen.

Information om hur du använder och hanterar GenStudio-arbetsytan från GenStudio Performance Marketing finns i [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/home).

Allmän information om integrationen mellan GenStudio och Workfront Planning finns i [Kom igång med Adobe Workfront Planning och Adobe GenStudio for Performance Marketing-integrering](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla Adobe Workfront Workflow-paket</p>
<p>Alla Adobe Workfront Planning-paket</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio package</p></td> 
   <td> 
<p>?? HAR GEN STUDIO ETT PAKET SOM STÖDER DET HÄR??</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio-licens</p></td> 
   <td><p> ?? KRÄVER GEN STUDIO EN SPECIFIK LICENS SOM STÖDER DETTA??</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> Ytterligare produkter</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>  
   <p>Konfiguration för GenStudio: ???VAD ÄR BEHOVET AV ÅTKOMSTNIVÅ FÖR GENS???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter*</p></td> 
   <td>  
   <p>I Workfront Planning: </p>
   <ul>
   <li><p>Contribute eller högre behörighet för en arbetsyta och en posttyp  </p> </li> 
   <li><p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p></li>
   </ul>
   <p>I Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Alla behörigheter i Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Skapa behörigheter i Adobe GenStudio for Performance Marketing för att skapa objekt</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Mer information om Adobe GenStudio for Performance Marketing finns i [Adobe GenStudio for Performance Marketing användarhandbok](https://experienceleague.adobe.com/sv/docs/genstudio-for-performance-marketing/user-guide/home).

+++   

## Att tänka på när du hanterar en GenStudio-arbetsyta i Workfront Planning

* Din organisation måste köpa Adobe GenStudio for Performance Marketing innan du kan visa en GenStudio-arbetsyta i Workfront Planning.

* Workfront-användare måste ha tillgång till GenStudio för att kunna se GenStudio arbetsyta i Workfront Planning.

* Du kan uppdatera följande information om en GenStudio-arbetsyta i Workfront Planning:

   * Redigera arbetsyteinställningarna <!--check to see if this is correct? is this editable or read only from Planning??-->
   * Redigera posttyperna och deras fält <!--check on this-->
   * Dela, redigera och lägga till vyer
   * Lägg till nya posttyper
   * Redigera, lägga till eller ta bort poster

* Uppdateringen av arbetsytans konfiguration, posttyper, vyer och fält för en GenStudio-arbetsyta är identisk med uppdateringen av en Workfront Planning-arbetsyta med dess element.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Hantera posttyper från GenStudio från Workfront Planning

>[!NOTE]
>
>Läs artikeln [Kom igång med Workfront Planning och GenStudio for Performance Marketing-integrering](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) innan du hanterar arbetsytan i GenStudio.

1. Logga in på Workfront som användare som även har tillgång till GenStudio.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Planning]**.

   Huvudsidan för Workfront Planning öppnas.

1. Klicka på **Andra arbetsytor** och hitta en arbetsyta som har en indikation som skapades av **System** och som har **GenStudio** -taggen på kortet.

   ![GenStudio-arbetsytans kort med taggen ](assets/genstudio-card-with-tag-highlighted.png)

1. Klicka på **arbetsytekortet för GenStudio** för att öppna arbetsytan för GenStudio i Workfront Planning.
1. Som standard skapas och visas följande posttyper för GenStudio från Workfront Planning:

   * Kampanjer
   * Produkter
   * Aktiveringar
   * Kanaler
   * Regioner

   Det finns en indikation på GenStudio-postens typkort att de ursprungligen skapades i GenStudio.

   <!--check screen shot-->

   ![GenStudio-posttypkort med taggen ](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Klicka på något av posttypskorten för att visa poster för den typen.

1. Gör något av följande:

   * Klicka på **Dela** i det övre högra hörnet på posttypsidan och klicka sedan på något av följande:
      * **Kopiera vylänken** om du vill dela en länk till posttypen
      * **Exportera den aktuella vyn** för att exportera den till en CSV- eller Excel-fil.
Du kan bara exportera tabellvyn. <!--check on this later; is this true or are there more options in the Share button-->

   * Klicka på **+ Visa** för att skapa en vy för posttypen GenStudio.

     Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   * Klicka på ikonen **Helskärm** ![Öppna helskärmsikonen](assets/open-full-screen-icon.png) om du vill öppna en vy i helskärmsläge.

   * Hantera element i en vy från alla vyer.

     Du kan t.ex. ändra filtret, grupperingarna, sorteringen och inställningarna för en vy, där det är tillgängligt.

     Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   * Lägg till poster i tabellen eller tidslinjevyn.

     Du kan bara skapa poster från grunden eller genom att importera en CSV- eller Excel-fil.

     Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

     Poster visas både från Workfront och GenStudio.

   * Redigera poster i tabellvyn eller klicka på en post för att öppna informationssidan.

     Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

   * Ta bort poster i tabellvyn.

     Mer information finns i [Ta bort poster](/help/quicksilver/planning/records/delete-records.md).

     Borttagna poster kan återställas från papperskorgen i Workfront Planning om de tas bort från Workfront.

     Mer information finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md)

   * Håll markören över ett fält i tabellvyn om du vill sortera eller dölja fältet.

     >[!NOTE]
     >
     >Du kan bara redigera ett fälts konfiguration och lägga till fler fält när du har behörigheten Hantera i GenStudio. <!--check to see if this is true??-->
