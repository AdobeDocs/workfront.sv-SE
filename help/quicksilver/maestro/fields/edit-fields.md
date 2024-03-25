---
title: Redigera fält
description: I Adobe Workfront kan du redigera fältinställningarna för fält som redan har skapats.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# Redigera fält

{{maestro-important-intro}}

Du kan redigera fältinställningarna för fält som redan har skapats i Adobe Workfront-planeringen.

Mer information om hur du skapar planeringsfält i Adobe Workfront finns i [Skapa fält](../fields/create-fields.md).

I den här artikeln beskrivs hur du kan redigera inställningarna för Workfront planeringsfält. Mer information om hur du redigerar fältvärden för poster finns i [Redigera poster](/help/quicksilver/maestro/records/edit-records.md).

## Att tänka på när du redigerar fältinformation

* Du kan redigera fält som du har skapat eller fält som har skapats av andra användare, om du har behörigheten Hantera på arbetsytan som fälten tillhör.
* Du kan redigera ett fält i posttyptabellen.
* Du kan inte redigera ett fält på detaljsidan för en post eller i tidslinjevyn.
* Du kan inte redigera fälttypen efter att fältet har sparats.
* Du kan inte avmarkera inställningen Tillåt negativa tal som tidigare var markerad, för fältet Nummer, Procent eller Valuta om det redan finns negativa värden lagrade på posterna som den är kopplad till.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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
<p>Din organisation måste vara registrerad i betaprogrammet för Adobe Workfront-planering. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Workfront-planering</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Redigera fält

{{step1-to-maestro}}

    Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill ta bort posttyper för.

   Arbetsytan öppnas och de posttyper som är associerade med den visas.
1. Klicka på kortet för den posttyp vars fält du vill redigera.

   Då öppnas posttypens sida.
1. (Villkorligt) Välj en **Tabellvy** från **Visa** nedrullningsbar meny i det övre högra hörnet på posttypssidan.
1. Håll markören över kolumnrubriken för ett fält som du vill redigera, klicka sedan på nedåtpilen efter fältnamnet och klicka sedan på **Redigera fält**

   eller

   Dubbelklicka på fältets kolumnrubrik.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Uppdatera information om fältet och klicka på **Spara**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Du kan inte uppdatera fälttypen efter att fältet har sparats.


1. (Villkorligt) Klicka på för länkade postfält **Redigera sökfält** och lägga till eller ta bort fält från den länkade posttypen.

   Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
