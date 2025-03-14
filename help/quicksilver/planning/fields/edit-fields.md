---
title: Redigera fältinställningar
description: I Adobe Workfront Planning kan du redigera fältinställningarna för fält som redan har skapats. I den här artikeln beskrivs hur du kan redigera inställningarna för Workfront Planning-fält.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---


# Redigera fältinställningar

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->

{{planning-important-intro}}

Du kan redigera fältinställningarna för fält som redan har skapats i Adobe Workfront Planning.

Mer information om hur du skapar Adobe Workfront Planning-fält finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

I den här artikeln beskrivs hur du kan redigera inställningarna för Workfront Planning-fält. Mer information om hur du redigerar fältvärden för poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Åtkomstkrav

+++ Expandera för att visa åtkomstkrav..

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
   <td>   <p>Hantera behörigheter till en arbetsyta <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Att tänka på när du redigerar fältinställningar

Du måste tänka på följande innan du gör ändringar i ett fälts konfiguration:

* Du kan redigera fält som du har skapat eller fält som har skapats av andra användare, om du har behörigheten Hantera på arbetsytan som fälten tillhör.
* Du kan redigera ett fält i posttyptabellen.
* Du kan inte redigera ett fält på postsidan eller i någon annan vy utanför tabellvyn.
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

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Uppdatera information om fältet och klicka på **Spara**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Du kan inte uppdatera fälttypen efter att fältet har sparats.
   >
   >* När du ändrar fältkonfigurationer (fältalternativ eller formeluttryck) kommer poster som redan innehåller information i de ändrade fälten att uppdatera sina värden i realtid. Det finns ingen varning och ingen granskningslogg för de värdeändringar som utlöses av fältkonfigurationsändringar. Alla användare som visar fälten ser omedelbart de nya värdena med ändringarna.

   Fältinformationen uppdateras för alla som har åtkomst till arbetsytan.

1. (Villkorligt) För länkade postfält klickar du på **Redigera uppslagsfält** och lägger till eller tar bort något av fälten från den länkade posttypen.

   Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

