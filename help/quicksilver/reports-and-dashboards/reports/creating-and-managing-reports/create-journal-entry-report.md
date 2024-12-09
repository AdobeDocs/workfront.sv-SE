---
title: Rapport om uppdateringsområdet
description: Journalanmälningsrapporten innehåller systemuppdateringar från uppdateringsområdet för projekt, uppgifter, utgåvor och andra objekt som tidigare bara var tillgängliga via Adobe Workfront API. Även om det här är en avancerad rapport som är avsedd för specifika användningsområden, är det lättare för dig att rapportera om projektaktiviteter och systemuppdateringar i Workfront.
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '2737'
ht-degree: 0%

---

# Rapport om uppdateringsområdet

<!-- Audited: 11/2024 -->

Journalanmälningsrapporten innehåller systemuppdateringar från uppdateringsområdet för projekt, uppgifter, utgåvor och andra objekt som tidigare bara var tillgängliga via Adobe Workfront API. Även om det här är en avancerad rapport som är avsedd för specifika användningsområden, är det lättare för dig att rapportera om projektaktiviteter och systemuppdateringar i Workfront.

>[!TIP]
>
>Journalpostrapporten innehåller endast systemuppdateringar från objektens uppdateringsområde. Om du vill rapportera återstående kommentarer i uppdateringsområdet måste du använda anteckningsrapporten.\
>Mer information om anteckningsrapporten finns i [Visa alla uppdateringar i en anteckningsrapport](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md). ‍

Journalanmälningsrapporten kan visa:

* Hur många statusändringar som har gjorts
* När en uppgift eller ett problem har tagits bort
* Hur värden i viktiga anpassade fält ändrades under ett projekts livscykel
* Vilka viktiga datum som har ändrats under ett projekts livscykel
* Om ägaren till ett projekt har ändrats

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
      <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för de objekt som innehåller journalposterna som du visar i rapporten</p> <p>När du har skapat rapporten får du behörigheten Hantera</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du kan utföra de åtgärder som beskrivs i den här artikeln måste du kontrollera följande:

