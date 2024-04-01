---
title: Skapa arbetsytor
description: En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning. Posttyperna är ordnade efter avsnitt på en arbetsyta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: eaf1cd4142b83a42d068e2d02fe673fa4dd25769
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Skapa arbetsytor

{{maestro-important-intro}}

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
<p>Din organisation måste vara registrerad i ett betaprogram som är stängt för Adobe Workfornt-planering. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <td> <p>Du måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när det gäller arbetsytor

* Du kan skapa arbetsytor för specifika organisationsenheter inom organisationen, så att de matchar det unika sätt som varje enhet fungerar på.
* De posttyper som en arbetsyta innehåller bör återspegla arbetslivscykeln för en organisationsenhet.
* När du skapar en arbetsyta är det bara du som har behörighet att komma åt och hantera arbetsytan. Du måste dela det med andra användare för att de ska kunna samarbeta med dig på samma plats. Mer information finns i [Dela en arbetsyta](/help/quicksilver/maestro/access/share-workspaces.md). Systemadministratörer kan hantera alla arbetsytor, även de som de inte skapade.
* Du kan ha följande:

   * Upp till 50 avsnitt på en arbetsyta.
   * Upp till totalt 1 000 posttyper från alla avsnitt på en arbetsyta. Alla posttyper är unika för varje arbetsyta. <!--this might change-->
   * Upp till 1 000 arbetsytor i din organisations Workfront-instans.


## Skapa en arbetsyta

{{step1-to-maestro}}

1. (Villkorligt) Om du inte har några arbetsytor i din miljö klickar du på **Skapa arbetsyta**

   Du kan också klicka på nedåtpilen till höger om arbetsytans namn från en befintlig arbetsyta och sedan klicka på **Skapa arbetsyta**.

   ![](assets/workspace-drop-down-right-menu.png)

   Detta öppnar arbetsyteområdet i Workfront Planning.
1. (Valfritt och villkorligt) Klicka på **Förhandsgranska** i någon av följande fördefinierade arbetsytemallar:

   * Marknadsföringshantering
   * Försäljningshantering
   * Produkthantering

   Det finns en indikation på vilka operativa posttyper, taxonomier och hur många fält som är associerade med varje mall.

   ![](assets/previewing-a-workspace-template.png)

   Mer information om mallar för arbetsytan i Workfront Planning finns i [Lista över arbetsytemallar](../architecture/workspace-templates.md).

1. Klicka **Använd mall** för att börja skapa arbetsytan från den valda mallen

   eller

   Klicka **Skapa arbetsyta** för att skapa en arbetsyta från grunden.

   En av följande typer av arbetsytor skapas:

   * En tom arbetsyta där du kan börja lägga till posttyper manuellt när du skapar en arbetsyta från grunden.
   * En arbetsyta med exempelposttyper som du kan anpassa ytterligare när du använder en av mallarna.

1. Klicka inuti arbetsytans namn i arbetsytans sidhuvud för den nya arbetsytan och tryck sedan på Retur

   eller

   Klicka på **Mer** meny ![](assets/more-menu.png)till höger om arbetsytans namn i sidhuvudet och klicka sedan på **Byt namn**.

1. (Valfritt och villkorligt) Om du har skapat arbetsytan från en mall klickar du inuti namnet på **Operativa posttyper** eller **Taxonomier** avsnitt

   eller

   Håll namnet på ett avsnitt och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Byt namn** för att byta namn på avsnittet.

   >[!TIP]
   >
   >Du kan byta namn på alla avsnitt på arbetsytan, även om du har skapat avsnittet.

1. (Valfritt) Gör något av följande om du vill ändra platsen för ett avsnitt:

   * Håll muspekaren över namnet på ett avsnitt och klicka på **ta** icon ![](assets/grab-icon.png)och sedan dra och släpp den på den högra platsen.
   * Håll muspekaren över namnet på ett avsnitt och klicka på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Flytta uppåt** eller **Flytta nedåt**. Avsnittet flyttas uppåt eller nedåt i arbetsytan.

1. (Valfritt) Gör något av följande om du vill lägga till ett nytt avsnitt:

   * Klicka **Lägg till avsnitt** längst ned på arbetsytan.
   * Håll muspekaren över namnet på ett avsnitt och klicka på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Lägg till avsnittet ovan** eller **Lägg till avsnitt nedan**.

1. (Valfritt) Klicka på **Lägg till posttyp** om du vill lägga till posttyper på arbetsytan i vilket avsnitt som helst.

   Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).

1. (Valfritt) Så här tar du bort ett avsnitt:

   1. Håll muspekaren över namnet på ett avsnitt och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Ta bort**. <!--add screen shot when UI is final?-->
   1. Markera ett nytt avsnitt som du vill flytta alla posttyper till och klicka sedan på **Ta bort**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Alla posttyper flyttas till urvalssektionen och avsnittet tas bort.
