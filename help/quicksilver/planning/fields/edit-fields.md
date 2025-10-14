---
title: Redigera fältinställningar
description: I Adobe Workfront Planning kan du redigera fältinställningarna för fält som redan har skapats. I den här artikeln beskrivs hur du kan redigera inställningarna för Workfront Planning-fält.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---


# Redigera fältinställningar

<!--leave the choice value information in yellow till January 2026-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan redigera inställningarna för befintliga fält i Adobe Workfront Planning.

Mer information om hur du skapar Adobe Workfront Planning-fält finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

I den här artikeln beskrivs hur du kan redigera inställningarna för Workfront Planning-fält. Mer information om hur du redigerar fältvärden för poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

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
   <td>   <p>Hantera behörigheter till en arbetsyta och posttyp </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p></td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Att tänka på när du redigerar fältinställningar

Du måste tänka på följande innan du gör ändringar i ett fälts konfiguration:

* Du kan bara redigera fältinställningar från posttyptabellen.
* Du kan inte redigera inställningarna för ett fält på postsidan eller i någon annan vy, utanför tabellvyn.
* Du kan inte redigera fälttypen efter att fältet har sparats.
* Du kan inte avmarkera inställningen Tillåt negativa tal som tidigare var markerad, för fältet Nummer, Procent eller Valuta om det redan finns negativa värden lagrade på posterna som den är kopplad till.
* Du kan redigera konfigurationen för följande fältelement när du har sparat fältet:

   * Namn eller beskrivning av fält
   * Alternativen för ett enskilt eller flervalsfält.
   * Uttrycket för ett formelfält.

  >[!WARNING]
  >
  >När formeluttryck ändras, eller alternativ läggs till eller tas bort från ett urvalsfält, försvinner data för de poster som redan har information lagrad i de fält vars konfiguration ändras.
  >
  >Det finns ingen varning eller indikation om att denna dataförlust kan inträffa när du ändrar fältkonfigurationen.
  >
  >Det finns inget meddelande till andra användare om att fältkonfigurationen har ändrats.

* Du kan redigera befintliga uppslagsfält från anslutna poster.
* Förutom att redigera fältet enligt beskrivningen i avsnittet [Redigera fältinställningar](#edit-field-settings-1) i den här artikeln, kan <span class="preview">du redigera ett envalsfält eller flervalsfält när du redigerar en post i tabellvyn när du uppdaterar fältvärdena. Mer information finns i avsnittet [Lägg till nya alternativ i ett befintligt urvalsfält när du redigerar poster i tabellvyn](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view) i den här artikeln.</span>

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Redigera fältinställningar

{{step1-to-planning}}

1. Klicka på arbetsytan vars postfält du vill redigera.

   Arbetsytan öppnas och alla posttyper i arbetsytan visas på kort.

1. Klicka på kortet för en posttyp.

   Då öppnas posttypens sida.

1. (Villkorligt) Klicka på fliken i en **tabellvy**.

   Alla befintliga poster som är associerade med posttypen visas i tabellvyns rader.
1. Håll markören över kolumnrubriken för ett fält som du vill redigera, klicka sedan på nedåtpilen efter fältnamnet och klicka sedan på **Redigera fält**

   eller

   Dubbelklicka på fältets kolumnrubrik.

   ![Pilmeny efter fältets namn i tabellhuvudet markerat](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Uppdatera information om fältet och klicka på **Spara**.

   Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Du kan inte uppdatera fälttypen efter att fältet har sparats.
   >
   >* När du ändrar fältkonfigurationer (fältalternativ eller formeluttryck) kommer poster som redan innehåller information i de ändrade fälten att uppdatera sina värden i realtid. Det finns ingen varning och ingen granskningslogg för de värdeändringar som utlöses av fältkonfigurationsändringar. Alla användare som visar fälten ser omedelbart de nya värdena med ändringarna.

   Fältinformationen uppdateras för alla som har åtkomst till arbetsytan.

1. (Villkorligt) För anslutna postfält klickar du på **Redigera uppslagsfält** och lägger till eller tar bort något av uppslagsfälten från den anslutna posttypen.

   Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).


<div class="preview">

## Lägga till nya alternativ i ett befintligt markeringsfält när du redigerar poster i tabellvyn

<!--some of this information is also available in Edit records article - update both when necessary-->

Du kan lägga till nya alternativ i ett befintligt envalsfält eller flervalsfält när du redigerar poster i tabellvyn.

>[!IMPORTANT]
>
>De funktioner som beskrivs i det här avsnittet är bara tillgängliga i tabellvyn. Den är inte tillgänglig i andra områden där ett eller flera fält visas.

**EXEMPEL**

Du kan ha ett envalsfält med namnet Status som har alternativen Nytt och Stängt, och du vill lägga till ett alternativ för statusen Pågående. Du kan lägga till valet genom att göra något av följande:

* Redigerar fältet. Mer information finns i avsnittet [Redigera fältinställningar](#edit-field-settings-1) i den här artikeln.
* Lägga till ett nytt alternativ när du redigerar posten i tabellvyn, enligt beskrivningen nedan.

Så här lägger du till ett nytt val i ett befintligt markeringsfält när du redigerar en post:

1. Gå till en posttypssida och öppna tabellvyn.
1. Lägg till det envalsfält eller flervalsfält som du vill lägga till som en ny kolumn i tabellvyn. Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).
1. Börja redigera fältet textbundet genom att dubbelklicka på cellen för fältet.
1. Skriv namnet på det alternativ som du vill lägga till och klicka sedan på **Lägg till alternativ**.

   ![Lägg till val i envalsfält i tabellvy](assets/add-choice-in-table-view-for-single-select-field.png)

   Det nya alternativet läggs omedelbart till i fältet för en markering.

   <!--<span class="preview">A new choice value is also added to each choice. You can use the choice values in API calls or other integrations. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). </span>-->

</div>