* Alla fält (inklusive anpassade fält) som du vill rapportera om spåras i Workfront. Du kan bara rapportera data från uppdateringsområdet som spåras.

  Mer information om hur du lägger till fält som du vill att Workfront ska spåra finns i [Konfigurera systemuppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

## Översikt över journaltrans.

Eftersom rapporten Journal Entry frågar efter systemuppdateringar kan den returnera ett stort antal resultat. Därför rekommenderar vi att du filtrerar efter specifika objekt - som projekt, program, portföljer, grupper och så vidare - när du skapar rapporten.

Mer information om de olika objekttyperna i Workfront finns i [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Eftersom journalpostrapporten returnerar så mycket data stöds inte export och schemalagd rapportleverans.

Standardvyn för den här rapporten innehåller följande kolumner:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Fält</th> 
   <th>Förklaring</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Fältnamn</strong> </td> 
   <td> <p><span style="font-weight: normal;">Namnet på det påverkade fältet. Beroende på hur du har konfigurerat rapporten kan den här kolumnen innehålla fält för status, ägar-ID, aktivitetsnamn, planerat slutförandedatum eller annat.</span> </p> <p><span style="font-weight: normal;">När </span> <strong>DE</strong>:<span style="font-weight: normal;"> visas i den här kolumnen indikerar det att fältet som visas är ett anpassat fält.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Ändra typ</strong> </td> 
   <td> <p>Den typ av ändring som har gjorts i det påverkade fältet. Beroende på vilka filterregler du har konfigurerat och vilka åtgärder som har vidtagits av användarna kan följande visas i det här fältet:</p> 
    <ul> 
     <li> <p>Lägg till</p> </li> 
     <li> <p>Granskning</p> </li> 
     <li> <p>Ta bort</p> </li> 
     <li> <p>Digest</p> </li> 
     <li> <p>Redigera</p> </li> 
     <li> <p>Återställ</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Övre objektkod</strong> </td> 
   <td> <p>Det högsta överordnade objektet i hierarkin.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Omfång</strong> </td> 
   <td> <p>Den typ av objekt som ändrades.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Anmälningsdatum</strong> </td> 
   <td> <p>Datumet då fältet ändrades.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Redigerad av namn</strong> </td> 
   <td> <p>Användaren som ändrade fältet.</p> </td> 
  </tr> 
 </tbody> 
</table>

Om du vill ordna informationen i den här rapporten kan du använda den inbyggda grupperingen Projekt. Projektgrupperingen ger dig en primär gruppering av projektnamn och en sekundär gruppering av anmälningsdatum. Du kan använda den här befintliga grupperingen när du skapar en rapport eller använda den när du visar rapporten.

Mer information om hur du ställer in vyer, filter och grupperingar för rapporten finns i relevanta avsnitt:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Se vilka statusändringar som har gjorts](#see-what-status-changes-occurred)
* [Se när en uppgift eller ett problem togs bort](#see-when-a-task-or-issue-was-deleted)
* [Se hur anpassade fält ändrades under ett projekts livscykel](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Se hur det planerade slutförandedatumet ändrades under ett projekts livscykel](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Se om ägaren till ett projekt har ändrats](#see-if-the-owner-of-a-project-changed)

## Se vilka statusändringar som har gjorts {#see-what-status-changes-occurred}

Du kan ställa in journalpostrapporten så att den visar:

* Hur många statusändringar som gjorts för ett projekt, en uppgift eller ett ärende

* Tidigare status var före ändringen
* Vem har ändrat status
* När statusändringen ägde rum

Om du vill se ett projekts hälsotillstånd kan du även konfigurera rapporten så att samma information visas med hjälp av projektfältet **Villkor**.

Den här informationen kan användas för att hjälpa till med revision och för att illustrera hur väl du och din organisation planerar.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>Om du vill jämföra skillnaden i dagar mellan villkorsändringar kan du använda Förbättrad analys.\
>Mer information om förbättrade analyser finns i [Översikt över förbättrade analyser](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport** och välj sedan **Journalpost**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report builder läses in.

1. Lägg till följande kolumner på fliken **Kolumner (Visa)**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolumn</th> 
      <th>Förklaring</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Fältnamn</p> </td> 
      <td> <p>Namnet på det påverkade fältet. I det här fallet bör <strong>status</strong> visas i den här kolumnen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ändra typ</p> </td> 
      <td> <p>Den typ av ändring som har gjorts i det påverkade fältet, till exempel <strong>Lägg till</strong>, <strong>Ta bort</strong> eller <strong>Redigera</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Redigerat efter namn</p> </td> 
      <td> <p>Namnet på den användare som uppdaterade statusen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Anmälningsdatum</p> </td> 
      <td> <p>Datumet då statusen ändrades.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Gammalt textvärde</p> </td> 
      <td> <p>Nyckeln för föregående status. Här följer statusnycklarna för standardprojektstatusarna:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: Aktuell</p> </li> 
        <li> <p><strong>DÖD</strong>: Död</p> </li> 
        <li> <p><strong>ONH</strong>: Väntande</p> </li> 
        <li> <p><strong>PLN</strong>: Planering</p> </li> 
        <li> <p><strong>CPL</strong>: Slutförd</p> </li> 
        <li> <p><strong>REQ</strong>: Begärd</p> </li> 
        <li> <p><strong>APR</strong>: Godkänd</p> </li> 
        <li> <p><strong>REJ</strong>: Avvisad</p> </li> 
        <li> <p><strong>IDA</strong>: Idea</p> </li> 
       </ul> <p>Om din organisation har konfigurerat anpassade statusvärden kan andra statusnycklar visas i den här kolumnen. Om du vill veta vilken anpassad status som är relaterad till en statusnyckel kontaktar du Workfront-administratören eller gruppadministratören.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nytt textvärde</p> </td> 
      <td> <p>Nyckeln för den uppdaterade statusen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Övre objektkod</p> </td> 
      <td> <p>Det högsta överordnade objektet för fältet som hade statusändringen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Omfång</p> </td> 
      <td> <p>Den typ av objekt som fick statusändringen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ärendenamn <br> (valfritt)</p> </td> 
      <td> <p>Namnet på utgåvan som hade en statusändring.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Uppgiftsnamn<br> (valfritt)</p> </td> 
      <td> <p>Namnet på den uppgift som hade en statusändring.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Mer information om hur du lägger till kolumner finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicka på **Lägg till en filterregel** på fliken **Filter** och lägg sedan till filterregeln **Fältnamn** > **Lika med** > **status**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Om du vill rapportera om villkorsändringar kan du i stället lägga till filterregeln **Fältnamn** > **Lika med** > **Villkor**.

   Mer information om hur du lägger till filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Valfritt) Lägg till en fråga om du vill begränsa rapportens fokus och minska inläsningstiderna.

   eller

   Skapa ytterligare filterregler för att inkludera specifika projekt, uppgifter eller problem.

   >[!IMPORTANT]
   >
   >Om du skapar en filterregel som använder modifieraren **Innehåller** kan inläsningstiden faktiskt öka. Därför rekommenderar vi att du använder en annan modifierare som **Lika** när det är möjligt för att filtrera efter ett visst projekt eller ett objekt-ID på högre nivå.

   Mer information om hur du lägger till en fråga finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicka på **Använd en befintlig gruppering** på fliken **Grupperingar** och välj sedan **Projekt**.

   Mer information om hur du lägger till grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicka på **Spara + Stäng**.

   Din nya rapport läses in.

## Se när en uppgift eller ett problem har tagits bort {#see-when-a-task-or-issue-was-deleted}

Du kan ställa in journalpostrapporten så att den visar:

* Vilka uppgifter eller problem som har tagits bort
* Vem tog bort en uppgift eller ett problem

Så här ser du när en uppgift eller ett problem togs bort:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport** och välj sedan **Journalpost**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report builder läses in.

1. Lägg till följande kolumner på fliken **Kolumner (Visa)**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolumn</th> 
      <th>Förklaring</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Omfång</p> </td> 
      <td> <p>Den typ av objekt som togs bort.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ändra typ</p> </td> 
      <td> <p>Den typ av ändring som inträffade. Ändringen <strong>Ta bort</strong> visas i den här kolumnen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Anmälningsdatum</p> </td> 
      <td> <p>Datumet då uppgiften eller utgåvan togs bort.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Redigerat efter namn</p> </td> 
      <td> <p>Namnet på den användare som tog bort uppgiften eller utgåvan.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektnamn</p> </td> 
      <td> <p>Namnet på det projekt där uppgifter eller utgåvor togs bort.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Mer information om hur du lägger till kolumner finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicka på **Lägg till filterregel** på fliken **Filter** och lägg sedan till följande filter:

   * **Ändra typ** > **Lika med** > **Ta bort**
   * **Projekt-ID** > **Lika med** > **&lt; projektnamn >**

     <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Mer information om hur du lägger till filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Valfritt) Lägg till en fråga om du vill begränsa rapportens fokus och minska inläsningstiderna.

   eller

   Skapa ytterligare filterregler för att inkludera specifika projekt, uppgifter eller problem.

   >[!IMPORTANT]
   >
   >Om du skapar en filterregel som använder modifieraren **Innehåller** kan inläsningstiden faktiskt öka. Därför rekommenderar vi att du använder en annan modifierare som **Lika** när det är möjligt för att filtrera efter ett visst projekt eller ett objekt-ID på högre nivå.

   Mer information om hur du lägger till en fråga finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Valfritt) Klicka på **Använd en befintlig gruppering** på fliken **Grupperingar** och välj sedan **Projekt**.

   Mer information om hur du lägger till grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicka på **Spara + Stäng**.

   Din nya rapport läses in.

## Se hur anpassade fält ändrades under ett projekts livscykel {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Du kan spåra viktiga fältändringar under projektets gång. Du kan ställa in journalposten så att den spårar:

* Om vissa anpassade fält lades till, uppdaterades eller redigerades
* När dessa ändringar gjordes
* Vem gjorde ändringarna

Så här ser du hur anpassade fält har ändrats under ett projekts livscykel:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport** och välj sedan **Journalpost**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report builder läses in.

1. Se till att du har gjort det på fliken **Kolumner (Visa)** eller klicka på **Lägg till kolumn** för att lägga till följande kolumner:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolumn</th> 
      <th>Förklaring</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Fältnamn</p> </td> 
      <td> <p>Namnet på det anpassade fältet som påverkas.</p> <p><span style="font-weight: normal;">När </span> <strong>DE</strong>:<span style="font-weight: normal;"> visas i den här kolumnen indikerar det att fältet som visas är ett anpassat fält.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ändra typ</p> </td> 
      <td> <p>Den typ av ändring som har gjorts i det påverkade fältet, till exempel <strong>Lägg till</strong>, <strong>Ta bort</strong> eller <strong>Redigera</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Redigerat efter namn</p> </td> 
      <td> <p>Namnet på den användare som uppdaterade det anpassade fältet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Anmälningsdatum</p> </td> 
      <td> <p>Det datum då värdet i det anpassade fältet ändrades.</p> <p>Du bör sortera efter det här fältet i fallande ordning.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Gammalt nummervärde</p> </td> 
      <td> <p>Det föregående talvärdet i det anpassade fältet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nytt nummervärde</p> </td> 
      <td> <p>Det aktuella nummervärdet i det anpassade fältet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tidigare datumvärde</p> </td> 
      <td> <p>Föregående datumvärde i det anpassade fältet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nytt datumvärde</p> </td> 
      <td> <p>Det aktuella datumvärdet i det anpassade fältet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Gammalt textvärde</p> </td> 
      <td> <p>Det tidigare textvärdet i det anpassade fältet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nytt textvärde</p> </td> 
      <td> <p>Det aktuella textvärdet i det anpassade fältet.</p> <p>Om det anpassade fältet är ett typsnittsfält visas objekt-ID:t i kolumnen <strong>Nytt textvärde</strong> .</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Mer information om hur du lägger till kolumner finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicka på **Lägg till en filterregel** på fliken **Filter** och lägg sedan till följande filter:

   * **Fältnamn för journalpost** > **Innehåller** > **DE**

     >[!TIP]
     >
     >Om du vill begränsa den här rapporten till specifika anpassade fält lägger du till filterregeln **Fältnamn för journalpost** > **Lika med** > **&lt; namn på anpassat fält>**.

   * **Projekt-ID** > **Lika med** > **&lt; projekt >**.

   ![](assets/qs-custom-form-changes-filter-350x92.png)

   Mer information om hur du lägger till filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Valfritt) Lägg till en fråga om du vill begränsa rapportens fokus och minska inläsningstiderna.

   eller

   Skapa ytterligare filterregler för att inkludera specifika projekt, uppgifter eller problem.

   >[!IMPORTANT]
   >
   >Om du skapar en filterregel som använder modifieraren **Innehåller** kan inläsningstiden faktiskt öka. Därför rekommenderar vi att du använder en annan modifierare som **Lika** när det är möjligt för att filtrera efter ett visst projekt eller ett objekt-ID på högre nivå.

   Mer information om hur du lägger till en fråga finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicka på **Använd en befintlig gruppering** på fliken **Grupperingar** och välj sedan **Projekt**.

   Mer information om hur du lägger till grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicka på **Spara + Stäng**.

   Din nya rapport läses in.

## Se hur det planerade slutförandedatumet ändrades under ett projekts livscykel {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Du kan ställa in journalanmälningsrapporten för att visa hur ofta det planerade slutförandedatumet ändras under ett projekts livstid.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport** och välj sedan **Journalpost**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report builder läses in.

1. Lägg till följande kolumner på fliken **Kolumner (Visa)**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolumn</th> 
      <th>Förklaring</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Fältnamn</p> </td> 
      <td> <p>Namnet på det påverkade fältet.</p> <p><span style="font-weight: normal;">När </span> <strong>DE</strong>:<span style="font-weight: normal;"> visas i den här kolumnen indikerar det att fältet som visas är ett anpassat fält.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ändra typ</p> </td> 
      <td>Den typ av ändring som inträffade, till exempel <strong>Lägg till</strong>, <strong>Ta bort</strong> eller <strong>Redigera</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Redigerat efter namn</p> </td> 
      <td> <p>Namnet på den användare som uppdaterade projektets planerade slutförandedatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Anmälningsdatum</p> </td> 
      <td> <p>Datumet då projektets planerade slutförandedatum ändrades.</p> <p>Du bör sortera efter det här fältet i fallande ordning.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Övre objektkod</p> </td> 
      <td> <p>Det högsta överordnade objektet för det fält som hade ändrat planerat slutförandedatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Omfång</p> </td> 
      <td> <p>Det objekt som hade det planerade slutförandedatumet ändrat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Tidigare datumvärde</p> </td> 
      <td> <p>Föregående värde för planerat slutförandedatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nytt datumvärde</p> </td> 
      <td> <p>Det aktuella värdet för planerat slutförandedatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektnamn</p> <p>(Valfritt)</p> </td> 
      <td> <p>Namnet på det projekt där det planerade slutförandedatumet ändrades.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Aktivitetsnamn</p> <p>(Valfritt)</p> </td> 
      <td> <p>Namnet på aktiviteterna i projektet som hade det planerade slutförandedatumet ändrat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ärendenamn</p> <p>(Valfritt)</p> </td> 
      <td>Namnet på de utgåvor i projektet som har den planerade ändringen av slutförandedatum.</td> 
     </tr> 
    </tbody> 
   </table>

   Mer information om hur du lägger till kolumner finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicka på **Lägg till en filterregel** på fliken **Filter** och lägg sedan till följande:

   * **Fältnamn** > **Lika med** > **Datum**
   * **Projekt-ID** > **Lika med** > **&lt; projektnamn >**.

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   Mer information om hur du lägger till filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Valfritt) Lägg till en fråga om du vill begränsa rapportens fokus och minska inläsningstiderna.

   eller

   Skapa ytterligare filterregler för att inkludera specifika projekt, uppgifter eller problem.

   >[!IMPORTANT]
   >
   >Om du skapar en filterregel som använder modifieraren **Innehåller** kan inläsningstiden faktiskt öka. Därför rekommenderar vi att du använder en annan modifierare som **Lika** när det är möjligt för att filtrera efter ett visst projekt eller ett objekt-ID på högre nivå.

   Mer information om hur du lägger till en fråga finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicka på **Använd en befintlig gruppering** på fliken **Grupperingar** och välj sedan **Projekt**.

   Mer information om hur du lägger till grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicka på **Spara + Stäng**.

   Din nya rapport läses in.

