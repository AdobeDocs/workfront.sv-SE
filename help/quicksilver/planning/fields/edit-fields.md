---
title: Redigera fältinställningar
description: I Adobe Workfront Planning kan du redigera fältinställningarna för fält som redan har skapats. I den här artikeln beskrivs hur du kan redigera inställningarna för Workfront Planning-fält.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Redigera fältinställningar

{{planning-important-intro}}

Du kan redigera fältinställningarna för fält som redan har skapats i Adobe Workfront Planning.

Mer information om hur du skapar Adobe Workfront Planning-fält finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

I den här artikeln beskrivs hur du kan redigera inställningarna för Workfront Planning-fält. Mer information om hur du redigerar fältvärden för poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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
   <p>Aktuell: Planera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

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

