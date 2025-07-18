---
title: Hantera postkommentarer
description: Du kan samarbeta med Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar i den högra panelen i en post. Du kan också visa andra ändringar som har gjorts i posten och registrerats av systemet i det här området.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 0%

---

# Hantera postkommentarer

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan samarbeta med Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar i den högra panelen i en post. Du kan också visa andra ändringar som har gjorts i posten och registrerats av systemet i det här området.

Den högra panelen i en post visar följande avsnitt:

* **Kommentarer**: Visar kommentarer och svar som användare lägger till i poster.
* **Historik**: Visar systemregistrerade ändringar som användare gör i postfälten. Mer information finns i [Översikt](/help/quicksilver/planning/records/history-section-overview.md) över avsnittet Historik.

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
<li>Primtal</li> 
<li>Sist</li></ul> 
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p> 
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
<p>Din organisations instans av Workfront måste vara registrerad i Adobe Unified Experience för att kunna komma åt Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td><p> Licens för deltagare eller högre</p>
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
   <td>   <p>Visa eller högre behörigheter till en arbetsyta och posttyp</a> </p>  
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



## Att tänka på när du kommenterar en post

* Du kan lägga till kommentarer och svar på poster i Workfront Planning, i avsnittet Kommentarer för en post.

* Kommentarer som läggs till i länkade poster visas inte i de poster som du länkar från. Om du till exempel kommenterar en Workfront Planning-produktpost som är länkad till en Campaign-post, visas kommentaren bara på produktposten i Workfront Planning och inte på den Campaign-post som du länkar från.

* Du kan lägga till kommentarer i Workfront Planning-poster som skapats som ett resultat av en anslutning mellan en post och ett objekt från ett annat program.

  Du kan till exempel kommentera Project Workfront Planning-posten när du har kopplat Workfront-projekt med Workfront Planning-poster. Mer information finns i [Ansluta poster](/help/quicksilver/planning/records/connect-records.md).

* Kommentarer som läggs till i länkade objekt i andra program visas inte i Workfront Planning och kommentarer som läggs till länkade objekt i Workfront Planning visas inte i andra program.

  Kommentarer som läggs till i projekt i Workfront visas till exempel inte i samma projekt som är länkat till en kampanj i Workfront Planning, och kommentarer som läggs till i projektets Workfront Planning-post visas inte i Workfront.

* Du kan tagga användare eller team för att uppmärksamma dem på en uppdatering. Både individuellt taggade användare och användare från de taggade teamen får ett meddelande i appen och ett e-postmeddelande om din uppdatering.

  >[!NOTE]
  >
  >   Endast användare från kunder som har registrerat sig med Adobe Unified Experience får både ett meddelande i appen och ett e-postmeddelande. Information om hur du tar reda på om ditt företag använder Adobe Unified Experience finns i [Adobe Unified Experience för Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Du kan lägga till en uppdatering av poster och granska ändringshistoriken från följande områden i Workfront Planning:

   * Från sidan med postinformation.
   * Från en vy, i rutan postinformation.

### Hantera kommentarer på poster

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas på kort.

1. Klicka på ett kort för en posttyp.
Sidan för posttyp öppnas och alla poster av den typen visas.

1. Välj en tabellvy i **listrutan Visa** .
1. Klicka på namnet på en post i tabellvyn.

   Sidan Detaljer **för** posten öppnas. Kommentarsområdet öppnas som standard i den högra panelen.

1. (Villkorligt) Om den högra panelen inte öppnas som standard klickar du på **ikonen** Visa kommentarer![ ](assets/show-comments-icon.png)Visa kommentarer i det övre högra hörnet för att öppna avsnittet Kommentarer.

1. Börja skriva en kommentar i rutan Ny **kommentar** .

   ![Tom kommentarsfält på posten](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Om du navigerar bort från kommentaravsnittet innan du har skrivit och skickat in en kommentar behålls kommentaren på sidan i utkastläge även efter att du har loggat ut och loggat in igen. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (Valfritt) Om du vill ångra eller göra om en ändring använder du följande kortkommandon:
   * Ctrl + Z (⌘+z för Mac) för att ångra en ändring
   * Ctrl + Y (⌘+y för Mac) för att göra om en ändring
1. (Valfritt och villkorligt) Om din Workfront-instans är en del av Adobe Unified Experience lägger du till **@** följt av namnet på en användare eller ett team för att tagga dem i uppdateringen. Mer information finns i avsnittet [Att tänka på när du kommenterar en post](#considerations-about-commenting-on-a-record) i den här artikeln.

1. (Valfritt) Använd alternativen i verktygsfältet RTF för att formatera din text, lägga till emojis eller länkar till din uppdatering för att förbättra ditt innehåll.

   >[!TIP]
   >
   >Du kan inte lägga till bilder i en postkommentar.


1. Fortsätt att lägga till kommentarer i posten.

   Mer information om hur du uppdaterar objekt, inklusive Workfront Planning-poster, finns i [Uppdatera arbete](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Valfritt) Klicka på **** Mer-ikonen ![Mer-menyn](assets/more-menu.png) i det övre högra hörnet av kommentaren och klicka sedan på **Ta bort** för att ta bort kommentaren.
1. (Valfritt) **Klicka på ikonen** Dölj kommentarer![ för att stänga den](assets/hide-comments-icon.png) högra panelen.

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

Du kan granska de ändringar som gjorts i posten i avsnittet Historik i den högra panelen för en post.

Mer information finns i [Översikt](/help/quicksilver/planning/records/history-section-overview.md) över avsnittet Historik.
