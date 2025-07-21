---
title: Konfigurera funktioner för arbetsytan mellan arbetsytor för posttyp
description: Du kan aktivera en posttyp som antingen ska läggas till på en annan arbetsyta eller anslutas från en annan arbetsyta.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 943c26efa6f6351abf885dbc5f3aa09c0b0fab05
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# Konfigurera funktioner för olika arbetsytor för posttyper

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Du kan ange att en posttyp ska läggas till på en annan arbetsyta eller anslutas från en annan arbetsyta i Adobe Workfront Planning.

Du måste först definiera funktionerna för en posttyps arbetsyta innan arbetsytehanterare kan ansluta den från eller importera den till andra arbetsytor.

Du definierar arbetsytefunktionerna för en posttyp när du skapar eller redigerar en posttyp.

Mer information finns i följande artiklar:

* [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md)
* [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

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
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera tillägg av en posttyp till andra arbetsytor

Som arbetsytehanterare kan du konfigurera en posttyp som ska läggas till i andra arbetsytor när du skapar eller redigerar en posttyp.

När du konfigurerar att lägga till en posttyp till andra arbetsytor kan en arbetsytehanterare importera posttypen och all information om den till någon av de arbetsytor som de hanterar.

Så här konfigurerar du att lägga till en posttyp på en annan arbetsyta när du redigerar posttypen:

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill redigera.

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll pekaren över kortet för en posttyp och klicka på menyn **Mer** ![Mer](assets/more-menu.png) i det övre högra hörnet av posttypskortet
eller
   * Klicka på ett posttypskort för att öppna posttypssidan och klicka sedan på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om posttypens namn.
1. Klicka på **Redigera**.

   ![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card.png)

1. I rutan **Redigera posttyp** väljer du fliken **Avancerade inställningar** .
1. Aktivera inställningen **Tillåt att den här posttypen läggs till i andra arbetsytor**.

   ![Redigera posttyp Avancerade inställningar med Lägg till i andra arbetsytor aktiverar](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. I fältet **Välj vem som kan lägga till den här posttypen i arbetsytor som de hanterar** lägger du till användare som du vill tillåta att den här posttypen läggs till i arbetsytor som de hanterar.

   Ditt namn läggs automatiskt till i fältet.

   Du kan lägga till enskilda användare, eller grupper, team, jobbroller eller företag vars användare du vill tillåta att den här posttypen läggs till på de arbetsytor som de hanterar.

   Du kan redigera det här fältet när du har sparat posttypen.
1. (Valfritt) Ta bort ditt namn från fältet **Välj vem som kan lägga till den här posttypen i arbetsytor som de hanterar**.

1. Klicka på **Spara**.

   Följande saker händer:

   * Posttypen och dess fält är nu tillgängliga och kan läggas till på en annan arbetsyta av de personer du har angett.

   >[!NOTE]
   >
   >Du kan bara redigera posttypen och dess fält från den ursprungliga arbetsytan.

   * På posttypskortet visas en global ikon, ![Global posttypsikon](assets/global-icon.png), som anger att posttypen är tillgänglig för alla arbetsytor vars hanterare du har angett i konfigurationen.
   * Ett systemgenererat **Workspace**-fält läggs till i posttypen.

     I fältet Workspace visas arbetsytan där varje post har skapats.

     Det här fältet är skrivskyddat och kan inte tas bort.

## Konfigurera anslutning till en posttyp från andra arbetsytor

Du kan konfigurera en posttyp att ansluta till från andra arbetsytor när du skapar eller redigerar posttypen.

Så här konfigurerar du en posttyp att ansluta till från andra arbetsytor när du redigerar posttypen:

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill redigera,

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll muspekaren över kortet för en posttyp och klicka på menyn **Mer** ![Mer](assets/more-menu.png) i det övre högra hörnet av posttypskortet och klicka sedan på **Redigera**
eller
   * Klicka på ett posttypskort för att öppna posttypssidan, klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Redigera**.

   ![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card.png)

1. I rutan **Redigera posttyp** väljer du fliken **Avancerade inställningar** .
1. Aktivera inställningen **Tillåt anslutning till den här posttypen i andra arbetsytor**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Redigera posttyp Avancerade inställningsflikar med anslutning från andra arbetsytor aktiverat](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   När det här alternativet är aktiverat är posttypen tillgänglig och kan anslutas från andra arbetsytor.

1. Välj från vilka arbetsytor som posttypen kan nås. Välj bland följande alternativ:

   * **Systemomfattande**: Användare kan ansluta till den här posttypen från alla arbetsytor där de har behörighet att hantera.
   * **Specifika arbetsytor**: Lägg till namnen på arbetsytorna där arbetsytehanterare kan ansluta till den här posttypen.
1. Klicka på **Redigera**.

   Följande saker händer:

   * Posttypen och dess fält är nu tillgängliga för anslutning från de arbetsytor du har angett.
   * Posttypkortet visar en ikon för anslutning mellan arbetsytor ![Anslutning mellan arbetsytor](assets/connect-from-other-workspaces-icon.png) som anger att posttypen är tillgänglig för anslutning från en arbetsyta som du har angett i konfigurationen.

   Posttypen blir tillgänglig för anslutning från de angivna arbetsytorna.









