---
title: Skapa Workspace Hierarkier
description: Som arbetsytehanterare kan du skapa flera arbetsytehierarkier mellan posttyperna i Adobe Workfront Planning. När du har anslutit posttyper på en arbetsyta och skapat en hierarki, kopplas posttyperna till varandra, med en posttyp som angetts som överordnad och upp till 6 andra posttyper som konfigurerats som underordnade.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '917'
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

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Som arbetsytehanterare kan du skapa flera arbetsytehierarkier mellan posttyper i Adobe Workfront Planning.

När posttyperna har anslutits inom en arbetsyta kan du skapa en hierarki som organiserar dessa anslutningar. Hierarkier organiserar post- och objekttyper i överordnade och underordnade relationer och kan innehålla upp till fyra nivåer med objekttyper.

Om det inte redan finns en anslutning mellan två posttyper kan den skapas när du skapar hierarkin. När hierarkin har definierats skapar den en strukturerad sökväg över relaterade posttyper på arbetsytan.

Hierarkier genererar vägbeskrivningar för posttyperna och deras respektive poster <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> som visas i deras rubriker. På så sätt vet användarna var de befinner sig i hierarkin i vilket skede som helst i arbetsflödet.

Allmän information om hierarkier och vägbeskrivningar finns i [Översikt över hierarki och vägbeskrivningar](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Åtkomstkrav

<!--check the access to see if you oversimplified???-->

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
1. Klicka på **Lägg till objekt** och välj en objekttyp i listrutan. Detta blir den första objekttypen i hierarkin. <!--logged bug to correct to "Add object type"-->

   Den första objekttypen kan bara vara en Planning-posttyp.

   Workfront-projekt kan inte väljas som överordnade objekt för andra objekttyper i en hierarki.

1. Klicka på **Lägg till objekt** om du vill lägga till en andra objekttyp, som är den första underordnade i hierarkin, och välj sedan en annan objekttyp i listrutan.
Varje ytterligare objekttyp blir underordnad till föregående objekttyper.

   ![Ny hierarkiruta utan markerat fält](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. Klicka på **Välj anslutet fält** för att ange vilket fält som ska kopplas till de två objekten.
1. (Villkorligt) Om det finns flera anslutningsfält väljer du ett i listan,

   eller

   Klicka på **Lägg till ny anslutning** för att lägga till ett nytt anslutningsfält.

   Detta skapar ett anslutningsfält från den posttyp som du använder som överordnad och ett motsvarande anslutningsfält till det från den posttyp som du använder som underordnad.

   Om du skapar en anslutning till Workfront-projekt skapas inget fält i projektet.

1. (Villkorligt) Om det inte finns några tillgängliga anslutna fält klickar du på **Skapa anslutning** och lägger till en ny anslutning. Klicka sedan på **Spara**.

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

      Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

   1. Klicka på **Spara**.

1. (Villkorligt) Om **Skapa motsvarande fält för den länkade posttypen** inte markerades när det anslutna fältet skapades, får du ett fel och måste göra följande först: <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. Klicka på **Avbryt** i rutan **Ny hierarki**.
   1. Klicka på bakåtpilen till vänster om arbetsytans namn och klicka sedan på kortet för den posttyp som du vill välja som överordnad.
   1. Öppna tabellvyn för den posttyp som du valde i steget ovan, gå till anslutningsfältet med den objekttyp som du vill använda som underordnad, hovra över kolumnrubriken och klicka sedan på fältet **Redigera**.
   1. Aktivera inställningen **Skapa motsvarande fält för länkad posttyp** och klicka sedan på **Spara**.
   1. Återgå till arbetsytans **inställningsområde** och klicka på **Ny hierarki** igen. Följ sedan stegen för att skapa en hierarki.

1. (Valfritt) Fortsätt lägga till upp till fyra objekttyper i hierarkierna enligt stegen ovan. Du kan lägga till alla objekttyper först och sedan lägga till anslutningsfälten mellan dem.
1. (Valfritt) Klicka på ikonen **Ta bort** ![Ta bort &#x200B;](assets/minus-icon.png) för att ta bort en anslutning.
1. Klicka på **Spara** för att spara hierarkin.

   >[!TIP]
   >
   >Knappen **Spara** är nedtonad om du inte har alla anslutna fält på plats.

   Följande saker händer:

   * Hierarkin läggs till i avsnittet **Hierarkier** på arbetsytan.
   * Posterna som fyller i anslutningsfälten visar alla anslutningar i sina vägbeskrivningar när du går till en posts sida.
1. (Valfritt) Hovra över en hierarki och klicka sedan på menyn **Mer** .

   ![Menyn Mer om hierarki har utökats](assets/hierarchy-more-menu-expanded.png)

1. Klicka på något av följande:

   * **Redigera**: Då öppnas rutan **Redigera hierarki** där du kan göra ändringar.
   * **Ta bort**: Detta tar bort hierarkin permanent. Det går inte att återställa borttagna hierarkier. Anslutningsfält tas inte bort.





