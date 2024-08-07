---
product-previous: workfront-goals
navigation-topic: goal-management
title: Hantera målkommentarer i Adobe Workfront-mål
description: Du kan lägga till kommentarer till alla mål som du kan visa i Adobe Workfront-mål.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 0%

---

# Hantera målkommentarer i Adobe Workfront-mål

<!--Audited: 01/2024-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

Du kan lägga till kommentarer till alla mål som du kan visa i Adobe Workfront-mål.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> 
   <p>För den nya planen och licensstrukturen:
  <ul><li>En Ultimate-plan </li>
  eller
  <li>Ytterligare en licens för Adobe Workfront Goals för Prime- eller Select Adobe Workfront-planerna. </li></ul> </p>
<p>För aktuell plan och licensstruktur: 
<ul><li> En Pro eller högre </li>
  <li>En Adobe Workfront Goals-licens förutom en Workfront-licens.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens</td>
 <td>
 <p>Alla</td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Nytt produktkrav: Om du har planen Select eller Prime Adobe Workfront måste du också köpa ytterligare en licens för Adobe Workfront Goals. Workfront-mål ingår i den ultimata Workfront-planen.</p>
 eller
 <p>Aktuellt produktkrav: Du måste köpa ytterligare en licens för Adobe Workfront Goals för att få tillgång till de funktioner som beskrivs i den här artikeln. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivåkonfiguration</td>
 <td> <p>Visa eller öka åtkomsten till mål</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <div>
  <p>Visa eller högre behörigheter för målet</p>
  <p>Som standard får användarna ingen åtkomst till målen </p>
 <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

## Hantera målkommentarer

Du kan lägga till kommentarer till mål i uppdateringsavsnittet på målsidan.

Du kan svara på eller gilla en kommentar som du eller andra har lagt till i det här området.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet eller på ikonen **Huvudmeny** ![](assets/lines-main-menu.png) i det övre vänstra hörnet, om den är tillgänglig, och klicka sedan på **Mål** .
Detta öppnar mållistan.
1. Leta reda på målet som du vill lägga till kommentarer i och klicka sedan på namnet för att öppna målsidan.
1. Klicka på **Uppdateringar** i den vänstra panelen.
1. (Valfritt) Om du vill hitta en befintlig kommentar börjar du skriva ett nyckelord <!--or a user's name--> i rutan **Sök** i det övre högra hörnet på fliken **Kommentarer**.

   ![](assets/search-field-in-updates-tab-goals.png)

   Nyckelordet <!--or user--> som du sökte efter markeras och kommentarerna som innehåller det visas högst upp i uppdateringsavsnittet.

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >Du måste söka efter ett ord i en kommentar eller ett svar. Du kan inte söka efter taggade användare eller team.

   Mer information finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. Klicka på ikonen **x** i sökfältet för att rensa sökresultaten och återgå till den fullständiga uppdateringen.
1. Klicka på fliken **Kommentarer** i det övre vänstra hörnet i uppdateringsområdet.
1. Börja skriva en kommentar i rutan **Ny kommentar**.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Om du navigerar bort från uppdateringsavsnittet innan du är klar med att skriva och skicka en kommentar, kommer kommentaren på sidan att vara i utkastläge även efter att du loggat ut och loggat in igen. Utkast sparas i 7 dagar efter vilka de tas bort och kan inte återställas. Kommentarerna är bara synliga för användaren som skriver dem.

1. (Valfritt) Om du vill ångra eller göra om en ändring använder du följande kortkommandon:
   * CTRL + Z ( ⌘ + z för Mac) för att ångra en ändring
   * CTRL + Y ( ⌘+y för Mac) för att göra om en ändring
1. (Valfritt) Om du vill lägga till RTF-formatering i en uppdatering, en hyperlänk eller ett känslolägesikoner använder du alternativen i verktygsfältet RTF eller ikonerna intill. Mer information finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Valfritt) I området **Tagga personer eller team** börjar du skriva namnet eller e-postadressen för en användare, eller ett team som du vill inkludera i kommentaren, och markerar sedan användaren när den visas i listan.
1. Välj alternativet **Privat till mitt företag** för att göra kommentaren synlig endast för personer i ditt företag.

   >[!TIP]
   >
   >Du måste ange ett företag i din profil för att det här alternativet ska vara tillgängligt i uppdateringsområdet.

1. Klicka på **Skicka**.

   >[!TIP]
   >
   >Om en annan användare skickar en kommentar till samma objekt som du uppdaterar, visas en röd linje med en ny indikator som informerar dig om de nyare kommentarerna samt ett blått meddelande längst ned på skärmen som anger antalet nya kommentarer.
   >
   >Indikatorn visas bara när kommentaren har skickats för objektet och inte när kommentaren fortfarande är sammansatt.
   >![](assets/real-time-new-red-indicator-unified-commenting-copy.png)

1. (Valfritt) Om du vill redigera en kommentar klickar du på menyn **Mer** ![](assets/more-icon.png) till höger om ikonen Gilla och sedan på **Redigera**.
1. Redigera informationen i kommentaren eller ta bort någon av de taggade användarna.
Du kan redigera din kommentar inom 15 minuter från det att du skickat in den. En&quot;redigerad&quot; indikator läggs till till vänster om datumstämpeln som visas när kommentaren uppdaterades.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * Ett e-postmeddelande skapas för att meddela användare om din uppdatering endast när du skickar den ursprungliga uppdateringen. Inget e-postmeddelande genereras när du har redigerat uppdateringen.
   >
   > * Datumstämpeln är datumet för den ursprungliga kommentaren och inte datumet för den senaste uppdateringen.

1. (Valfritt) Klicka på menyn **Mer** ![](assets/more-icon.png) och klicka sedan på något av följande alternativ för att kopiera information från en kommentar till Urklipp eller till ett nytt svar:

   * **Kopiera länk** om du vill kopiera länken till en uppdatering, utan svaren.
   * **Kopiera brödtext** om du vill kopiera texten i en uppdatering.
   * **Citat-svar** om du vill öppna en ny kommentarsruta där den ursprungliga kommentaren citeras i ett nytt svar och markeras som ett blockcitat.

     Mer information finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Valfritt) Klicka på menyn **Mer** ![](assets/more-icon.png) till höger om en kommentar och klicka sedan på **Ta bort** för att ta bort en kommentar som du har lagt till. Mer information finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Valfritt) Klicka på **Svara** för att svara på en befintlig kommentar och följ sedan stegen 5-9 ovan. Mer information om hur du svarar på uppdateringar finns i [Svara på uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). <!--insure this stays accurate-->
1. (Villkorligt och valfritt) Om andra användare har lagt till kommentarer som visas utanför det synliga området i uppdateringsavsnittet, klickar du på **Visa** i den blå **nya kommentarsbanderollen** längst ned på skärmen för att visa dessa kommentarer.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Ytterligare kommentarer visas längst ned på skärmen.
1. (Valfritt) Klicka på ikonen **Gilla**![](assets/like-icon.png) om du vill gilla en kommentar som någon annan har lagt till. Ikonen uppdateras med antalet gilla-markeringar.

1. (Valfritt) Klicka på fliken **Systemaktivitet** för att visa uppdateringar som loggats av systemet. När ett mål uppdateras genererar Workfront en anteckning om den uppdateringen som visas på fliken Systemaktivitet. Workfront registrerar också en systemuppdatering när ett resultat, en aktivitet eller ett projekt läggs till i målet eller när det uppdateras. <!--ensure the casing on the tab has not changed-->


