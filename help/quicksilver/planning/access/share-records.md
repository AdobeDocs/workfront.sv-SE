---
title: Dela poster
description: Du kan dela poster med knappen Dela för att öka samarbetet i Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 0%

---


<!--update metadata with real information at release-->

# Dela poster

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Du kan justera personers behörigheter till enskilda poster i en posttyp.

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

<!--checking on the below with Lilit-->

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

* Som arbetsytehanterare kan du dela en post med en användare som inte är en del av arbetsytan. I det här fallet visas en varning bredvid den tillagda entiteten om att de inte har åtkomst till arbetsytan. Du kan fortsätta lägga till användaren i posten, som också kommer att lägga till honom/henne på arbetsytan, eller sluta lägga till användaren i posten, som inte kommer att lägga till honom/henne på arbetsytan.

* När du delar en post med användare som har behörigheten Hantera på arbetsytan, får de även behörigheten Hantera till posten som standard. Visningsbehörigheten är nedtonad.

* Om du inte har behörighet att lägga till personer på arbetsytan kan du bara visa och lägga till användare, team, grupper, roller och företag som redan har lagts till på arbetsytan. Du kan inte lägga till andra entiteter som inte redan ingår i arbetsytan.

* Du kan inaktivera ärvda behörigheter för en enskild post. I så fall kan du ge dem behörighet till enskilda poster, eller så kan de få behörighet om de tillhör alternativet **Alla på arbetsytan kan visa**. <!-- is this OK to say "workspace? should it be "record"??-->

* Om flera delningsbehörigheter gäller för samma användare får de den högsta behörigheten av dessa behörigheter.

  Om en post till exempel delas med en användare med behörigheten Visa, och deras grupp med behörigheten Hantera, får de behörigheten Hantera för posten.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Om ett formelfält eller ett uppslagsfält från en kopplad post baseras på ett fält på en post som du inte har behörighet till, ser du rätt beräkning av vilka faktorer i posten som du inte kan komma åt på annat sätt.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Dela postbehörigheter

Du kan justera behörigheter för enskilda poster om du har behörigheten Hantera på arbetsytan.

{{step1-to-planning}}

1. Öppna arbetsytan vars poster du vill dela.
1. Klicka på den posttyp vars poster du vill dela.

1. Gör något av följande:

   * Håll markören över namnet på en post i tabellvyn, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Dela**.
   * Klicka på namnet på en post i valfri vy och klicka sedan på **Dela** i det övre högra hörnet på postens informationssida.

   Rutan **Dela** öppnas.

   ![Behörigheter för poster med ärvda behörigheter ](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Valfritt) I området **Vem har åtkomst** är alternativet **Alla på arbetsytan kan visa** markerat som standard.  Alla användare som har behörigheten Visa eller högre till arbetsytan och posttypen kan visa posten.

1. (Valfritt) Klicka på antalet användare under alternativet **Ärvda behörigheter** för att visa användare, team, grupper, företag eller jobbroller som ärver behörigheter från arbetsytan.

   >[!TIP]
   >
   >Du kan inte ta bort enskilda entiteter från listan Ärvda behörigheter.

1. (Valfritt och villkorligt) Om du vill dela posttypen med specifika entiteter och ge dem en annan åtkomst till posttypen än de redan har för arbetsytan gör du följande:

   1. Välj **Inaktivera** i listrutan **Ärvda behörigheter**.

   >[!TIP]
   >
   >Workspace-hanterare har fortfarande behörigheten Hantera för posttypen och posten.

   1. (Valfritt) Välj **Endast inbjudna personer kan komma åt** från området **Vem har åtkomst**.

   1. I fältet **Bevilja åtkomst till den här posttypen** lägger du till de användare, team, grupper, företag eller jobbroller som du vill ge en annan behörighetsnivå än de har för arbetsytan eller posttypen.
   1. Välj någon av följande behörighetsnivåer:

      * Visa
      * Hantera

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* Förutom team, grupper, företag och jobbroller kan du bara dela med användare som har lagts till i Adobe Admin Console. Du kan inte lägga till användare med endast Workfront. Mer information finns i [Hantera användare i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >* Om användarna har behörighet att hantera Contribute eller Hantera på arbetsytan och posttypen, behåller de behörigheterna Hantera för posten. Visningsbehörigheten är nedtonad
   >* Du kan inte ge användarna mindre behörighet till posten om de har Contribute eller senare.
   > Mer information finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Om du vill ge användare som inte har behörighet till arbetsytan åtkomst att visa en post går du till fältet **Bevilja åtkomst till den här vyn** och börjar skriva namnet på en användare, en grupp, ett team, ett företag eller en jobbroll. Klicka sedan på den när den visas i listan.

   Enheten som du har valt läggs till i posten och på arbetsytan med **Visa**-behörigheter.

   Systemadministratörer får alltid behörigheten Hantera för poster som delas med dem, och det finns en indikation på att en användare är systemadministratör.

1. (Valfritt) Klicka på **Kopiera länk** om du vill kopiera en länk till posten till Urklipp och dela den med andra. Länken öppnar postens informationssida.
1. Klicka på **Spara**.

   Posten delas nu med andra användare.
   <!--Checking with Lilit on this: The users you shared the record with receive both an in-app and email notification about having given permissions to the following entities:

   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them. -->

1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt posttypssidan och visa den i den valda vyn. De måste ha behörighet till posttypen för att kunna visa den. Mer information finns också i [Dela poster via en länk](/help/quicksilver/planning/records/share-records.md).

## Ta bort behörigheter till en post (************** DETTA KOPIERADES FRÅN POSTTYPER, DET MÅSTE REDIGERAS FÖR POSTER, MEN VÄNTA PÅ LISTANS SLACK-SVAR **********)

Du kan ta bort användarnas behörigheter från en post. De behåller dock åtminstone behörigheten Visa på postarbetsytan, vilket ger dem åtminstone behörigheten Visa för posttypen. Du måste ta bort deras åtkomst från arbetsytan om du vill att de inte ska ha behörighet till posttyperna på arbetsytan.

{{step1-to-planning}}

1. Öppna arbetsytan vars posttyper du vill sluta dela och klicka sedan på ett posttypskort. Då öppnas posttypssidan.

1. Klicka på **Dela** i det övre högra hörnet av posttypen på fliken i valfri vy.
1. Klicka på **Dela posttypen**.

   Rutan **Dela** öppnas.
1. Hitta den användare, grupp, team, företag eller jobbroll vars behörigheter du vill ta bort, utöka den nedrullningsbara menyn Behörigheter till höger om namnet och klicka sedan på **Ta bort**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Ta bort alternativ i listrutan för posttypsdelning](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Klicka på **Spara**.

   Personer har inte längre de angivna behörigheterna för posttypen. De har dock fortfarande behörighet till arbetsytan, såvida du inte också tar bort dem från arbetsytebehörigheterna.

   Användarna som har tagits bort från vyn får inget meddelande om att de inte längre har åtkomst till den.
