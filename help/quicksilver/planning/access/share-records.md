---
title: Dela poster
description: Du kan dela poster med knappen Dela för att öka samarbetet i Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---


<!--update metadata with real information at release-->

# Dela poster

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Du kan justera personers behörigheter till enskilda poster i en posttyp. O

Du kan dela en Adobe Workfront Planning-post på följande sätt:

* Dela en länk till posten.

  Mer information finns i [Dela poster via en länk](/help/quicksilver/planning/records/share-records.md).

* Dela alla poster på en arbetsyta med andra användare genom att dela arbetsytan och posttypen.

  Mer information finns i följande artiklar:

   * [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md)

   * [Dela en posttyp](/help/quicksilver/planning/access/share-record-types.md)

* Dela en post med alternativet **Dela**.

  I den här artikeln beskrivs hur du kan dela en post med andra genom att använda alternativet **Dela**.

>[!IMPORTANT]
>
>Användare som har åtkomst till en arbetsyta får automatiskt minst behörigheten Visa för alla poster på arbetsytan.
>Delade vyer ger inte användarna behörighet till posterna. Endast arbetsytor för delning kan ge användare behörighet att spela in typer och poster.
>
>Allmän information om delning av objekt i Workfront Planning finns även i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla Workfront- och Planning-paket</p> 
eller
<p>Alla arbetsflödes- och planeringspaket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Alla</p> 
   <p><b>ANMÄRKNING</b></p>
   <p>Endast personer med en standardlicens kan beviljas behörigheten Hantera för poster. Alla andra licenser kan bara ha behörigheten Visa och alternativet Hantera är nedtonat för dem.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  <p>Hantera behörigheter till en arbetsyta, en posttyp och posten</p>  
   <p><b>VIKTIGT</b></p>
   <p>Endast användare med behörigheten Hantera på en arbetsyta kan dela en post</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planning.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på vid delning av poster

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

* Du kan dela poster med följande enheter: personer, grupper, team, företag eller jobbroller.
* När du delar en arbetsyta med användare får de som standard samma behörigheter som posterna på arbetsytan.
* När du tar bort en enhet från en arbetsyta tas alla delningsbehörigheter bort från posttyperna och alla poster i den.
* En användares åtkomst till posten bestäms genom en kombination av följande tre inställningar:

   * Deras behörigheter ärvs från posttypen och arbetsytan
   * Behörigheter läggs till individuellt i dialogrutan för postdelning
   * Följande behörigheter:

      * **Alla på arbetsytan kan visa**: Detta gör att posten kan visas av alla på arbetsytan <!-- is this OK to say "workspace? should it be "record"??-->
      * **Endast inbjudna personer kan komma åt**: Detta är markerat som standard och tillåter att åtkomsten till posten begränsas till vissa personer.

* Du kan tilldela följande behörighetsnivåer till en post:

   * Visa
   * Hantera

* När du delar en post med en användare läggs de till som standard med samma behörighet som de har för posttypen.

  Exempel:

   * Om de har behörigheten Visa för posttypen får de behörigheten Visa för posten
   * Om de har Contribute- eller Hantera-behörighet för posttypen får de behörigheten Hantera för posten

* Som arbetsytehanterare kan du dela en post med en användare som inte är en del av arbetsytan. I det här fallet visas en varning bredvid den tillagda entiteten om att de inte har åtkomst till arbetsytan. Du kan acceptera att användaren läggs till både i posten och på arbetsytan, eller neka att användaren läggs till på arbetsytan, vilket även tar bort användaren från posten.

* När du delar en post med användare som har behörigheten Hantera på arbetsytan, får de även behörigheten Hantera till posten som standard. Visningsbehörigheten är nedtonad.

* Om du inte har behörighet att lägga till personer på arbetsytan kan du bara visa och lägga till användare, team, grupper, roller och företag som redan har lagts till på arbetsytan. Du kan inte lägga till andra entiteter som inte redan ingår i arbetsytan.

* Du kan inaktivera ärvda behörigheter för en enskild post. I så fall kan du ge dem behörigheter individuellt, eller så kan de få behörigheter om de tillhör alternativet Alla på arbetsytan. <!-- is this OK to say "workspace? should it be "record"??-->

* Om flera delningsbehörigheter gäller för samma användare får de den högsta behörigheten av dessa behörigheter.

  Om en post till exempel delas med en användare med behörigheten Visa, och deras grupp med behörigheten Hantera, får de behörigheten Hantera för posten.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Om ett formelfält eller ett uppslagsfält från en kopplad post baseras på ett fält på en post som du inte har behörighet till, ser du rätt beräkning av vilka faktorer i posten som du inte kan komma åt på annat sätt.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Dela postbehörigheter

