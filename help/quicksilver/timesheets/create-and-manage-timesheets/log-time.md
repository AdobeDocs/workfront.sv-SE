---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Loggtid
description: Du kan logga tid för arbetsobjekt i &nbsp;Adobe Workfront för att ange hur många timmar du ska arbeta med dem. Du kan också logga tid som inte är relaterad till arbetet, som semester, sjuktid eller tid som du tillbringar i möten. Den tid du loggar visas i tidrapporten.
author: Alina
feature: Timesheets
role: User
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '3583'
ht-degree: 0%

---

# Loggtid

<!--Audited: 12/2023-->

<!--remove all preview and production references from this article with 23.3 release-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). 

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

Du kan logga tiden för arbetsobjekt i Adobe Workfront för att ange hur många timmar du ska arbeta med dem. Du kan också logga tid som inte är relaterad till arbetet, som semester, sjuktid eller tid som du tillbringar i möten. Den tid du loggar visas i tidrapporten.

Mer information om vilka timmar du kan logga in i Workfront finns i [Hantera timtyper](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln och logga Project Specific hours:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: 
   <ul><li>Ljus eller högre för att logga allmänna timmar i en tidrapport</li>
   <li>Standard för att logga timmar i ett projekt, en uppgift eller ett ärende</li></ul>


<p>Aktuell: 
   <ul><li>Granska eller senare för att logga allmänna timmar i en tidrapport</li>
   <li>Arbeta eller senare för att logga timmar i ett projekt, en uppgift eller ett ärende</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till den typ av arbetspost som du loggar tid för </p> <p>Du behöver till exempel Redigera-åtkomst till Problem för att kunna logga tid för problem</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter för det arbetsobjekt du loggar tid för, inklusive behörigheter för loggtimmar</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du loggar tid i Workfront

* Du kan logga tid för projekt, uppgifter eller problem eller logga tid direkt i tidrapporten.

  Mer information om hur du skapar tidrapporter finns i [Skapa en tidrapport för engångsbruk](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* All tid som loggas via andra verktyg än tidrapporten visas i tidrapporten för motsvarande tidsperiod.
* Uppgifter och ärenden i ett projekt som inte är aktuellt fylls inte i i förväg i en tidrapport.
* Den tid som är inloggad i tidrapporten används omedelbart för uppgiften, utgåvan eller projektet.
* Tidrapporter innehåller den totala tiden för alla loggade datum. Helger inkluderas alltid, även när tidslinjeberäkningar har konfigurerats för att exkludera dem (enligt beskrivningen i [Konfigurera systemomfattande projektinställningar](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* Det maximala antalet objekt som visas i en tidrapport är 45. Om det finns fler än 45 objekt vars datum matchar tidsramen för tidrapporten visas endast de senast uppdaterade objekten.
* Timposter som ingår i fakturerade faktureringsposter är nedtonade och kan inte redigeras i tidrapporten. Mer information finns i [Skapa faktureringsposter](../../manage-work/projects/project-finances/create-billing-records.md).
* Personliga uppgifter visas inte som standard i tidrapporten. Personliga uppgifter visas bara i tidrapporten när de har loggat tid. När du har loggat tiden för en personlig uppgift kan du fästa uppgiften på tidrapporten och den kommer att finnas kvar på tidrapporten om den är fäst. Mer information finns i [Skapa arbetsobjekt från startdelen](../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Loggtid {#log-time-section}

Du kan logga tid i följande områden i Workfront:

* [Tidrapport](#timesheet)
* [Startsida](#home)
* [Projekt, uppgift eller utleverans](#project-task-or-issue)
* [Panelen Sammanfattning](#summary-panel)
* [Varumärkena](#boards)
* [Mobilapp](#mobile-app)

### Tidrapport {#timesheet}

#### Logga tid på en tidrapport {#log-time-on-a-timesheet}

Du kan logga tid på följande objekt i tidrapporten:

* I förväg ifyllda uppgifter, utgåvor och projekt som visas automatiskt, baserat på hur Workfront-administratören anger tidrapportinställningarna. Information om hur tidrapporter fylls i i förväg finns i [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  Endast de uppgifter och utgåvor som du har tilldelats är ifyllda i tidrapporten. Uppgifter och ärenden som tilldelats dina team eller jobbroller fyller inte i din tidrapport automatiskt.

  Om du klickar på Arbeta på ett objekt som har tilldelats dina team tilldelas objektet till dig och objektet visas i tidrapporten.

* Uppgifter, ärenden eller projekt som du lägger till manuellt.
* Uppgifter, ärenden eller projekt som du redan har loggat in på någon annan plats i Workfront.
* Allmän tid (semester, utbildning, overheadtime).

>[!NOTE]
>
>Granska användare som tilldelats en tidrapportprofil kan se området Tidrapporter och logga allmänna timmar. De kan dock inte logga timmar för uppgifter eller ärenden som tilldelats dem och som visas på tidrapporten.

Så här loggar du tid på en tidrapport:

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) längst upp till vänster.

1. Klicka [!UICONTROL **Tidrapporter**]. Din aktuella tidrapport visas som standard.
   ![Tidrapport](assets/timesheet-redesigned-nwe.png)


1. (Valfritt) Klicka på **helskärm** icon ![](assets/full-screen.png) om du vill visa tidrapporten i helskärmsläge klickar du på **exit-full-screen** ![](assets/exit-full-screen.png) -ikonen för att återgå till tidrapporten.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Valfritt) Om du vill lägga till ett projekt, en uppgift eller ett problem i tidrapporten klickar du på knappen **Lägg till objekt** nedrullningsbar meny i det övre vänstra hörnet av tidrapporten och klicka sedan på **Lägg till projekt**, **Lägg till aktiviteter**, eller **Lägg till problem**.

   En lista med projekt, uppgifter eller problem visas.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Valfritt) Klicka på sökikonen ![Söka efter ett objekt](assets/search-icon.png) om du vill söka efter ett visst objekt med hjälp av ett nyckelord som ska läggas till i tidrapporten.

1. (Valfritt) Expandera listrutorna för filter, vy och gruppering för att tillämpa eller anpassa en och visa önskad objektinformation.

1. Markera ett eller flera objekt i listan och klicka sedan på **Lägg till**.

   Om du har lagt till färre än 50 objekt samtidigt läggs objekten till i tidrapporten. Uppgifter och ärenden visas under namnet på projektet.

   >[!NOTE]
   >
   >När du lägger till uppgifter eller utgåvor i tidrapporten läggs även projektet till.


1. (Villkorligt) Om du lägger till 50 eller fler objekt samtidigt visas ett bekräftelsemeddelande med antalet objekt som har lagts till i tidrapporten.

   Klicka **Lägg till alla** om du vill lägga till alla objekt eller klicka **Avbryt** om du vill sluta lägga till de markerade objekten, och sedan **Avbryt** för att stänga listan med objekt.

   Uppgifter och ärenden visas under namnet på projektet.

   >[!NOTE]
   >
   >Objekten som du lägger till manuellt i tidrapporten är fästa och kommer att finnas kvar på aktuella och framtida tidrapporter tills du tar bort dem manuellt. Information om hur du tar bort objekt från tidrapporten genom att ta bort dem finns i steg 10.

   <!--(ensure this stays accurate)-->

1. (Valfritt) Klicka på **Komprimera** ![](assets/collapse-icon.png) eller **Expandera** ![](assets/expand-icon.png) -ikoner bredvid projektnamnet för att antingen visa eller dölja listan med uppgifter och ärenden för projektet.


   >[!TIP]
   >
   >   När du använder ett vanligt QWERTY-tangentbord och klickar på namnet på ett projekt i tidrapporten trycker du på följande uppsättning tangenter för att komprimera eller utöka projektet:
   >   * Så här expanderar du projektet och visar dess arbetsobjekt:
   >     * Skift + Alt + Uppil för Windows-datorer
   >     * Skift + Alt + Uppil för Mac-datorer
   >   * Så här komprimerar du projektet och döljer dess arbetsobjekt:
   >     * Skift + Alt + Nedpil för Windows-datorer
   >     * Skift + Alt + Nedåtpil för Mac-datorer.


1. (Valfritt) Om du vill fästa ett objekt som visas på tidrapporten automatiskt manuellt håller du pekaren över objektets namn och klickar på **fäst** icon ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   När du använder ett vanligt QWERTY-tangentbord efter att ha klickat på ett objekt i tidrapporten trycker du på följande uppsättning tangenter för att fästa ett objekt:
   >   * Alternativ + P för både Windows- och Mac-datorer.


1. (Valfritt) Klicka på sökikonen ![](assets/search-icon.png) och börja skriva ett nyckelord för att hitta ett projekt, en uppgift eller ett problem i tidrapporten.

1. (Villkorligt) Om Workfront- eller gruppadministratören har aktiverat **Tilldela jobbroller till timposter manuellt** väljer du en jobbroll i listrutan. Den roll som anges när du tilldelas arbetsuppgiften visas som standard. Om du inte har tilldelats någon roll för objektet visas din primära roll som standard. Mer information om inställningen finns i artikeln [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![Loggtid för flera roller i tidrapporten](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Valfritt) Klicka på **+** om du vill lägga till ytterligare en rad och sedan välja en ny timtyp i listrutan i dialogrutan [!UICONTROL Hour Type] kolumn för att logga tid för en annan timtyp.

   ![Nedrullningsbar meny för timtyp](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)


   >[!TIP]
   >
   >   Beroende på operativsystem eller webbläsare och när du använder ett vanligt QWERTY-tangentbord trycker du på följande uppsättning med tangenter för att lägga till ytterligare en rad:
   >   * Ctrl + Alt + + + för Windows-datorer
   >   * Cmd + Option + + för Mac-datorer

   Timtyper är tillgängliga beroende på vad som har definierats på system-, projekt- och användarnivå, vilket beskrivs i [Definiera timtyper och tillgänglighet för tidrapporter](define-hour-types-and-availability.md).

   Timtypen kan inte ändras efter att en tidrapport har stängts.

   >[!TIP]
   >
   >Om du tidigare loggade tid och timtypen som du valde nu är inaktiverad tonas hela raden för den loggade tiden ned. Om du väljer en annan timtyp och uppdaterar sidan tas alternativet för inaktiverad timtyp bort från listrutan så att du inte kan lägga till ytterligare timmar till den timtypen.
   >
   >Överväg att lägga till en ny rad för arbetsuppgiften som du vill logga ytterligare tid för och välja en ny timtyp om du vill behålla den inaktiverade timtypen som är kopplad till den senaste loggade tiden.

1. Klicka på **delete** icon  ![](assets/delete.png) bredvid jobbrollen för att ta bort den. När du loggat för rollen tas även den bort.

   >[!TIP]
   >
   >   Beroende på operativsystem eller webbläsare och när du använder ett vanligt QWERTY-tangentbord trycker du på följande uppsättning tangenter för att ta bort en rad:
   >   * Ctrl + Alt + - för Windows-datorer
   >   * Cmd + Option + - för Mac datorer

1. Ange hur lång tid du vill logga in en viss dag i tidslinjesektionen i tidrapporten och klicka sedan utanför timrutan för att spara timposten. Timmarna sparas automatiskt. Raden som du loggar tid för markeras med ljusblått och rutan för timuppgifterna markeras med mörkblått.

   ![Loggtidsruta i tidrapport](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   Du loggar tid i timmar eller dagar. Den här inställningen konfigureras av användare med en planlicens eller av systemadministratören, vilket beskrivs i [Konfigurera om tid är inloggad i timmar eller dagar](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Du måste spara tidrapporten manuellt om något av följande inträffar:
   >
   >* Jobbrollen som är associerad med tiden som du loggade tidigare har ändrats och **Tilldela jobbroller till timposter manuellt** inställningen har inaktiverats. Loggningstiden för nya datum associeras med en annan jobbroll.
   >   
   >   Om rollen har ändrats och **Tilldela jobbroller till timposter manuellt** om inställningen är aktiverad kan du logga tid eller uppdatera rollen och dina ändringar sparas automatiskt.
   >
   >* Jobbrollen som tilldelats en aktivitet eller ett problem skiljer sig från jobbrollen som tidrapportägaren loggar tid med <!--or assigned to them_ this last  piece came from a Support note but but sure what role it's referring to. Leaving it out for now.-->.
   >
   >Tidrapporten kommer att spara tiden automatiskt igen när det inte finns fler motstridiga poster mellan de två rollerna.
   >

1. (Valfritt) Ange mängden övertid i fältet Övertid i tidrapporthuvudet.

   >[!TIP]
   >
   >Du kan inte logga ett större antal övertidstimmar än det aktuella totala antalet timmar på tidrapporten. Om du till exempel har loggat 7 timmar på tidrapporten hittills kan du inte logga 8 timmars övertid.

1. (Valfritt) Klicka på **Kommentar** för att lägga till en kommentar för timbidraget.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   När du använder ett vanligt QWERTY-tangentbord när du har klickat på rutan för timmatning, trycker du på följande uppsättning tangenter för att öppna kommentarsrutan:
   >   * Skift+F2 för både Windows- och Mac-datorer.

1. Klicka **Klar** för att spara kommentaren.

   >[!TIP]
   >
   >   När du använder ett vanligt QWERTY-tangentbord kan du trycka på följande uppsättning tangenter i kommentarsrutan för att spara kommentaren:
   >   * Ctrl + Retur för Windows-datorer.
   >   * Cmd + Retur för Mac-datorer.


1. (Valfritt) Klicka på **Visa kommentarer** i verktygsfältet om du vill visa timkommentarer under arbetsuppgiften.

   ![Kommentarer som anges under objektet i tidrapporten](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Alla ändringar du gör i tidrapporten sparas automatiskt.

1. (Valfritt) Klicka på raden för en uppgift eller ett problem och klicka sedan på **Öppna sammanfattning** i det övre högra hörnet av tidrapporten om du vill lägga till en uppdatering eller uppdatera information om uppgiften eller problemet. Panelen Sammanfattning öppnas till höger.

   ![summary-panel-for-task-opened-in-tidrapport](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Din uppdatering visas i uppdateringsområdet för den arbetsuppgift som är associerad med den loggade tiden.

   >[!TIP]
   >
   >Du kan inte kommentera projekt eller allmänna timtävlingsbidrag för tid.

1. Klicka [!UICONTROL **Stäng sammanfattning**] för att stänga panelen Sammanfattning och återgå till tidrapporten.

1. (Valfritt) Klicka på [!UICONTROL **Uppdateringar**] i den vänstra panelen och lägg sedan till en uppdatering i tidrapporten. Mer information om Workfront-uppdateringar finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesigned-tidrapport-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

1. (Valfritt) Gå tillbaka till **Tidrapport** området där du vill stänga eller skicka tidrapporten.

   * **Stäng**: Stäng tidrapporten när du är klar med uppdateringen. Det här alternativet är endast tillgängligt när din tidrapport inte är kopplad till en godkännare.

   * **Skicka för godkännande:** Det här alternativet är bara tillgängligt om det finns en godkännare på tidrapporten. Spara ändringarna och skicka in för godkännande. Du kan öppna tidrapporten när du har stängt den genom att klicka på **Återkalla**, om ett godkännande ännu inte har beviljats. Mer information finns i [Skicka en tidrapport för godkännande](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Avvisa**: Det här alternativet visas när du är en tidrapportgodkännare och tidrapporten har skickats till dig för godkännande. Om du klickar på den ändras tidrapportens status till Avvisat och tidrapporten förblir öppen.

   * **Godkänn**: Det här alternativet visas när du är en tidrapportgodkännare och tidrapporten har skickats till dig för godkännande. Om du klickar på den ändras tidrapportens status till Godkänd och tidrapporten stängs.

   >[!TIP]
   >
   >Alternativen Avvisa och Godkänn visas också på tidrapporten när du är systemadministratör och tidrapporten är kopplad till en godkännare.

1. (Villkorligt) Om du har stängt eller skickat in tidrapporten för godkännande klickar du på något av följande alternativ:

   * **Öppna igen**: Det här alternativet är tillgängligt för tidrapporter som du redan har stängt och som inte har några godkännare, eller tidrapporter som redan har godkänts. Öppna tidrapporten igen om du vill ändra timposter.
   * **Återkalla**: Det här alternativet är tillgängligt för tidrapporter som har skickats in för godkännande men ännu inte har godkänts eller avvisats. Klicka **Återkalla** för att öppna tidrapporten igen och ändra timinmatningar.

#### Ta bort ett objekt från tidrapporten

Du kan ta bort en timpost eller en artikel (projekt, uppgift eller utgåva) från en tidrapport.

Så här tar du bort en timpost från en tidrapport:

1. Gå till tidrapporten och hitta timposten som du vill ta bort.
1. Ersätt de angivna timmarna med 0 eller Ta bort timmarna och ersätt dem med 0 och tryck sedan på Retur.

   Timmarna tas bort och tidrapporten sparas automatiskt.

Du kan ta bort ett objekt (projekt, uppgift eller utgåva) från tidrapporten genom att ta bort dess fästen, om du ännu inte har loggat in på den, och om du har lagt till objektet manuellt (vilket beskrivs i steg 4-8 i [Logga tid på en tidrapport](#log-time-on-a-timesheet) i den här artikeln). <!--ensure this stays accurate-->

Du kan inte ta bort objekt som ingår i tidrapporten automatiskt enligt tidrapportinställningarna i ditt Workfront-system eller -grupp som är konfigurerade att fylla i tidrapporterna i förväg (enligt beskrivningen i [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)). Objekten stoppar förifyllning av tidrapporten när datumen för objekten ligger utanför tidsramen i tidrapporten.

Så här tar du bort ett objekt från tidrapporten som har lagts till manuellt:

1. Kontrollera att ingen tid är inloggad mot objektet.
1. Klicka på **ta bort** icon ![Fäst ett objekt](assets/pin-icon.png) bredvid objektet för att ta bort fästet för objektet från tidrapporten.

   >[!TIP]
   >
   >   När du använder ett vanligt QWERTY-tangentbord efter att ha klickat på ett objekt i tidrapporten trycker du på följande uppsättning tangenter för att ta bort ett objekt:
   > * Alternativ + P för både Windows- och Mac-datorer.

   Objektet tas bort från tidrapporten när du har uppdaterat sidan.

### Startsida {#home}

Du kan logga projektspecifik tid i Hem.

Allmän information om hur du använder området Hem finns i följande avsnitt:

* Mer information om hur du använder det äldre Hem-området finns i [Använda området Hem](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).
* Mer information om hur du använder den nya hemområdet finns i [Kom igång med Nytt hem](../../workfront-basics/using-home/new-home/get-started-with-new-home.md).

#### Logga tid på ett arbetsobjekt från den nya hemsidan

Du kan logga tid på uppgifter och problem i alla widgetar med hjälp av panelen Sammanfattning i Hem-området. Mer information finns i [Panelen Sammanfattning](#summary-panel) i den här artikeln.

Om du dessutom vill logga tiden för ett objekt i widgeten Mitt arbete:

1. Till **Startsida** område.
1. Lägg till **Mitt arbete** widgeten till ditt hem.
1. (Valfritt) Välj en uppgift, ett problem eller en förfrågan i en lista och klicka sedan på **Arbeta på den**
1. Håll muspekaren över uppgiften eller problemet som du vill logga in på och klicka sedan på **Loggtid** icon ![](assets/log-time-icon-in-new-home.png) till höger om uppgiftsinformationen.

   ![](assets/log-time-ui-for-task-from-new-home.png)

1. Klicka **Loggtid**.

   Den loggade tiden visas i objektets Timmar-avsnitt och i din tidrapport.

#### Logga tid på ett arbetsobjekt från det äldre hemområdet

1. I **Arbetslista** markerar du det objekt där du vill logga tid.
1. Klicka på i den högra panelen **Loggtid**.

   ![](assets/log-time-home-350x181.png)

1. I **Ange timmar** väljer du lämplig timtyp.\
   Timtyper är tillgängliga beroende på vad som har definierats på system-, projekt- och användarnivå, vilket beskrivs i [Definiera timtyper och tillgänglighet för tidrapporter](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Villkorligt) Om Workfront- eller gruppadministratören har aktiverat **Tilldela jobbroller till timposter manuellt** väljer du en jobbroll i listrutan. Den roll som anges när du tilldelas arbetsuppgiften visas som standard. Om du inte har tilldelats någon roll för objektet visas din primära roll som standard. Mer information om inställningen finns i artikeln [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Ange vilken tid du vill logga och klicka sedan på **Loggtid**.

   Den loggade tiden visas i objektets Timmar-avsnitt och i din tidrapport.

### Projekt, uppgift eller utleverans {#project-task-or-issue}

Du kan logga projektspecifik tid för ett projekt, en uppgift eller ett problem i följande avsnitt:

* [Uppdateringsavsnitt](#updates-section)
* [Avsnittet Timmar](#hours-section)

#### Uppdateringsavsnitt{#updates-section}

Om du vill logga tid i uppdateringsavsnittet för ett projekt, en uppgift eller ett problem måste du ha följande:

* Korrekt åtkomst och behörigheter enligt beskrivningen i [Åtkomstkrav](#access-requirements) i den här artikeln.

* Din Workfront-administratör måste aktivera loggtiden direkt i projektinställningarna under [!UICONTROL **Tidrapport och timmar**]> [!UICONTROL **Inställningar**] i systemområdet om du vill logga tiden direkt till ett projekt.

  Mer information om hur du tillåter användare att logga timmar direkt till projekt finns i [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Så här loggar du tid i uppdateringsavsnittet för ett projekt, en uppgift eller ett problem:

1. Gå till ett projekt, en uppgift eller ett ärende.
1. I den vänstra panelen väljer du **Uppdateringar**.
1. Klicka **Loggtid**. <!-- did Anna B change the casing for this button? If yes and if she changed it for the other areas, update screen shot too-->

   Dialogrutan Loggtid visas.

   >[!TIP]
   >
   >   Om din profils inställning är att logga tid i dagar visas rutan Ange dagar.
   >   
   >   I det övre högra hörnet av rutan Ange dagar finns en indikation på hur många timmar en dag ska ha.

   ![](assets/log-time-box-in-updates-stream.png)

1. Ange följande information:

   * **Timtyp**: Välj en timtyp på den nedrullningsbara menyn, om den skiljer sig från den som visas som standard.

     Beroende på vilka timtyper som är konfigurerade i systemet kan alternativen här variera. Mer information om hur du konfigurerar timtyper finns i [Definiera timtyper och tillgänglighet för tidrapporter](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Jobbroll**: (Villkorligt) Om Workfront- eller gruppadministratören har aktiverat **Tilldela jobbroller till timposter manuellt** inställning, välja en **Jobbroll** i listrutan. Den roll som anges när du tilldelas till objektet visas som standard. Om du inte har tilldelats en roll för objektet visas din primära roll som standard. Mer information om inställningen finns i artikeln [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   * **Timmar**: Ange antalet timmar för projektet, uppgiften eller utgåvan.

1. Klicka **Loggtid**.

   Den loggade tiden visas i objektets Timmar-avsnitt och i din tidrapport.

#### Avsnittet Timmar{#hours-section}

Du måste vara Workfront-administratör för att kunna logga tid för projekt, uppgifter och problem i timavsnittet,

eller

Du måste ha alla följande:

* En planlicens med administrativ åtkomst till tidrapporter och timmar. Mer information om hur du ger administrativ åtkomst till tidrapporter och timmar finns i [Ge användarna administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* Contribute eller högre behörigheter för projektet med åtkomst till loggtimmar. Mer information om att bevilja behörigheter för projekt finns i [Dela ett projekt i Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* Din Workfront-administratör måste aktivera loggtiden direkt i projektinställningarna i **Tidrapport och timmar > Inställningar** under Konfigurera om du vill logga tiden direkt till ett projekt. Mer information om hur du tillåter användare att logga timmar direkt till projekt finns i [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Så här loggar du tid i timavsnittet för ett projekt, en uppgift eller ett problem:

1. Gå till ett projekt, en uppgift eller ett ärende.
1. Klicka på i den vänstra panelen **Timmar**.
1. Klicka **Loggtid**.

   Dialogrutan Loggtimmar visas.

1. Ange följande information:

   * **Ägare:** Ditt namn visas i det här fältet som standard.\
     Om du loggar timmarna för en annan användare anger du användarens namn.

   * **Timtyp**: Välj en timtyp på den nedrullningsbara menyn, om den skiljer sig från den som visas som standard.

     Beroende på vilka timtyper som är konfigurerade i systemet kan alternativen här variera. Mer information om hur du konfigurerar timtyper finns i [Definiera timtyper och tillgänglighet för tidrapporter](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Jobbroll**: (Villkorligt) Om Workfront- eller gruppadministratören har aktiverat **Tilldela jobbroller till timposter manuellt** inställning, välja en **Jobbroll** i listrutan. Den roll som anges när du tilldelas till objektet visas som standard. Om du inte har tilldelats en roll för objektet visas din primära roll som standard. Mer information om inställningen finns i artikeln [Konfigurera tidrapport och timinställningar](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     ![](assets/log-time-box-in-hours-section-on-task.png)
   * **Timmar**: Ange antalet timmar för projektet, uppgiften eller utgåvan.

1. Klicka **Loggtid**.

### Panelen Sammanfattning

Du kan logga tid för uppgifter och problem på panelen Sammanfattning.
Mer information finns i [Sammanfattning](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Varumärkena {#boards}

Du kan logga in på anslutna kort på ett Workfront-kort. Detta är samma process som när du loggar tid för en uppgift eller ett problem, och de timmar som är inloggade på kortet sparas för den anslutna aktiviteten eller problemet.
Mer information finns i [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Mobilapp {#mobile-app}

Du kan logga tid från Workfront mobilapp.
Mer information finns i [Adobe Workfront för Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) eller [Adobe Workfront för iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
