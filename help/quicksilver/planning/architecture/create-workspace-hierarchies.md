---
title: Skapa Workspace Hierarkier
description: Som arbetsytehanterare kan du skapa flera arbetsytehierarkier mellan posttyperna i Adobe Workfront Planning. När du har anslutit posttyper på en arbetsyta och skapat en hierarki, kopplas posttyperna till varandra, med en posttyp som angetts som överordnad och upp till 6 andra posttyper som konfigurerats som underordnade.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Skapa arbetsytehierarkier

Som arbetsytehanterare kan du skapa flera arbetsytehierarkier mellan posttyperna i Adobe Workfront Planning.

När du har anslutit posttyper på en arbetsyta och skapat en hierarki, kopplas posttyperna till varandra, med en posttyp som angetts som överordnad och upp till 6 andra posttyper som konfigurerats som underordnade. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

Hierarkier genererar vägbeskrivningar för de posttyper och poster <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> som visas i deras rubriker. På så sätt vet användarna var de befinner sig i hierarkin i vilket skede som helst i arbetsflödet.

Allmän information om hierarkier och vägbeskrivningar finns i [Översikt över hierarki och vägbeskrivningar](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Åtkomstkrav

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ Expandera om du vill visa åtkomstkraven för att utföra stegen i den här artikeln:  

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
<ul> 
<li><p>Alla Workfront- och Planning-paket</p></li>
eller
<li><p>Alla arbetsflöden och alla planeringsdokument</p></li></ul>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta</p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en arbetsytehierarki

{#step1-to-planning}

1. Klicka på ett arbetsytekort.
1. Klicka på menyn **Mer** ![Mer meny](assets/more-menu.png) till höger om arbetsytans namn och klicka sedan på **Inställningar**.
Avsnittet **Hierarkier** öppnas som standard.
1. Klicka på **Ny hierarki** i det övre högra hörnet på sidan **Hierarkier** .
1. Klicka på **Lägg till objekt** och välj ett objekt i listrutan. Det här blir det överordnade objektet i din hierarki.
Du kan välja en posttyp på den aktuella arbetsytan eller ett projekt från Workfront.
1. Klicka på **Lägg till objekt** om du vill lägga till ett andra objekt, som är det första underordnade objektet i hierarkin, och välj sedan ett annat objekt i listrutan.
   ![Ny hierarkiruta utan markerat fält](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. Klicka på **Välj anslutet fält** för att ange vilket fält som ska kopplas till de två objekten.
1. (Villkorligt) Om det finns ett anslutet fält mellan de två objekttyperna väljer du det i listan. Annars klickar du på **Lägg till ny anslutning**.

   >[!WARNING]
   >
   >Om **Skapa motsvarande fält för den länkade posttypen** inte markerades när det anslutna fältet skapades måste du redigera fältet innan du kan fortsätta.

1. (Villkorligt) Om du lägger till en ny anslutning gör du följande:

   1. Lägg till ett namn för det anslutna fältet i rutan **Namn**.
   1. Välj mellan följande anslutningstyper:

      * **Många till många**
      * **En till många**
      * **Många till en**
      * **En till en**
   1. Välj någon av följande typer av postutseenden:

      * **Namn och bild**
      * **Namn**
      * **Bild**
Mer information finns i [Koppla samman posttyper ](/help/quicksilver/planning/architecture/connect-record-types.md) .
   1. Klicka på **Spara**.
1. (Valfritt) Fortsätt lägga till upp till fyra objekttyper i hierarkierna enligt stegen ovan. Du kan lägga till alla objekttyper först och sedan lägga till anslutningsfälten mellan dem.
1. (Valfritt) Klicka på ikonen **Ta bort** ![Ta bort ](assets/minus-icon.png) för att ta bort en anslutning.
1. Klicka på **Spara** för att spara hierarkin.

   >[!TIP]
   >
   >Knappen **Spara** är nedtonad om du inte har alla anslutna fält på plats.

   Följande saker händer:

   * Hierarkin läggs till i avsnittet **Hierarkier** på arbetsytan.
   * Posterna som fyller i anslutningsfälten visar alla anslutningar i sina vägbeskrivningar när du går till en posts sida.
1. (Valfritt) Hovra över en hierarki, klicka på menyn **Mer** och sedan på något av följande:

   * **Redigera**: Då öppnas rutan **Redigera hierarki** där du kan göra ändringar.
   * **Ta bort**: Detta tar bort hierarkin permanent. Det går inte att återställa borttagna hierarkier. Anslutningsfält tas inte bort.





