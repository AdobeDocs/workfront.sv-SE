---
product-area: reporting
navigation-topic: reporting-elements
title: Skapa eller redigera vyer i Adobe Workfront
description: Du kan anpassa vilken typ av information som visas på skärmen med hjälp av vyer. Du kan använda flera typer av vyer i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '1777'
ht-degree: 0%

---

# Skapa eller redigera vyer i Adobe Workfront

Du kan anpassa vilken typ av information som visas på skärmen med hjälp av vyer. Du kan använda flera typer av vyer i Adobe Workfront.

I den här artikeln beskrivs hur du skapar och redigerar standardvyer för listor och rapporter, och hur du skapar Agile-vyer. Mer information finns i [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att skapa en vy i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter till en rapport för att skapa eller redigera en vy i en rapport</p> <p>Hantera behörigheter till en vy för att redigera den</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa eller anpassa en vy

Hur du skapar eller anpassar en vy varierar beroende på om du skapar eller anpassar en standardvy eller en flexibel vy.

* [Skapa eller anpassa en standardvy](#create-or-customize-a-standard-view)
* [Skapa eller anpassa en Agile-vy](#create-or-customize-an-agile-view)

### Skapa eller anpassa en standardvy {#create-or-customize-a-standard-view}

Du kan skapa en ny standardvy eller anpassa en befintlig standardvy som du skapade tidigare.

1. Klicka på **Visa** nedrullningsbar meny i en lista där du vill skapa eller anpassa en vy.
1. (Valfritt) Om du vill anpassa en befintlig vy väljer du den standardvy som du vill anpassa.\
   Standardvyer är tillgängliga för alla typer av listor i Workfront, till exempel rapporter, projektlistor och uppgiftslistor.
1. Klicka på **Visa** nedrullningsbar meny och klicka sedan på **Anpassa vy** eller **Ny vy**.\
   The **Anpassa vy** visas.

1. I **Förhandsgranska kolumn** gör du något av följande:

   * Ändra värdet för en kolumn genom att klicka på kolumnrubriken och sedan markera ett nytt fält.
   * Lägg till en kolumn genom att klicka **Lägg till kolumn** börjar du skriva namnet på den kolumn som du vill lägga till och klickar sedan på den när den visas i listrutan.
   * Justera den ordning som kolumnerna visas i genom att dra kolumnrubriken till en ny plats.

      * (Valfritt) I dialogrutan **Kolumninställningar** klickar du på **Sammanfatta den här kolumnen med** och välj sedan ett av de tillgängliga alternativen för att sammanfatta informationen. När du väljer det här alternativet sammanställs informationen i kolumnen i rapportens grupperingar.\
        För datumfält kan du sammanfatta värdena med följande alternativ:

         * Maximal
         * Minimum

        För tal- och valutafält kan du sammanfatta värdena med följande alternativ:

         * Antal
         * Summa
         * Genomsnittlig
         * Maximal
         * Minimum

        >[!NOTE]
        >
        >Följande undantag gäller för överordnade objekt (till exempel överordnade uppgifter) när du samlar värden för följande fält i grupperingar:
        >   
        >   * Alla sifferfält och valutafält utom Faktiska timmar (till exempel Planerad/Faktisk arbetskostnad, Planerad/Faktisk utgiftskostnad, Planerad/Faktisk kostnad, Planerad timmar) samlar endast värdena för de underordnade aktiviteterna och fristående aktiviteter. De sammanställer inte värdena för de överordnade uppgifterna eller de överordnade överordnade uppgifterna.
        >   * Faktiska timmar sammanställer värdena för huvuduppgiften och de fristående uppgifterna. de sammanställer inte siffrorna för överordnade och underordnade uppgifters överordnade uppgifter.
        >   * Anpassade datafält för tal- och valutavärden samlar alla uppgifter: föräldrar, barn, föräldrar till föräldrar och fristående uppgifter.
        >   
        >

        Mer information om hur du använder grupperingar i en rapport finns i artikeln [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Valfritt) Klicka på **Avancerade alternativ** om du vill ange följande information för kolumnen:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Etikett för anpassad kolumn</strong></td> 
           <td><p>Ange en anpassad etikett för kolumnen. Den här etiketten ersätter standardetiketten.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Fältformat</strong></td> 
           <td>Välj i vilket format du vill att värdena ska visas för fälten i kolumnen.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Visa den här kolumnen när du arbetar på en instrumentpanel</strong></td> 
           <td><p>Välj det här alternativet om du vill visa den här kolumnen på en kontrollpanel när rapporten visas sida vid sida med en annan rapport. När det här alternativet är avmarkerat visas inte den här kolumnen när du visar rapporten på en kontrollpanel där rapporter visas sida vid sida.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Kolumnregler</strong></td> 
           <td><p>Klicka <strong>Lägg till en regel för den här kolumnen</strong> för att definiera en regel för kolumnen. När du har lagt till en regel kan du definiera fält- och textformat för hur fält som matchar den regeln visas. Klicka <strong>Lägg till regel</strong> efter att du har definierat regeln.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Mer information om villkorlig formatering av vyer i rapporter finns i artikeln [Använda villkorsstyrd formatering i textläge](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Villkorligt) Om du klickade **Avancerade alternativ**, klicka **Klar**.

1. Klicka **Spara vy** om du vill skapa en ny vy eller ersätta den aktuella vyn med dina ändringar.\
   eller\
   Klicka **Spara som ny vy** för att spara ändringarna som en ny vy.

   >[!TIP]
   >
   >The **Spara som ny vy** är det enda tillgängliga alternativet när du anpassar en inbyggd Workfront-vy.

   Åtkomsten styr hur vyn sparas. Om du skapade vyn från början kan du spara ändringarna; i annat fall uppmanas du att spara en version. Tänk på att de ändringar du gör i vyn påverkar användare som vyn har delats med.

### Skapa eller anpassa en Agile-vy {#create-or-customize-an-agile-view}

Du kan skapa en ny Agile-vy eller anpassa en befintlig Agile-vy som du tidigare har skapat.

>[!IMPORTANT]
>
>Flexibla vyer är bara tillgängliga när du visar ett projekt.

Mer information om Agile-vyer finns i artikeln [Hantera ett projekt i Agile-vyn](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
>Den här proceduren gäller endast för den äldre Agile-vyn, inte för styrelsevyn för ett projekt.

Så här skapar eller anpassar du en Agile-vy:

1. Gå till listan med uppgifter i ett projekt.
1. Klicka på **styrelse** icon ![Ikon för anslagstavla](assets/board-icon-for-agile-view.png)och klicka sedan på **Använd äldre flexibilitet** i styrelseläget.

1. (Villkorligt) Så här anpassar du en befintlig Agile-vy:

   1. Klicka på **Visa** och välj sedan den Agile-vy som du vill anpassa.\
      Du kan inte anpassa Agile-standardvyn.

   1. Klicka på **Visa** nedrullningsbar meny igen och klicka sedan på **Anpassa vy**.\
      ![](assets/view-agile-customize.png)

1. (Villkorligt) Klicka på **Ny vy**.\
   The **Anpassa flexibel vy** visas.

1. I **Anpassa flexibel vy** anger du ett namn för vyn Agile.\
   Vi rekommenderar att du tar med ordet&quot;Agile&quot; i visningsnamnet så att användarna vet att det här är en Agile-vy.\
   Det här namnet visas i dialogrutan **Visa** när du väljer en vy.

1. Definiera de statuskolumner som ska visas på artikelpanelen i den flexibla vyn. Detta är uppgiftsstatusvärdena som definieras av Workfront-administratören, enligt beskrivningen i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Det går bara att använda systemstatus på Agile-artikelpanelen. Om en status endast är tillgänglig för en enskild grupp som du är medlem i, är statusen inte tillgänglig på den flexibla artikelpanelen. Dessutom visas inte uppgifter som har en status som bara är tillgänglig för en anpassad grupp när du visar projektet i en Agile-vy.

   Användarna kan flytta artiklar mellan dessa statuskolumner på Agile-artikelpanelen.\
   När du definierar statuskolumner kan du göra följande:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ändra ordning på statuskolumner:</strong> </td> 
      <td> Dra en statuskolumn till den ordning där du vill att den ska visas.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ta bort statuskolumner:</strong> </td> 
      <td>Klicka på ikonen (x) för den kolumn som du vill ta bort.<br>Du kan inte ta bort statusen"Nytt" om inte en anpassad status har lagts till i vyn och den anpassade statusen är lika med"Nytt".<br>Mer information om hur du skapar en anpassad status finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Skapa eller redigera en status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Lägg till statuskolumner:</strong> </td> 
      <td> <p>Klicka på <strong>Plus</strong> och välj sedan den status som du vill lägga till.<br>Alla standardstatusvärden för systemet visas, liksom alla anpassade statusvärden som har delats med dig.<br>Du kan konfigurera upp till 10 statusar att visa.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. I **Koppla kortfärg till** väljer du bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Artikel:</strong> </td> 
      <td>Alla underaktiviteter matchar färgen för den överordnade uppgiften, så att färgerna för alla artiklar i en viss simbana är desamma.<br>Färger tilldelas slumpmässigt till aktiviteter när de skapas om aktiviteten inte har några underaktiviteter eller inte har någon överordnad aktivitet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fri form:</strong> </td> 
      <td> Alla kort visas som blått som standard tills användaren ändrar färgen manuellt enligt beskrivningen i artikeln <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Kategorisera artiklar efter färg på Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioritet:</strong> </td> 
      <td> <p> Färgerna kopplas till artikelprioriteten enligt följande:</p> 
       <ul> 
        <li>Hög = röd</li> 
        <li>Medel = gul</li> 
        <li>Låg = Grön<br>Om Workfront-administratören har konfigurerat anpassade prioriteringar för ditt Workfront-system är den högsta prioriteten röd, den näst högsta gula och den återstående är grön.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aktivitetsägare:</strong> </td> 
      <td> Alla artiklar med samma primära tilldelade färg har samma färg.<br>Den primära tilldelaren är den användare som först tilldelades uppgiften. </td> 
     </tr> 
    </tbody> 
   </table>

1. I **Agile** i **Ytterligare fält** område, klicka **Lägg till fält** markerar du det fält som du vill lägga till i artikelkort. (Detta är samma fält som du kan lägga till när du skapar en anpassad vy eller skapar kolumner för en rapport.)\
   Upprepa den här processen om du vill lägga till upp till tre ytterligare fält till artikelkorten.\
   När du lägger till fält i artikelkort är fälten skrivskyddade och visas endast när fältet fylls i.

   Som standard visas följande typer av data på artikelkortet:

   * Artikelnamn med en länk direkt till uppgiften
   * Projektnamnet med en länk direkt till projektet\
     Den här länken visas endast när den flexibla vyn används på en iteration. den visas inte när du använder en Agile-vy i ett projekt.
   * Uppgiftsbeskrivningen
   * Aktuellt åtagande
   * Visa och redigera procentandelen antingen genom att justera själva procentandelen eller genom att justera antalet punkter eller timmar som är klara
   * Tilldelade användare

   Du kan visa ytterligare data (inklusive anpassade data) på artikelkort. Du kan visa ytterligare fält på artikelkort av någon anledning. Du kan till exempel visa Kund-ID om du arbetar med artiklar för flera kunder i projektet eller om du vill visa Startdatum för aktiviteten.

1. Klicka **Spara**.\
   Åtkomsten styr hur vyn sparas. Om du skapade vyn från början kan du spara ändringarna; i annat fall uppmanas du att spara en version. Tänk på att de ändringar du gör i vyn påverkar användare som vyn har delats med.

1. (Valfritt) Klicka på **Lista** om du vill återgå till listan med uppgifter.
