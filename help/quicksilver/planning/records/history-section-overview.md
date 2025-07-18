---
title: Översikt över avsnittet Historik
description: Du kan granska ändringar som gjorts i posten och som spelats in av systemet på den högra panelen av en post i Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Översikt över avsnittet Historik

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

Du kan samarbeta om Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.

Den högra panelen i en post visar följande avsnitt:

* **Kommentarer**: Visar kommentarer och svar som användare lägger till i poster. Mer information om hur du hanterar kommentarer i Workfront Planning-poster finns i [Hantera postkommentarer](/help/quicksilver/planning/records/manage-record-comments.md).
* **Historik**: Visar systemregistrerade ändringar som användare gör i postfälten.

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <li><p> Planering av Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Någon av följande Workfront-planer:</p> 
<ul><li>Utvald</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td> 
   <td> 
<p>Någon </p> 
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td> <p>Contributor eller högre licens</p>
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td>   <p>Visa eller högre behörigheter till en arbetsyta och posttyp </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Mall för layout</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planering.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>

</td>
  </tr>
</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Leta reda på avsnittet Historik för en post

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas på kort.

1. Klicka på ett kort för en posttyp.
Sidan för posttyp öppnas och alla poster av den typen visas.

1. Från vilken vy som helst klickar du på namnet på en post.

   Postens sida öppnas. Kommentarsområdet öppnas som standard i den högra panelen.
1. Klicka på ikonen **Visa historik** ![Visa historik](assets/show-history-icon.png). Alla ändringar som görs i postens fält visas på den högra panelen, med början från den senaste.
1. (Valfritt) Klicka på ikonen **Dölj historik** ![Dölj historik](assets/hide-history-icon.png) för att stänga den högra panelen.

## Överväganden om historikavsnittet

Du kan granska ändringarna som gjorts för postfält i historikavsnittet på den högra panelen på en postsida.

![Området Historik i Kommentarer](assets/history-area-in-comments.png)

* Workfront Planning registrerar följande information i avsnittet Historik:

   * Eventuella fältändringar

   * De gamla och de nya värdena för fält, när värdena ändras. De gamla värdena visas i genomstruket format.

   * Det fullständiga namnet på den användare som gjorde ändringen

   * En datum- och tidsstämpel som anger när ändringen inträffade.

* Fält av följande typer visar alltid det gamla värdet (i genomstrykningsformat) och det nya värdet:

   * Text
   * Paragraf
   * Valuta
   * Datum
   * Nummer
   * Procent
   * Välj en gång

* Fält av följande typer visar det gamla värdet i genomstrykningsformat endast om minst ett av de flera värdena har tagits bort:

   * Flera val
   * Länkade postfält
   * Folk

  Om ändringen bara lägger till värden i fältet visas inte det gamla värdet och endast det nya fältvärdet visas.

* Fält av kryssrutetyp visar aldrig det gamla värdet i genomstruket format. Om fältet redigeras visas bara det aktuella tillståndet vid den tidpunkt då ändringen gjordes.

  Mer information om Workfront Planning-fält finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

* Ändringar av fält av följande typer visas inte i avsnittet Historik:

   * Länkade fält (uppslagsfält)
   * Formel
   * Skapad av
   * Skapad den den
   * Senast ändrad av
   * Senast ändrat den

* Om ett fält tas bort från systemet finns uppdateringarna som gjorts i det fältet kvar i historikavsnittet. Det finns inget som tyder på att fältet har tagits bort i historikdelen av en post.
