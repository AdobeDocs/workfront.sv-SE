---
title: Lägg till befintliga posttyper
description: Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du importera en befintlig posttyp från en annan arbetsyta.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Lägg till befintliga posttyper

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Som arbetsytehanterare kan du importera eller lägga till en befintlig posttyp till en annan arbetsyta.

Du måste ange en posttyp som centraliserad innan arbetsytehanterare kan importera den till andra arbetsytor.

Du kan ange en posttyp som centraliserad när du skapar eller redigerar den, medan du definierar dess inställningar för arbetsytan.

Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

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
   <td role="rowheader"><p>Adobe Workfront-paket*</p></td> 
   <td> 
<ul><li><p>Alla Workfront-paket</p></li>
Och
<li><p>Planering Plus-paket</p></li></ul>
Eller:
<ul><li><p>Alla arbetsflödespaket</p> </li>
Och
<li><p>Planera Prime- eller Ultimate-paket</p></li></ul>
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Översikt över centraliserade posttyper

Att tänka på när du lägger till befintliga posttyper från en annan arbetsyta

* När det inte finns några konfigurerade posttyper som ska läggas till på en annan arbetsyta visas inte alternativet att importera dem från en annan arbetsyta när du skapar en posttyp. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* När du har lagt till posttypen från en annan arbetsyta läggs även följande information till från den befintliga posttypen:

   * Fält
   * Postanslutningar

* Du kan bara visa poster som lagts till från andra arbetsytor om du har behörighet till dessa arbetsytor.

* Du kan bara redigera posttypen, inklusive dess fält, på den ursprungliga arbetsytan. Du kan inte redigera den från arbetsytorna där den lades till.
* Poster som läggs till från alla arbetsytor visas för alla användare som kommer åt dem från alla arbetsytor, även om de skapas i en arbetsyta där de inte har någon behörighet.

## Skapa en posttyp från en befintlig posttyp

1. Börja skapa en posttyp enligt beskrivningen i artikeln [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md) och klicka sedan på **Lägg till befintlig**. <!--check this - the option might have been renamed in the UI-->

   ![Modal för att lägga till posttyp med möjlighet att importera från en annan arbetsyta](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Klicka på **Fortsätt**.
1. I rutan **Välj posttyp** klickar du på kortet för den posttyp som du vill lägga till från en befintlig arbetsyta och sedan på **Lägg till**.

   Posttypen läggs till på arbetsytan som du valde och följande saker händer:

   * Posttypen **för** arbetsytan  ikon ![Anslutningsikonen för arbetsytan](assets/global-icon.png) läggs till på kortet för den importerade posttypen.
   * Det skrivskyddade fältet **Workspace** läggs till i den importerade posttypen. Fältet visar vilken arbetsyta varje post skapades i.

     >[!NOTE]
     >
     >* Du kan inte redigera den importerade posttypen eller dess fält. Du kan redigera posttypen och dess fält från den ursprungliga arbetsytan.

1. (Valfritt) Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) på den importerade posttypens kort, eller till höger om posttypens namn på sidan, och klicka sedan på **Ta bort**.
1. (Villkorligt) Skriv **delete** i det angivna fältet och klicka sedan på **Ta bort permanent**.

   Detta tar bort den importerade posttypen från den markerade arbetsytan. Den ursprungliga posttypen och dess fält finns kvar på den ursprungliga arbetsytan.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



