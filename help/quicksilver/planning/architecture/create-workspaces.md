---
title: Skapa arbetsytor
description: En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning. Posttyperna är ordnade efter avsnitt på en arbetsyta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Skapa arbetsytor

{{planning-important-intro}}

I Adobe Workfront Planning är arbetsytorna centraliserade platser där team kan planera arbetet.

En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning.

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Du får behörigheten Hantera för de arbetsytor du skapar. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Du måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när det gäller arbetsytor

* Du kan skapa arbetsytor för specifika organisationsenheter inom organisationen, så att de matchar det unika sätt som varje enhet fungerar på.
* De posttyper som en arbetsyta innehåller bör återspegla arbetslivscykeln för en organisationsenhet.
* När du skapar en arbetsyta är det bara du som har behörighet att komma åt och hantera arbetsytan. Du måste dela det med andra användare för att de ska kunna samarbeta med dig på samma plats. Mer information finns i [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md). Systemadministratörer kan hantera alla arbetsytor, även de som de inte skapade.
* Du kan ha följande:

   * Upp till 50 avsnitt på en arbetsyta.
   * Upp till totalt 1 000 posttyper från alla avsnitt på en arbetsyta. Alla posttyper är unika för varje arbetsyta. <!--this might change-->
   * Upp till 1 000 arbetsytor i din organisations Workfront-instans.


## Skapa en arbetsyta

Du kan skapa en arbetsyta och lägga till posttyper för att ordna dina objekt i Workfront Planning. Mer information om hur du redigerar en arbetsyta finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Klicka på **Skapa arbetsyta**

   Rutan Skapa arbetsyta visas. Du kan skapa en arbetsyta från grunden eller skapa den med någon av de tillgängliga mallarna.

1. (Valfritt och villkorligt) Klicka på **Förhandsgranska** i någon av följande fördefinierade arbetsytemallar:

   * Grundläggande: Marknadsföringshantering
   * Avancerat: Marknadsföringshantering
   * Enterprise: Marketing Management
   * Försäljningshantering
   * Produkthantering

   Förhandsvisningsrutan för mallen öppnas.

   Det finns en indikation på vilka operativa posttyper, taxonomier och hur många fält som är associerade med varje mall.

   ![](assets/previewing-a-workspace-template.png)

   Mer information om mallar för arbetsytan i Workfront Planning finns i [Lista över arbetsytemallar](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Klicka på **Använd mall** i förhandsgranskningsrutan för mallen för att börja skapa arbetsytan från den valda mallen

   eller

   Klicka på **Bakåt** och sedan på **Ny arbetsyta** för att skapa en helt ny arbetsyta.

   En av följande typer av arbetsytor skapas:

   * En tom arbetsyta med namnet **Namnlös Workspace** där du kan börja lägga till posttyper manuellt när du skapar en arbetsyta från grunden.
   * En arbetsyta som namnges efter mallen som du valde och som fylls med exempelposttyper. Du kan anpassa posttyperna och arbetsytan ytterligare.

1. Klicka i namnet på arbetsytan i sidhuvudet på den nya arbetsytan för att byta namn på den och tryck sedan på Retur.

1. (Valfritt och villkorligt) Om du har skapat arbetsytan från en mall klickar du inuti namnet på **driftposttyperna** eller **taxonomierna** .

   eller

   Håll namnet på ett avsnitt, klicka på menyn **Mer** ![](assets/more-menu.png) och klicka sedan på **Byt namn** för att byta namn på avsnittet.

   >[!TIP]
   >
   >Du kan byta namn på alla avsnitt på en arbetsyta, även om du inte har skapat avsnittet.

   Mer information om hur du redigerar arbetsytor, inklusive redigering av arbetsytor, finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Valfritt) Klicka på **Lägg till posttyp** om du vill lägga till posttyper på arbetsytan i valfritt avsnitt.

   Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Mer information om hur du redigerar och tar bort posttyper på en arbetsyta finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).


