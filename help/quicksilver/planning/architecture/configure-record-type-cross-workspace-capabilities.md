---
title: Konfigurera funktioner för arbetsytan mellan arbetsytor för posttyp
description: Du kan aktivera en posttyp som antingen ska läggas till på en annan arbetsyta eller anslutas från en annan arbetsyta.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Konfigurera funktioner för olika arbetsytor för posttyper

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Du kan konfigurera posttyper så att de fungerar på flera arbetsytor.

Följande är funktioner för olika arbetsytor för posttyper:

* Du kan ange en posttyp som centraliserad. Användarna kan lägga till centraliserade posttyper i andra arbetsytor som de kan hantera.
* Du kan ange en posttyp som en kopplingsbar typ. Användare kan ansluta till den här posttypen från andra arbetsytor.

Du måste först definiera funktionerna för en posttyps arbetsyta innan arbetsytehanterare kan ansluta den från eller lägga till den i andra arbetsytor.

Du definierar arbetsytefunktionerna för en posttyp när du skapar eller redigerar en posttyp.

Mer information finns i följande artiklar:

* [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md)
* [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md)

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
<ul><li><p>Alla Workfront-paket</p></li>
<p>Och</p>
<li><p>Planeringspaket för att skapa kopplingsbara posttyper</p></li>
<li><p>Planning Plus-paket för att skapa centraliserade posttyper</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av din kontoansvarige på Workfront. </p> 
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

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Konfigurera centraliserade posttyper

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

Som arbetsytehanterare kan du konfigurera en posttyp så att den blir en centraliserad posttyp. En centraliserad posttyp kan läggas till i andra arbetsytor.

En arbetsytehanterare kan lägga till en centraliserad posttyp på en arbetsyta som de hanterar. Posttypens originalfält läggs också till.

Användarna kan lägga till poster i en centraliserad posttyp från vilken arbetsyta som helst som har Contribute-behörigheter och där den centraliserade posttypen läggs till, inklusive den ursprungliga arbetsytan. De kan visa poster från en arbetsyta som de bara har behörigheten Visa till.

Mer information finns i [Posttyper för arbetsytan - översikt](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

Så här konfigurerar du en posttyp som central:

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill konfigurera som centraliserade.

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll pekaren över kortet för en posttyp och klicka på menyn **Mer** ![Mer](assets/more-menu.png) i det övre högra hörnet av posttypskortet
   * Klicka på ett posttypskort för att öppna posttypssidan och klicka sedan på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om posttypens namn.
1. Klicka på **Redigera**.

   ![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card.png)

   >[!TIP]
   >
   >Om en posttyp redan har angetts som en centraliserad posttyp och har lagts till på andra arbetsytor är alternativet Redigera nedtonat.

1. Klicka på fliken **Avancerade inställningar** i rutan **Redigera posttyp**.
1. Aktivera inställningen **Tillåt att den här posttypen läggs till i andra arbetsytor**.

   ![Redigera posttyp Avancerade inställningar med Lägg till i andra arbetsytor aktiverar](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >När du har lagt till en centraliserad posttyp på en annan arbetsyta kan den här inställningen inte längre inaktiveras.

1. I fältet **Välj vem som kan lägga till den här posttypen i arbetsytor som de hanterar** lägger du till entiteter som du vill tillåta att den här posttypen läggs till i arbetsytor som de hanterar.

   Ditt namn läggs automatiskt till i fältet.

   Du kan lägga till enskilda användare, eller grupper, team, jobbroller eller företag vars användare du vill tillåta att den här posttypen läggs till på de arbetsytor som de hanterar.

   Du måste utse minst en enhet (användare, team, grupp, roll eller företag) för att kunna aktivera den här inställningen.

   Du kan redigera det här fältet när du har sparat posttypen.

1. (Valfritt) Ta bort ditt namn från fältet **Välj vem som kan lägga till den här posttypen i arbetsytor som de hanterar**.

1. Klicka på **Spara**.

   Följande saker händer:

   * Posttypen och dess fält är nu tillgängliga och kan läggas till på en annan arbetsyta av de personer du har angett.

   >[!NOTE]
   >
   >Du kan bara redigera posttypens utseende och inställningar och dess ursprungliga fält från den ursprungliga arbetsytan.

   * Posttypkortet visar en centraliserad ikon ![Centraliserad posttypsikon](assets/global-icon.png) som anger att posttypen är tillgänglig för tillägg till andra arbetsytor.
   * Ett systemgenererat **Workspace**-fält läggs till i registervyn för posttypen och dess posterdetaljer.

     I fältet Workspace visas arbetsytan där varje post skapas.

     Det här fältet är skrivskyddat och kan inte tas bort.
1. (Valfritt) Gå till en annan arbetsyta och skapa en posttyp med en befintlig posttyp. Välj den posttyp som du aktiverade i stegen ovan.

   Mer information finns i [Lägga till befintliga posttyper från en annan arbetsyta](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Konfigurera posttyper som kan anslutas

<!--this is a UI term; don't change the title of this section-->

Du kan konfigurera en posttyp som ska anslutas till från andra arbetsytor när du skapar eller redigerar posttypen.

Så här konfigurerar du en posttyp att ansluta till från andra arbetsytor när du redigerar posttypen:

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill redigera.

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll muspekaren över kortet för en posttyp och klicka på menyn **Mer** ![Mer](assets/more-menu.png) i det övre högra hörnet av posttypskortet och klicka sedan på **Redigera**
   * Klicka på ett posttypskort för att öppna posttypssidan, klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Redigera**.

   ![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card.png)

1. Klicka på fliken **Avancerade inställningar** i rutan **Redigera posttyp**.
1. Aktivera inställningen **Tillåt anslutning till den här posttypen i andra arbetsytor**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Redigera posttyp Avancerade inställningsflikar med anslutning från andra arbetsytor aktiverat](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   När det här alternativet är aktiverat är posttypen tillgänglig och kan anslutas till från andra arbetsytor.

1. Välj från vilka arbetsytor som posttypen kan nås. Välj bland följande alternativ:

   * **Systemomfattande**: Användare kan ansluta till den här posttypen från alla arbetsytor där de har behörigheten Hantera.
   * **Specifika arbetsytor**: Lägg till namnen på arbetsytorna där arbetsytehanterare kan ansluta till den här posttypen.
1. Klicka på **Spara**.

   Följande saker händer:

   * Posttypen och dess fält är nu tillgängliga för anslutning från de arbetsytor du har angett.
   * Posttypskortet visar en ikon för anslutning mellan arbetsytor ![Anslutningsikon mellan arbetsytor](assets/connect-from-other-workspaces-icon.png) som anger att posttypen är tillgänglig för anslutning från en arbetsyta som du har angett i konfigurationen.

   Posttypen blir tillgänglig att ansluta till från de angivna arbetsytorna.
1. (Valfritt) Gå till en annan arbetsyta och lägg till en anslutning till den posttyp som du har aktiverat för anslutningsbarhet mellan arbetsytor i stegen ovan.

   Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).









