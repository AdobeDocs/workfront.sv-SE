---
title: Hantera postkommentarer
description: Du kan samarbeta med poster i Adobe Maestro genom att lägga till uppdateringar och ställa frågor eller svar i kommentarområdet i en post.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Hantera postkommentarer

Du kan samarbeta i Adobe Maestro-poster genom att lägga till uppdateringar och ställa frågor eller svar i kommentarområdet i en post.

## Att tänka på när du kommenterar en post

* Du kan lägga till kommentarer och svar i driftsposter och taxonomier i Maestro, i kommentarsavsnittet i en post.

* Kommentarer som läggs till i länkade poster visas inte i de poster som du länkar från. Om du till exempel kommenterar ett projekt som är länkat till en Campaign-post, visas kommentaren bara i projektposten i Maestro och inte i kampanjposten som du länkar från.

* Kommentarer som läggs till i länkade objekt i andra program visas inte i Maestro.
Kommentarer som läggs till i länkade objekt i Maestro visas inte i andra program.\
  Kommentarer som läggs till i projekt i Workfront visas t.ex. inte i samma projekt som är länkat till en kampanj i Maestro.

* Du kan tagga användare så att de uppmärksammas på en uppdatering. Taggade användare får inga meddelanden i appen eller e-postmeddelanden om din uppdatering. Du kan inte tagga team i en Maestro-kommentar.

  >[!TIP]
  >
  >* Kommentarägare taggas inte automatiskt i en uppdatering.
  >
  >* Du kan inte ta bort taggade användare från en uppdatering när du svarar på den.

* Du kan lägga till en uppdatering till poster från följande områden i Maestro:

   * Från detaljsidan.

  <!--* From the table view.-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe product</p> </td>
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
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Alla</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### Hantera kommentarer på poster

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](assets/dots-main-menu.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](assets/lines-main-menu.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Maestro]**.

   Den senast öppnade arbetsytan öppnas som standard.
1. Välj en tabellvy på menyn **Visa** listruta.
1. Klicka på namnet på en post i tabellvyn.

   Posten **Information** sidan öppnas.

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
   * **Kopiera brödtext** t: Texten i kommentaren kopieras till Urklipp.
   * **Offertsvar**: Innehållet i kommentaren kopieras till ett nytt svar. Bilder inkluderas inte i det kopierade svaret.

   Mer information finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Valfritt) Klicka på **Mer** icon ![](assets/more-menu.png) i kommentarens övre högra hörn och klicka sedan på **Ta bort** för att ta bort kommentaren.

