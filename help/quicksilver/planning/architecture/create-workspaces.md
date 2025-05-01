---
title: Skapa arbetsytor
description: En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning. Posttyperna är ordnade efter avsnitt på en arbetsyta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Skapa arbetsytor

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

I Adobe Workfront Planning är arbetsytorna centraliserade platser där team kan planera arbetet.

En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning.

Allmän information om arbetsytor finns i [Översikt över arbetsytor](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

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
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Du får behörigheten Hantera för de arbetsytor du skapar. </p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning.</p>
<p><span class="preview">I förhandsvisningsmiljön har standardanvändare och systemadministratörer Planering aktiverat som standard.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   ![Förhandsgranska en arbetsytemall](assets/previewing-a-workspace-template.png)

   Mer information om mallar för arbetsytan i Workfront Planning finns i [Lista över arbetsytemallar](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Klicka på **Använd mall** i förhandsgranskningsrutan för mallen för att börja skapa arbetsytan från den valda mallen

   eller

   Klicka på **Bakåt** och sedan på **Ny arbetsyta** för att skapa en helt ny arbetsyta.

   En av följande typer av arbetsytor skapas:

   * En tom arbetsyta med namnet **Namnlös Workspace** där du kan börja lägga till posttyper manuellt när du skapar en arbetsyta från grunden.
   * En arbetsyta som namnges efter mallen som du valde och som fylls med exempelposttyper. Du kan anpassa posttyperna och arbetsytan ytterligare.

   För Workfront-administratörer visas den nya arbetsytan på fliken **Arbetsytor som jag är på**.

   För alla andra användare som kan skapa arbetsytor visas den nya arbetsytan i området **Arbetsytor**.

1. Klicka i namnet på arbetsytan i sidhuvudet på den nya arbetsytan för att byta namn på den och tryck sedan på Retur.

1. (Valfritt och villkorligt) Om du har skapat arbetsytan från en mall klickar du inuti namnet på **driftposttyperna** eller **taxonomierna** .

   eller

   Håll namnet på ett avsnitt, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Byt namn** för att byta namn på avsnittet.

   >[!TIP]
   >
   >Du kan byta namn på alla avsnitt på en arbetsyta, även om du inte har skapat avsnittet.

   Mer information om hur du redigerar arbetsytor, inklusive redigering av arbetsytor, finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Valfritt) Klicka på **Lägg till posttyp** om du vill lägga till posttyper på arbetsytan i valfritt avsnitt.

   Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Mer information om hur du redigerar och tar bort posttyper på en arbetsyta finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).


