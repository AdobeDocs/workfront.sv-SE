---
title: Dela poster
description: Du kan dela poster med knappen Dela för att öka samarbetet i Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 54a6e633e903c73a78b36e90fb27edb445dc8d47
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---


<!--update metadata with real information at release-->

# Dela poster

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


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
* När du delar en post har användarna samma åtkomst överallt där posten visas i systemet.
* Om du begränsar behörigheter till en post kan användarna inte längre visa den posten och värdena för dess sökfält någonstans i systemet där posten läggs till.
* Workfront kontrollerar inspelningsbehörigheter i anslutningar som är upp till fem poster djupa, så att användarna bara ser poster som delas med dem.
* Du kan tilldela följande behörighetsnivåer till en post:

   * Visa
   * Hantera
* När du delar en arbetsyta och en posttyp med användare får de som standard samma behörigheter som posterna på arbetsytan.
När användare har Contribute-behörighet för en arbetsyta eller posttyp får de behörigheten Hantera för posterna av den posttypen.
* När du tar bort en enhet från en arbetsyta tas alla delningsbehörigheter bort från posttyperna och alla poster i den.
* En användares åtkomst till posten bestäms genom en kombination av följande tre inställningar:

   * Deras behörigheter ärvs från posttypen och arbetsytan
   * Behörigheter läggs till individuellt i dialogrutan för postdelning
   * Följande behörigheter:

      * **Alla på arbetsytan kan visa**: Detta gör att posten kan visas av alla på arbetsytan <!-- is this OK to say "workspace? should it be "record"??-->
      * **Endast inbjudna personer kan komma åt**: Detta är markerat som standard och tillåter att åtkomsten till posten begränsas till vissa personer.

     >[!NOTE]
     >
     >Om du väljer att bevilja **alla på arbetsytan behörighet** till en posttyp eller en post, får alla som visas i delningslistan på arbetsytan samma behörigheter för posttypen och posten, även när ärvda behörigheter är inaktiverade.


* När du delar en post med en användare läggs de till som standard med samma behörighet som de har för posttypen.

  Exempel:

   * Om de har behörigheten Visa för posttypen får de behörigheten Visa för posten
   * Om de har Contribute- eller Hantera-behörighet för posttypen får de behörigheten Hantera för posten

* Som arbetsytehanterare kan du dela en post med en användare som inte har behörighet till posttypen eller arbetsytan. I det här fallet visas en varning bredvid den tillagda entiteten om att de inte har tillgång till arbetsytan eller posttypen. <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> Du kan fortsätta lägga till användaren i posten. Användaren läggs också till i posttypen och på arbetsytan, eller avbryta delningen.

* När en användare har behörigheterna Hantera eller Contribute på arbetsytan och posttypen och du lägger till dem i postbehörigheterna, är visningsbehörigheterna nedtonade. De behåller samma behörigheter till posten som de har till posttypen, och du kan inte ge dem lägre behörigheter till posten. <!--Lilit is checking on this, it is not working correctly-->

  När de har behörigheten Visa på arbetsytan eller posttypen behåller de behörigheterna Visa för posterna. Du kan ge dem behörigheten Hantera för posten genom att inaktivera ärvda behörigheter och välja inställningen Endast inbjudna personer har åtkomst. <!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* Du kan inaktivera ärvda behörigheter för en enskild post. I så fall kan du ge dem behörighet till enskilda poster, eller så kan de få behörighet om de tillhör alternativet **Alla på arbetsytan kan visa**.

* Om flera delningsbehörigheter gäller för samma användare får de den högsta behörigheten av dessa behörigheter.

  Om en post till exempel delas med en användare med behörigheten Visa, och deras grupp med behörigheten Hantera, får de behörigheten Hantera för posten.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Om ett formelfält eller ett uppslagsfält från en kopplad post baseras på ett fält på en post som du inte har behörighet till, ser du rätt beräkning av vilka faktorer i posten som du inte kan komma åt på annat sätt.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Dela postbehörigheter

Som arbetsytehanterare kan du justera behörigheter till enskilda poster.

{{step1-to-planning}}

1. Öppna arbetsytan vars poster du vill dela.
1. Klicka på den posttyp vars poster du vill dela.

