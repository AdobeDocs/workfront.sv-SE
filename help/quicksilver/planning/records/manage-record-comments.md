---
title: Hantera postkommentarer
description: Du kan samarbeta om Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# Hantera postkommentarer

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Du kan samarbeta om Adobe Workfront Planning-poster genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.

I den högra panelen för en post visas följande avsnitt:

* **Kommentar**: Visar kommentarer och svar som användare lägger till i poster.
* **Historik**: Visar ändringar som användarna gör i postfälten. Mer information finns i [Översikt över avsnittet Historik](/help/quicksilver/planning/records/history-section-overview.md).

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
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller i Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Visa eller högre behörigheter på en arbetsyta</a> </p>  
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


## Att tänka på när du kommenterar en post

* Du kan lägga till kommentarer och svar till poster i Workfront Planning, under Kommentarer i en post.

* Kommentarer som läggs till i länkade poster visas inte i de poster som du länkar från. Om du till exempel kommenterar en produktpost för Workfront Planning som är länkad till en Campaign-post, visas kommentaren bara på produktposten i Workfront Planning och inte på Campaign-posten som du länkar från.

* Du kan lägga till kommentarer i Workfront Planning-poster som har skapats som ett resultat av en anslutning mellan en post och ett objekt från ett annat program.

  Du kan till exempel kommentera projektposten för Workfront Planning när du har kopplat Workfront-projekt till Workfront Planning-poster. Mer information finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).

* Kommentarer som läggs till i länkade objekt i andra program visas inte i Workfront Planning och kommentarer som läggs till i länkade objekt i Workfront Planning visas inte i andra program.

  Kommentarer som läggs till i projekt i Workfront visas t.ex. inte i samma projekt som är länkat till en kampanj i Workfront Planning, och kommentarer som läggs till i projektet Workfront Planning-posten visas inte i Workfront.

* Du kan tagga användare så att de uppmärksammas på en uppdatering. Taggade användare får inga meddelanden i appen eller e-postmeddelanden om din uppdatering. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* Du kan lägga till en uppdatering i poster och granska ändringshistoriken från följande områden i Workfront Planning:

   * Från sidan med postinformation.
   * Från en vy, i rutan med postinformation.

### Hantera kommentarer på poster

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas på kort.

1. Klicka på ett posttypskort.
Posttypssidan öppnas och alla poster av den typen visas.

1. Välj en tabellvy på menyn **Visa** listruta.
1. Klicka på namnet på en post i tabellvyn.

   Posten **Information** sidan öppnas. Kommentarsområdet öppnas som standard i den högra panelen.

1. (Villkorligt) Om den högra panelen inte öppnas som standard klickar du på **Visa kommentarer** ![](assets/show-comments-icon.png) i det övre högra hörnet för att öppna kommentarsavsnittet.

1. Börja skriva en kommentar i **Ny kommentar** box.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Om du navigerar bort från kommentarsavsnittet innan du är klar med att skriva och skicka en kommentar, kommer kommentaren på sidan att vara i utkastläge även efter att du loggat ut och loggat in igen. Alla bilder som läggs till i kommentaren sparas också i utkastet. Utkast sparas i 7 dagar efter vilka de tas bort och kan inte återställas. Kommentarerna är bara synliga för användaren som skriver dem.

1. (Valfritt) Om du vill ångra eller göra om en ändring använder du följande kortkommandon:
   * CTRL + Z ( ⌘ + z för Mac) för att ångra en ändring
   * CTRL + Y ( ⌘+y för Mac) för att göra om en ändring
1. (Valfritt) Lägg till **@** följt av namnet på en användare som ska tagga någon i uppdateringen.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (Valfritt) Använd alternativen i verktygsfältet RTF för att formatera texten, lägga till känslolägesikoner, länkar eller bilder till uppdateringen för att förbättra innehållet. Mer information finns i avsnittet&quot;Använd RTF i en Workfront-uppdatering&quot; i artikeln [Uppdatera arbete](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Om en annan användare skickar en kommentar till samma objekt som du uppdaterar finns det en röd linje med en ny indikator som informerar dig om de nyare kommentarerna.
   >
   >Indikatorn visas först när kommentaren har skickats för objektet, inte när kommentaren fortfarande är sammansatt.
   >
   >![](assets/new-line-indicator-comments.png)

1. Klicka **Skicka** för att lägga till uppdateringen i posten.
1. (Valfritt) Om du vill redigera en kommentar klickar du på **Mer** meny ![](assets/more-menu.png) i kommentarens övre högra hörn och klicka sedan på **Redigera**.

   >[!IMPORTANT]
   >
   >Du kan bara redigera kommentaren inom 15 minuter från det att du skickat in den.

1. Redigera informationen i kommentaren, lägg till eller ta bort bilder eller ta bort någon av de taggade användarna. En&quot;redigerad&quot; indikator läggs till till vänster om kommentaren.

   >[!TIP]
   >
   >Kommentarer från det aktuella året visar inte året i datumstämpeln. Om du hovrar över en tidsstämpel visas hela datumet, inklusive året.

1. (Valfritt och villkorligt) Om du vill söka efter en befintlig kommentar börjar du skriva ett nyckelord i sökrutan i det övre högra hörnet av **Kommentar** område.

   ![](assets/search-box-for-comments-area.png)

1. (Valfritt) Klicka på **Svara** eller börja skriva en kommentar i **Lägg till svar ...** för att svara på en befintlig kommentar följer du steg 4-8 ovan. <!--(**************accurate??***********)-->

1. (Villkorligt och valfritt) Om andra användare har lagt till kommentarer som visas utanför det synliga området i kommentarsavsnittet när du lade till dina kommentarer, klickar du på **Visa** innanför **banner för nya kommentarer** längst ned på skärmen för att visa dessa kommentarer.

   ![](assets/new-comments-banner-on-record.png)

   Ytterligare kommentarer visas längst ned på skärmen.

1. (Valfritt) Klicka på **Gilla** om du vill gilla en uppdatering eller bekräfta att du har läst den. Ikonen uppdateras med antalet gilla-markeringar.
1. (Villkorligt och valfritt) Om du har tagit med ytterligare personer i kommentaren klickar du på avatarerna för de användare som ingår i uppdateringen för att visa en lista över de användare som kommentaren delas med.
1. (Valfritt) Klicka på **Mer** icon ![](assets/more-menu.png) i kommentarens övre högra hörn och klicka på något av följande alternativ för att kopiera information från en kommentar:

   * **Kopiera länk**: Detta kopierar en länk till kommentaren till Urklipp.
   * **Kopiera brödtext**: Texten i kommentaren kopieras till Urklipp.
   * **Offertsvar**: Innehållet i kommentaren kopieras till ett nytt svar. Bilder inkluderas inte i det kopierade svaret.

   Mer information finns i [Uppdatera arbete](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Valfritt) Klicka på **Mer** icon ![](assets/more-menu.png) i kommentarens övre högra hörn och klicka sedan på **Ta bort** för att ta bort kommentaren.
1. (Valfritt) Klicka på **Dölj kommentarer** icon ![](assets/hide-comments-icon.png) för att stänga den högra panelen.

## Översikt över avsnittet Historik

Du kan granska ändringarna som gjorts i posten i historikavsnittet på den högra panelen i en post.

Mer information finns i [Översikt över avsnittet Historik](/help/quicksilver/planning/records/history-section-overview.md).
