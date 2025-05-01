---
title: Översikt över avsnittet Historik
description: Du kan granska ändringar som gjorts i posten och som spelats in av systemet på den högra panelen av en post i Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Översikt över avsnittet Historik

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön för alla kunder, eller i produktionsmiljön för kunder som aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Du kan samarbeta om Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.

I den högra panelen för en post visas följande avsnitt:

* **Kommentarer**: Visar kommentarer och svar som användare lägger till i poster. Mer information om hur du hanterar kommentarer i Workfront Planning-poster finns i [Hantera postkommentarer](/help/quicksilver/planning/records/manage-record-comments.md).
* **Historik**: Visar ändringar som användarna gör i postfälten.

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
   <td> <p>Contributor eller högre licens</p>
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
   <td>   <p>Visa eller högre behörigheter på en arbetsyta <span class="preview">och posttyp</span> </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> 
   <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning-områdena.</p>
   <div class="preview">
<p> I förhandsgranskningsmiljön måste användare med en ljus- eller Contributor-licens tilldelas en layoutmall som innehåller Planning.</p>

<p>Standardanvändare och systemadministratörer har Planering aktiverat som standard.</p></div>

<p>Mer information finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Skapa och hantera layoutmallar</a>.</p>
    </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Leta reda på historikavsnittet för en post

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas på kort.

1. Klicka på ett posttypskort.
Posttypssidan öppnas och alla poster av den typen visas.

1. Klicka i valfri vy på namnet på en post.

   Postens sida öppnas. Kommentarsområdet öppnas som standard i den högra panelen.
1. Klicka på ikonen **Visa historik** ![Visa historik](assets/show-history-icon.png). Alla ändringar som görs i postens fält visas på den högra panelen, med början från den senaste.
1. (Valfritt) Klicka på ikonen **Dölj historik** ![Dölj historik](assets/hide-history-icon.png) för att stänga den högra panelen.

## Överväganden om historikavsnittet

Du kan granska ändringarna som gjorts för postfält i historikavsnittet på den högra panelen på en postsida.

![Historikområde i kommentarer](assets/history-area-in-comments.png)

* Workfront Planning registrerar följande information i historikavsnittet:

   * Alla fältändringar

   * Det gamla och de nya värdena i fälten när värdena ändras. De gamla värdena visas i genomstrykningsformat.

   * Det fullständiga namnet på användaren som gjorde ändringen

   * En datum- och tidsstämpel som anger när ändringen inträffade.

* Fält av följande typer visar alltid det gamla värdet (i genomstrykningsformat) och det nya värdet:

   * Text
   * Stycke
   * Valuta
   * Datum
   * Nummer
   * Procent
   * Enkelval

* Fält av följande typer visar det gamla värdet i genomstrykningsformat endast om minst ett av de flera värdena har tagits bort:

   * Flera val
   * Länkade postfält
   * Folk

  Om ändringen bara har lagt till värden i fältet visas inte det gamla värdet och bara det nya fältvärdet visas.

* Fält av typen Kryssruta visar aldrig det gamla värdet i genomstrykningsformat. Om fältet redigeras visas bara det aktuella läget när ändringen gjordes.

  Mer information om Workfront Planning-fält finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

* Ändringar i fält av följande typer visas inte i avsnittet Historik:

   * Länkade (sökning) fält
   * Formel
   * Skapad av
   * Skapad den
   * Senast ändrad av
   * Senast ändrat den

* Om ett fält tas bort från systemet finns uppdateringarna som gjorts i det fältet kvar i historikavsnittet. Det finns inget som tyder på att fältet har tagits bort i historikdelen av en post.
