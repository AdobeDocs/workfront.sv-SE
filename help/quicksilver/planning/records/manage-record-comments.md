---
title: Hantera postkommentarer
description: Du kan samarbeta om Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 60f2890e431065d0eb034a9254680e43a51ecab8
workflow-type: tm+mt
source-wordcount: '1045'
ht-degree: 0%

---

# Hantera postkommentarer

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan samarbeta om Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.

I den högra panelen för en post visas följande avsnitt:

* **Kommentarer**: Visar kommentarer och svar som användare lägger till i poster.
* **Historik**: Visar ändringar som användarna gör i postfälten. Mer information finns i [Översikt över avsnittet Historik](/help/quicksilver/planning/records/history-section-overview.md).

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
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Contributor eller högre licens</p>
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
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning-områdena.</p>
   <div class="preview">
<p> I förhandsgranskningsmiljön måste användare med en ljus- eller Contributor-licens tilldelas en layoutmall som innehåller Planning.</p>

<p>Standardanvändare och systemadministratörer har Planering aktiverat som standard.</p></div>

<p>Mer information finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Skapa och hantera layoutmallar</a>.</p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Att tänka på när du kommenterar en post

* Du kan lägga till kommentarer och svar till poster i Workfront Planning, under Kommentarer i en post.

* Kommentarer som läggs till i länkade poster visas inte i de poster som du länkar från. Om du till exempel kommenterar en produktpost för Workfront Planning som är länkad till en Campaign-post, visas kommentaren bara på produktposten i Workfront Planning och inte på Campaign-posten som du länkar från.

* Du kan lägga till kommentarer i Workfront Planning-poster som har skapats som ett resultat av en anslutning mellan en post och ett objekt från ett annat program.

  Du kan till exempel kommentera projektposten för Workfront Planning när du har kopplat Workfront-projekt till Workfront Planning-poster. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

* Kommentarer som läggs till i länkade objekt i andra program visas inte i Workfront Planning och kommentarer som läggs till i länkade objekt i Workfront Planning visas inte i andra program.

  Kommentarer som läggs till i projekt i Workfront visas t.ex. inte i samma projekt som är länkat till en kampanj i Workfront Planning, och kommentarer som läggs till i projektet Workfront Planning-posten visas inte i Workfront.

* Du kan tagga användare eller team så att de uppmärksammas på en uppdatering. Både individuellt taggade användare och användare från taggade team får ett meddelande i appen och ett e-postmeddelande om uppdateringen.

  >[!NOTE]
  >
  >   Endast användare som har anslutit sig till Adobe Unified Experience får både ett meddelande i appen och ett e-postmeddelande. Information om hur du avgör om ditt företag använder Adobe Unified Experience finns i [Adobe Unified Experience för Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Du kan lägga till en uppdatering i poster och granska ändringshistoriken från följande områden i Workfront Planning:

   * Från sidan med postinformation.
   * Från en vy, i rutan med postinformation.

### Hantera kommentarer på poster

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas på kort.

1. Klicka på ett posttypskort.
Posttypssidan öppnas och alla poster av den typen visas.

1. Välj en tabellvy i listrutan **Visa**.
1. Klicka på namnet på en post i tabellvyn.

   Postens **informationssida** öppnas. Kommentarsområdet öppnas som standard i den högra panelen.

1. (Villkorligt) Om den högra panelen inte öppnas som standard klickar du på ikonen **Visa kommentarer** ![Visa kommentarer](assets/show-comments-icon.png) i det övre högra hörnet för att öppna kommentarsavsnittet.

1. Börja skriva en kommentar i rutan **Ny kommentar**.

   ![Tom kommentarsruta på post](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Om du navigerar bort från kommentarsavsnittet innan du är klar med att skriva och skicka en kommentar, kommer kommentaren på sidan att vara i utkastläge även efter att du loggat ut och loggat in igen. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (Valfritt) Om du vill ångra eller göra om en ändring använder du följande kortkommandon:
   * CTRL + Z (⌘ + z för Mac) för att ångra en ändring
   * CTRL + Y (⌘+y för Mac) för att göra om en ändring
1. (Valfritt och villkorligt) Om din Workfront-instans ingår i Adobe Unified Experience lägger du till **@** följt av namnet på en användare eller ett team som taggar dem i uppdateringen. Mer information finns i avsnittet [Att tänka på när du kommenterar en post](#considerations-about-commenting-on-a-record) i den här artikeln.

1. (Valfritt) Använd alternativen i verktygsfältet RTF för att formatera texten, lägga till känslolägesikoner eller länkar till uppdateringen för att förbättra innehållet.

   >[!TIP]
   >
   >Du kan inte lägga till bilder i en postkommentar.


1. Fortsätt lägga till kommentarer i posten.

   Mer information om hur du uppdaterar objekt, inklusive Workfront Planning-poster, finns i [Uppdatera arbete](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Valfritt) Klicka på ikonen **Mer** ![Mer meny](assets/more-menu.png) i det övre högra hörnet av kommentaren och klicka sedan på **Ta bort** för att ta bort kommentaren.
1. (Valfritt) Klicka på ikonen **Dölj kommentarer** ![Dölj kommentarer](assets/hide-comments-icon.png) för att stänga den högra panelen.

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ..** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## Översikt över avsnittet Historik

Du kan granska ändringarna som gjorts i posten i historikavsnittet på den högra panelen i en post.

Mer information finns i [Översikt över avsnittet Historik](/help/quicksilver/planning/records/history-section-overview.md).