## Se om ägaren till ett projekt har ändrats {#see-if-the-owner-of-a-project-changed}

Du kan ställa in journalanmälningsrapporten för att visa hur många gånger projektägaren, eller projektledaren, ändras under ett projekts livslängd.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport** och välj sedan **Journalpost**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report builder läses in.

1. Lägg till följande kolumner på fliken **Kolumner (Visa)**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolumn</th> 
      <th>Förklaring</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Fältnamn</p> </td> 
      <td>Namnet på det påverkade fältet. <strong>ownerID</strong> visas i den här kolumnen.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ändra typ</p> </td> 
      <td> <p>Den typ av ändring som inträffade, till exempel <strong>Lägg till</strong>, <strong>Ta bort</strong> eller <strong>Redigera</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Övre objektkod</p> </td> 
      <td> <p>Det högsta överordnade objektet för det projekt som projektägaren uppdaterades för.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Anmälningsdatum</p> </td> 
      <td>Datumet då projektägaren ändrades.<br>Du bör sortera efter det här fältet i fallande ordning.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Redigerat efter namn</p> </td> 
      <td> <p>Namnet på den användare som uppdaterade projektägaren.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ytterligare information 1</p> </td> 
      <td> <p>Projektets nuvarande ägare.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ytterligare info 2</p> </td> 
      <td> <p>Den tidigare projektägaren för projektet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektnamn</p> </td> 
      <td> <p>Projektet där fältet Projektägare uppdaterades.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Mer information om hur du lägger till kolumner finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicka på **Lägg till filterregel** på fliken **Filter** och lägg sedan till följande:

   * **Fältnamn** > **Lika med** > **ownerID**
   * **Projekt-ID** > **Lika med** > **&lt; projektnamn >**.

   ![](assets/qs-owner-changes-filter-350x94.png)

   Mer information om hur du lägger till filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Valfritt) Lägg till en fråga om du vill begränsa rapportens fokus och minska inläsningstiderna.

   eller

   Skapa ytterligare filterregler för att inkludera specifika projekt, uppgifter eller problem.

   >[!IMPORTANT]
   >
   >Om du skapar en filterregel som använder modifieraren **Innehåller** kan inläsningstiden faktiskt öka. Därför rekommenderar vi att du använder en annan modifierare som **Lika** när det är möjligt för att filtrera efter ett visst projekt eller ett objekt-ID på högre nivå.

   Mer information om hur du lägger till en fråga finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Valfritt) Klicka på **Använd en befintlig gruppering** på fliken **Grupperingar** och välj sedan **Projekt**.

   Mer information om hur du lägger till grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicka på **Spara + Stäng**.

   Den nya journalpostrapporten visas.