1. Gör något av följande:

   * Håll markören över namnet på en post i tabellvyn, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Dela**.
   * Markera en post i tabellvyn och klicka sedan på **Dela** i det blå verktygsfältet längst ned i listan.
   * Klicka på namnet på en post i valfri vy och klicka sedan på **Dela** i det övre högra hörnet på postens informationssida.

   Rutan **Dela** öppnas.

   ![Behörigheter för poster med ärvda behörigheter &#x200B;](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Valfritt) I området **Vem har åtkomst** är alternativet **Alla på arbetsytan kan visa** markerat som standard.  Alla användare som har **Visa** eller högre behörighet till arbetsytan och posttypen har samma behörigheter som posten.

1. (Valfritt) Klicka på antalet användare under alternativet **Ärvda behörigheter** för att visa användare, team, grupper, företag eller jobbroller som ärver behörigheter från arbetsytan.

   >[!TIP]
   >
   >Du kan inte ta bort enskilda entiteter från listan Ärvda behörigheter. <!--test this!-->

1. (Valfritt och villkorligt) Om du vill dela posten med specifika entiteter och ge dem en annan åtkomst till posttypen än de redan har för arbetsytan gör du följande:

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
   >* Om användarna har behörighet att hantera Contribute eller Hantera på arbetsytan och posttypen, behåller de behörigheterna Hantera för posten. Visningsbehörigheten är nedtonad. <!--this is not dimmed at this time, Lilit to check-->
   >* Du kan inte ge användarna mindre behörighet till posten om de har Contribute eller högre för posttypen.
   > Mer information finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
   >* När du delar en post med en användare visas även deras primära jobbroll <span class="preview"> och deras e-postadress</span> i fältet. Du måste ha inställningen Visa kontaktinformation aktiverad för objektet Användare på din åtkomstnivå för att kunna se användarens e-post.

1. Om du vill ge användare som inte har behörighet till arbetsytan åtkomst att visa en post går du till fältet **Bevilja åtkomst till den här vyn** och börjar skriva namnet på en användare, en grupp, ett team, ett företag eller en jobbroll. Klicka sedan på den när den visas i listan.

   Den entitet du har valt läggs till i posten och även i posttypen och på arbetsytan med **Visa**-behörigheter.

   Systemadministratörer får alltid behörigheten Hantera för poster som delas med dem, och det finns en indikation på att en användare är systemadministratör.

1. (Valfritt) Klicka på **Kopiera länk** om du vill kopiera en länk till posten till Urklipp och dela den med andra. Länken öppnar postens informationssida.
1. Klicka på **Spara**.

   Posten delas nu med andra användare.

   Användarna som du delade posten med får både ett meddelande i appen och ett e-postmeddelande om att de har fått behörigheter till följande enheter:

   * Posten
   * Posttypen, om de aldrig hade behörigheter tidigare
   * Arbetsytan, om de inte hade behörighet till arbetsytan innan posten delades med dem.

   Mer information finns i [Adobe Workfront Planning-meddelanden: artikelindex](/help/quicksilver/planning/notifications/notifications-information.md).

1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt posttypssidan och visa den i den valda vyn. De måste ha behörighet till posttypen för att kunna visa den. Mer information finns också i [Dela poster via en länk](/help/quicksilver/planning/records/share-records.md).

## Ta bort behörigheter till en post

Du kan ta bort användarnas behörigheter från en post. De behåller dock åtminstone behörigheterna Visa på arbetsytan, vilket ger dem åtminstone behörigheten Visa för posttypen. Du måste ta bort deras åtkomst från arbetsytan om du vill att de inte ska ha behörighet till posttyperna eller posterna på arbetsytan.

{{step1-to-planning}}

1. Öppna arbetsytan vars poster du vill sluta dela och klicka sedan på ett posttypskort. Då öppnas posttypssidan.
1. Gör något av följande:

   * Håll markören över namnet på en post i tabellvyn, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Dela**.
   * Markera en post i tabellvyn och klicka sedan på **Dela** i det blå verktygsfältet längst ned i listan.
   * Klicka på namnet på en post i valfri vy och klicka sedan på **Dela** i det övre högra hörnet på postens informationssida.

   Rutan **Dela** öppnas.
1. Hitta den användare, grupp, team, företag eller jobbroll vars behörigheter du vill ta bort, utöka den nedrullningsbara menyn Behörigheter till höger om namnet och klicka sedan på **Ta bort**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Ta bort behörigheter på posten](assets/remove-option-on-record-sharing-drop-down.png)

1. Klicka på **Spara**.

   Personer har inte längre de angivna behörigheterna för posten. De har dock fortfarande behörighet till posttypen och arbetsytan, såvida du inte också tar bort dem från dessa behörigheter.

   Användarna som har tagits bort från åtkomsten till posten får inget meddelande om att de inte längre har dessa behörigheter.
