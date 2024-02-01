---
title: Hantera postkommentarer
description: Du kan samarbeta med poster i Adobe Maestro genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 0%

---


# Hantera postkommentarer

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Du kan samarbeta med poster i Adobe Maestro genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.

I den högra panelen för en post visas följande avsnitt:

* **Kommentar**: Visar kommentarer och svar som användare lägger till i poster.
* **Historik**: Visar ändringar som användarna gör i postfälten. Mer information finns i [Översikt över avsnittet Historik](/help/quicksilver/maestro/records/history-section-overview.md).

>[!TIP]
>
>På den högra panelen visas både för driftsposter och taxonomiposter.


## Att tänka på när du kommenterar en post

* Du kan lägga till kommentarer och svar i driftsposter och taxonomier i Maestro, i kommentarsavsnittet i en post.

* Kommentarer som läggs till i länkade poster visas inte i de poster som du länkar från. Om du till exempel kommenterar en Maestro-produktpost som är länkad till en Campaign-post, visas kommentaren bara i produktposten i Maestro och inte i Campaign-posten som du länkar från.

* Du kan lägga till kommentarer i Maestro-poster som har skapats som ett resultat av en anslutning mellan en Maestro-post och ett objekt från ett annat program.

  Du kan t.ex. kommentera Project Maestro-posten när du har kopplat Workfront-projekt till Maestro-poster. Mer information finns i [Koppla poster](/help/quicksilver/maestro/records/connect-records.md).

* Kommentarer som lagts till i länkade objekt i andra program visas inte i Maestro och kommentarer som lagts till i länkade objekt i Maestro visas inte i andra program.

  Kommentarer som läggs till i projekt i Workfront visas t.ex. inte i samma projekt som är länkat till en kampanj i Maestro, och kommentarer som läggs till i projektet Maestro visas inte i Workfront.

* Du kan tagga användare så att de uppmärksammas på en uppdatering. Taggade användare får inga meddelanden i appen eller e-postmeddelanden om din uppdatering. <!--this might change??-->

* Du kan lägga till en uppdatering i poster och granska ändringshistoriken från följande områden i Maestro:

   * Från sidan Detaljer för en post eller taxonomi.

  <!--* From the table view.-->

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
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <td> <p>Det finns inga åtkomstnivåkontroller i Maestro. </p>  
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
   <td> <p>Din Workfront- eller gruppadministratör måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Hantera kommentarer på poster

{{step1-to-maestro}}

Den senast öppnade arbetsytan öppnas som standard.
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
1. (Valfritt) Använd alternativen i verktygsfältet RTF för att formatera texten, lägga till känslolägesikoner, länkar eller bilder till uppdateringen för att förbättra innehållet. Mer information finns i avsnittet&quot;Använd RTF i en Workfront-uppdatering&quot; i artikeln [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

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

   Mer information finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Valfritt) Klicka på **Mer** icon ![](assets/more-menu.png) i kommentarens övre högra hörn och klicka sedan på **Ta bort** för att ta bort kommentaren.
1. (Valfritt) Klicka på **Dölj kommentarer** icon ![](assets/hide-comments-icon.png) för att stänga den högra panelen.

## Översikt över avsnittet Historik

Du kan granska ändringar som gjorts i posten i historikavsnittet på den högra panelen i en driftspost eller taxonomi.

Mer information finns i [Översikt över avsnittet Historik](/help/quicksilver/maestro/records/history-section-overview.md).

