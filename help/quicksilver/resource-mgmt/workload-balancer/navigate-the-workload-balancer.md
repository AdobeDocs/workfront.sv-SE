---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Navigera till arbetsbelastningsutjämnaren
description: Använd belastningsutjämnaren för att förstå tillgängligheten för dina resurser och för att tilldela arbete till dina användare. I den här artikeln får du hjälp med att använda de ikoner och inställningar som är tillgängliga för att uppdatera vyn för och navigera i arbetsbelastningsutjämnaren.
author: Lisa
feature: Resource Management
exl-id: 60dabfc5-6a2e-4368-9dac-db48d0307895
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '4348'
ht-degree: 0%

---

# Navigera till arbetsbelastningsutjämnaren

{{preview-fast-release-general}}

<!--Audited: 12/2024-->

Använd Utjämning av arbetsbelastning i Adobe Workfront för att tilldela användare arbete baserat på deras tillgänglighet. I den här artikeln beskrivs hur du kan använda inställningar och alternativ för att navigera i arbetsbelastningsutjämnaren och visa den information som är relevant för dig. Ytterligare artiklar som visas här beskriver hur du kan använda belastningsutjämnaren för att hantera dina resurser och deras allokering till arbete.

Utjämning av arbetsbelastning är tillgängligt i flera områden av Adobe Workfront. Att navigera är detsamma i alla områden.

Mer information om var arbetsbelastningsutjämnaren finns finns i [Hitta arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/manage-resources/the-workload-balancer/locate-workload-balancer).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Planera, när du använder belastningsutjämnaren för arbetsbelastning i resursområdet; Arbeta när du använder belastningsutjämnaren för ett team eller projekt</p></td>
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomsten till följande:</p> 
    <ul> 
     <li>Resurshantering</li> 
     <li>Projekt</li> 
     <li>Uppgifter</li> 
     <li>Problem</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Visa eller högre behörigheter för projekt, uppgifter och ärenden</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du visar objekt i arbetsbelastningsutjämnaren

Tänk på följande när du visar arbetsbelastningsutjämnaren:

* Utjämning av arbetsbelastning visar arbetsobjekt i två olika områden, beroende på deras uppdrag. Arbetsobjekt och användare visas i följande områden:

   * **Ej tilldelat arbete**: Objekt som inte har några tilldelningar eller bara är tilldelade till jobbroller eller team.
   * **Tilldelat arbete**: Objekt som har tilldelats minst en användare. De tilldelade objekten visas under den tilldelade användarens namn.

  >[!NOTE]
  >
  >* Arbetsobjekt som tilldelats en jobbroll eller ett team, och som även tilldelats en användare, visas både i området Ej tilldelat arbete och under den tilldelade användarens namn i området Tilldelat arbete.
  >* Arbetsobjekt som har tilldelats en användare och en jobbroll, där jobbrollen har valts som primär tilldelare för artikeln, visas i området Ej tilldelat arbete.
  >* Arbetsobjekt som tilldelats till mer än en användare visas under alla de tilldelade användarnas namn på området Tilldelat arbete.
  >* <span class="preview">Rolltilldelningar visas under arbetsobjekt i området Ej tilldelat arbete när inställningen Visa rolltilldelningar är aktiverad. Mer information finns i avsnittet [Anpassa vyn](#customize-the-view) i den här artikeln.</span>

  Mer information finns i [Uppdragsområden i Arbetsbelastningsutjämnaren](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md#assignment-areas-in-the-workload-balancer) i [Översikt över tilldelning av arbete i belastningsutjämnaren](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

* När ett projekt inte har några uppgifter under en tidsperiod är fältet på projektnivån tomt för den tiden.

  ![Projekt utan aktiviteter under en tidsperiod](assets/wb-no-tasks-in-time-period.png)

* Om du inte har behörighet att visa vissa objekt visas de som **Otillgängliga arbetsobjekt** eller **Otillgängliga projekt**.

  ![Otillgängliga arbetsobjekt](assets/wb-inaccessible-work-items.png)

* Namnen på arbetsobjekten visas till vänster och deras tidslinje visas till höger.
* Det totala antalet planerade timmar för varje arbetsuppgift visas till höger om arbetsobjektets namn och till vänster om fältet som representerar arbetsobjektets tidslinje.
* Det totala antalet planerade timmar för varje projekt visas till höger om namnet på projektet och till vänster om fältet som representerar projektets tidslinje.

  Information om planerade timmar för projektet är det totala antalet planerade timmar för alla objekt som listas i Utjämning av arbetsbelastning, och inte det totala antalet planerade timmar för projektet.

Mer information om hur du visar information i Arbetsbelastningsutjämnaren finns i följande artiklar:

* [Leta reda på arbetsbelastningsutjämnaren](../workload-balancer/locate-workload-balancer.md)
* [Filtrera information i Utjämning av arbetsbelastning](../workload-balancer/filter-information-workload-balancer.md)
* [Dela arbetsbelastningsutjämnaren med en länk](../workload-balancer/share-link-for-workload-balancer.md)
* [Uppdatera arbetsobjekt i belastningsutjämnaren med hjälp av sammanfattningen](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

Mer information om hur du hanterar resurser med hjälp av belastningsutjämnaren finns i följande artiklar:

* [Översikt över tilldelning av arbete i arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/manage-resources/the-workload-balancer/assign-work-in-workload-balancer)
* [Hantera användarallokeringar i arbetsbelastningsutjämnaren](https://experienceleague.adobe.com/sv/docs/workfront/using/manage-resources/the-workload-balancer/manage-user-allocations-workload-balancer)


## Navigera i Utjämning av arbetsbelastning för flera projekt i resursområdet

Att navigera i belastningsutjämnaren är detsamma i alla områden där du kommer åt den.

I följande underavsnitt beskrivs hur du visar informationen i Utjämning av arbetsbelastning för flera projekt.

Du kan justera ett antal inställningar och alternativ i Utjämning av arbetsbelastning för att visa den information du behöver fokusera på i den tidsram som passar dig bäst.

När du har valt de inställningar som du vill använda för vyn kommer arbetsbelastningsutjämnaren ihåg dessa inställningar varje gång du öppnar den från en webbläsare eller enhet.

### Få åtkomst till belastningsutjämnaren för flera projekt i resursområdet

Så här navigerar du i belastningsutjämnaren för flera projekt:

{{step1-to-resourcing}}

1. Klicka på **Utjämning av arbetsbelastning** i den vänstra panelen.

   ![Utjämnare för arbetsbelastning](assets/nwe-balancer-global.png)

   I Utjämning av arbetsbelastning visas information om arbetstilldelning som börjar med den aktuella veckan i följande två områden:

   * Området **Ej tilldelat arbete** visar följande arbetsobjekt:

      * Arbetsobjekt (uppgifter och ärenden) som tilldelats roller, team eller som inte har tilldelats visas när du har tillämpat filter.
Arbetsytan Ej tilldelat visas inte som standard. Vi rekommenderar att du använder filter för att visa relevant information för dig i det här området.

        Mer information om hur du använder filter finns i [Filterinformation i Arbetsbelastningsutjämnaren](../workload-balancer/filter-information-workload-balancer.md).

      * <span class="preview">Rolltilldelningar under arbetsobjekt visas bara när du aktiverar inställningen Visa rolltilldelningar. Mer information finns i avsnittet [Anpassa vyn](#customize-the-view) i den här artikeln.</span>

      * Projekt visas bara när du aktiverar inställningen Grupp efter projekt. Mer information finns i avsnittet [Anpassa vyn](#customize-the-view) i den här artikeln.

   * Under **Tilldelad arbetsuppgift** visas följande arbetsobjekt:

      * Alla aktiva användare i systemet visas som standard i det här området. Vi rekommenderar att du använder filter för att begränsa mängden information i det här området. Om användare tilldelas till objekt visas även arbetsobjekten under deras namn.

      * Uppgifter och ärenden som tilldelats minst en användare visas under användarens namn.

        Arbetsobjekten under användarens namn i området Tilldelat arbete sorteras efter följande villkor, i den här ordningen:

         1. Planerat startdatum (äldsta först)
         1. Planerat slutförandedatum (äldsta först)
         1. Alfabetiskt efter projekt (endast när de första två kriterierna är identiska för flera arbetsobjekt)

            >[!TIP]
            >
            >* Du kan anpassa projektsorteringen genom att välja ett alternativ i inställningen Sortera projekt efter.
            >
            >* Projekt visas bara när du aktiverar inställningen &quot;Grupp efter projekt&quot;.
            > 
            >Mer information om hur du anpassar inställningar finns i avsnittet [Anpassa vyn](#customize-the-view) i den här artikeln.

1. (Valfritt) Klicka på ikonen **Filter** ![Filter &#x200B;](assets/filter-icon.png) i området **Tilldelat arbete** och välj sedan **Standardfilter** i området **Förslag** i filterrutan.

   När du använder standardfiltret visas användare som tillhör något av dina team och deras arbetsobjekt. Du kan redigera en kopia av det här filtret.

   >[!TIP]
   >
   >Standardfiltret är bara tillgängligt i Utjämning av arbetsbelastning i området Resurser.

1. Fortsätt med följande steg för att navigera i arbetsbelastningsutjämnaren:

   * [Välj en tidsram i Utjämning av arbetsbelastning](#select-a-time-frame-in-the-workload-balancer)
   * [Anpassa vyn](#customize-the-view)
   * [Tilldela arbetsobjekt och justera användarallokeringar](#assign-work-items-and-adjust-user-allocations)
   * [Visa allokeringar i ett diagram](#view-allocations-in-a-chart)

### Välj en tidsram i Utjämning av arbetsbelastning

1. Få åtkomst till belastningsutjämnaren för arbetsbelastning i området **Resurs**, enligt beskrivningen i avsnittet [Få åtkomst till belastningsutjämnaren för flera projekt i området Resurser](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.

   Utjämning av arbetsbelastning visar information om arbetstilldelning som börjar med den aktuella veckan.

1. Använd den vågräta rullningen för att visa tidslinjen för arbetsobjekt som sträcker sig utanför skärmens gränser.
1. Klicka på ikonerna **Bakåt eller framåt** ![Ikonerna Bakåt och framåt](assets/back-and-forward-icons.png) i det övre vänstra hörnet för att navigera i tidslinjen och klicka sedan på **Idag** för att återgå till den aktuella veckan.
1. Klicka på listrutan **Tidsram** i verktygsfältet och klicka sedan på startdatumet för den period som du vill visa. Som standard är den första veckan som du väljer i kalendern den vecka som du har navigerat till.

   ![Kalenderval](assets/calendar-date-picker-wb.png)

1. Välj det antal veckor som du vill visa samtidigt i Utjämning av arbetsbelastning bland följande alternativ:
   * 1 vecka
   * 2 veckor
   * 4 veckor. Det här är standardinställningen.
   * 6 veckor
   * 3 månader

   ![Välj veckor](assets/3-months-12-weeks-drop-down-wb.png)

1. Klicka på något av följande alternativ i verktygsfältet för att visa information i olika tidsramar:
   * **Dag**: Visar information per dag i fyra veckor med början från dagens datum, som standard.
   * **Vecka**: Visar information per vecka i fyra veckor.
   * **Månad**: Visar information per månad i tre månader.

1. Fortsätt navigera i arbetsbelastningsutjämnaren enligt beskrivningen i följande avsnitt.

### Anpassa vyn

1. Få åtkomst till belastningsutjämnaren för arbetsbelastning i området **Resurs**, enligt beskrivningen i avsnittet [Få åtkomst till belastningsutjämnaren för flera projekt i området Resurser](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.

   Namnen på arbetsobjekten listas till vänster och representeras av fält till höger om Arbetsbelastningsutjämnaren. Längden på fältet representerar tidslinjen för ett arbetsobjekt.

1. (Valfritt och rekommenderat) Använd filter i områdena Ej tilldelat och Tilldelat arbete för att endast visa arbetsuppgifter eller användare som är relevanta för dig.

   Mer information finns i [Filtrera information i Utjämning av arbetsbelastning](../workload-balancer/filter-information-workload-balancer.md).

   Som standard representerar blå staplar tidslinjerna för projekt och uppgifter och marmelinerna problem.

   Du kan ändra färg på staplarna för projekt och uppgifter när du väljer ett färgtema som matchar projektet. Mer information finns i den här proceduren.

   Arbetsobjekten i den tilldelade arbetsytan sorteras efter projekt enligt följande kriterier, i den här ordningen:
   1. Planerat startdatum (äldsta först)
   1. Planerat slutförandedatum (äldsta först)
   1. Alfabetiskt efter projekt (endast när de första två kriterierna är identiska för flera arbetsobjekt)

1. Klicka på den **högerriktade pilen** till vänster om områdena Ej tilldelat eller Tilldelad om du vill expandera alla objekt under projektnamnen (i området Ej tilldelat) och under användarnamnen (i området Tilldelad).

   >[!TIP]
   >
   >Arbetsobjekt visas under projektnamn i området Ej tilldelat när du aktiverar inställningen Gruppera efter projekt.

1. Klicka på den **nedåtriktade pilen** till vänster om området Ej tilldelat eller Tilldelad om du vill komprimera alla objekt under projektnamnen (i området Ej tilldelat) och under användarnamnen (i området Tilldelad).

1. Håll pekaren över och dra och släpp **separationslinjen** mellan den vänstra panelen och tidslinjeområdet för att justera storleken på den vänstra panelen.

   ![Separationslinje](assets/wb-adjust-panel-size.png)

1. Klicka på ikonen **Inställningar** ![Inställningar](assets/settings-gear-icon.png) .

   Panelen Inställningar visas till höger.

   <span class="preview">Exempelbild i förhandsvisningsmiljön:</span>
   ![Panelen Inställningar för belastningsutjämnare](assets/workload-balancer-settings.png)

   Exempelbild i produktionsmiljön:
   ![Panelen Inställningar](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Välj bland alternativen nedan för att uppdatera informationen som du visar i Utjämning av arbetsbelastning och klicka sedan på ikonen **X** i det övre högra hörnet av inställningsrutan för att stänga den.

   * **Gruppera efter projekt**: När det här alternativet har valts grupperas objekten i områdena Ej tilldelat och Tilldelat arbete efter projekt. Detta är markerat som standard.

   * **Inkludera timmar från utgåvor**: När detta är markerat visas utgåvor som tilldelats användare under användarens namn i området Tilldelad arbetsyta och utgåvor som inte har tilldelats användare visas i området Ej tilldelad arbetsyta. De planerade timmarna från problemen räknas mot de planerade timmarna för projektet och för användaren i området Tilldelad arbetstid.
   * **Visa beräknade datum**: När detta väljs visas den projicerade tidslinjen för arbetsobjekt utöver den planerade tidslinjen. Observera följande:
      * Den planerade tidslinjen för projekt, uppgifter och utgåvor visas som en mörkblå linje ovanför aktivitetsfältet, utgåvan och projektfälten.
      * Den projicerade tidslinjen som ligger utanför den planerade tidslinjen visas i ljusblått, även när du uppdaterar färgtemat enligt beskrivningen nedan.
      * Den projicerade tidslinjen för de objekt som du inte har tillgång till visas i ljusgrått med en linje under.
      * När en aktivitet eller ett problem har slutförts före det förfallna datumet för planerad slutförande, slås allokeringsnumren för de återstående dagarna igenom och räknas inte av mot användarens allokering. Detta visas bara när både inställningen Visa beräknade datum och ikonen Visa allokering är aktiverad.

     >[!TIP]
     >
     >Observera att arbetsobjekt visas i Utjämning av arbetsbelastning när antingen deras planerade eller planerade tidslinjer (inte nödvändigtvis båda samtidigt) inträffar under den valda tidsramen.

   * **Visa slutfört arbete**: När det här alternativet är aktiverat visas slutförda uppgifter och utgåvor på den tilldelade arbetsytan. Detta är aktiverat som standard.

     En grön bockmarkeringsikon visas i det övre högra hörnet av en uppgift eller ett problemfält när de är klara. Samma ikon visas för ett projekt när aktiviteterna eller utgåvorna för den valda tidsramen i projektet har slutförts.
   * **Visa återstående tid**: När detta är aktiverat visar Workfront skillnaden mellan den dagliga tid som användaren är tillgänglig för arbete baserat på sina scheman och de timmar som användaren är tilldelad till i arbetsytan Tilldelad arbetstid för användarna. Detta är inaktiverat som standard och den tilldelade tiden visas som standard.
   * <span class="preview">**Visa rolltilldelningar**: När detta är aktiverat visas rolltilldelningar i arbetsytan Ej tilldelat under deras tilldelade arbetsobjekt. Detta är aktiverat som standard.</span>

   * I avsnittet **Välj färgtema** väljer du den färg du vill använda för projekt- och aktivitetsfälten.

     >[!TIP]
     >
     >Inställningen för att välja färgtema påverkar inte färgen på problemfälten. Problem visas alltid i ett fält med maronfärg.

     Välj bland följande:
      * **Standard**: Fälten för alla projekt och deras arbetsobjekt visas i blått.
      * **Projekt**: Fälten som är associerade med varje projekt och dess aktiviteter ändras beroende på projektets namn. Alla uppgifter som tillhör projektet visas i fält som matchar projektets färg. Projektstaplarna visas i en ljusare ton för att skilja dem från åtgärderna. Projektfälten innehåller också en projektikon när du väljer att inte visa tilldelningar.
      * **Projektstatus**: Fälten som är associerade med varje projekt och dess arbetsobjekt ändras till färgen för projektets status.

        Projektstatusen är den som är associerad med projektgruppen. Om gruppen inte har gruppspecifika statusar är färgen på arbetsartikelfälten densamma som på projektstatus på systemnivå. Både systemet och anpassade statusar visas. Mer information om gruppstatus finns i [Skapa eller redigera en gruppstatus](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

   * I avsnittet **Visa användartilldelning i** väljer du bland följande:
      * **Timmar**: Visar tilldelad tid som timmar. Det här är standardinställningen.
      * **Procent**: Visar tilldelad tid i procent av den totala tillgängliga tiden
   * I avsnittet **Sorteringsinställningar** väljer du hur du vill att objekten ska sorteras i arbetsbelastningsutjämnaren. Välj bland följande alternativ:
      * **Sortera användare efter primär roll**: Användare visas i alfabetisk ordning efter sina primära roller i området Tilldelad arbetsyta.
      * **Sortera användare i alfabetisk ordning**: Användare visas i alfabetisk ordning efter förnamn på arbetsytan Tilldelad.
      * **Sortera projekt efter**: Välj ett projektfält i listrutan om du vill sortera projekt i bokstavsordning efter fältet i områdena Ej tilldelat eller Tilldelat arbete.

   >[!TIP]
   >
   >Du kan bara sortera efter projekt när inställningen Gruppera efter projekt är aktiverad. I annat fall är den här inställningen nedtonad.

1. (Valfritt och villkorligt) När du ändrar färgtemat till Projektstatus håller du markören över namnet på ett projekt till vänster för att visa projektets status.

   ![Verktygstips för projektstatus](assets/hover-over-project-status-tooltip-350x115.png)

### Tilldela arbetsobjekt och justera användarallokeringar

1. Gå till Utjämning av arbetsbelastning i området Resurser, vilket beskrivs i avsnittet [Öppna Utjämning av arbetsbelastning för flera projekt i området Resurser](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.
1. Klicka på ikonen **Visa tilldelningar** ![Visa tilldelningsikonen](assets/show-allocations-icon-small.png) om du vill visa planerade timmar per dag eller vecka för arbetsobjekt.

   Detta ersätter namnet i fälten för arbetsobjekten med antalet planerade timmar per dag eller vecka i områdena Ej tilldelat och Tilldelat arbete. Den här inställningen är inaktiverad som standard.

   Dagar som visar överbeläggningar visas i rött.

   >[!TIP]
   >
   >* Alternativet Visa allokeringar påverkar bara vad som visas för projekt, uppgifter, utgåvor och objekt som inte är tillgängliga. Dagliga planerade timmar för användare visas som standard och kan inte döljas.
   >* Du måste aktivera inställningen Gruppera efter projekt för att visa dagliga planerade timmar för projekt.
   >* När du visar Utjämning av arbetsbelastning per vecka visas antalet timmar per vecka som planerats.

1. (Valfritt) Hovra över den tilldelade tiden på användarraden för att förstå användarens kapacitet och allokering. Kapaciteten är användarens tillgänglighet enligt schema.

   ![Information om tilldelad tid](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Valfritt) Klicka på ikonen **Dölj tilldelningar** ![Visa tilldelningsikonen](assets/show-allocations-icon-small.png) för att visa namnet på aktiviteterna och utgåvorna i fälten för arbetsobjekten.
1. Klicka på ikonen **Mer meny** ![Mer ikon](assets/more-icon.png) till höger om namnet på en aktivitet, ett problem, ett <span class="preview">eller en roll</span> och klicka sedan på något av alternativen nedan.

   ![Mer-menyn](assets/more-menu-right-of-task-350x104.png)

   * **Tilldela det här till** och börja sedan skriva namnet på en användare, roll eller team som du vill tilldela arbetsobjektet till i fältet **Sök efter personer, roller eller team**.

     Klicka på **Avancerat** för att komma åt skärmen Avancerade tilldelningar för arbetsobjektet. Mer information finns i [Skapa avancerade uppdrag](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     Du kan även använda följande kortkommandon för att tilldela uppgifter eller ärenden:

      * I Windows: CTRL-klicka på aktivitets- eller problemfältet.
      * I Mac: CMD-klicka på aktivitets- eller problemfältet.

     Mer information om hur du tilldelar arbetsobjekt till användare i belastningsutjämnaren finns i [Översikt över hur du tilldelar arbete i belastningsutjämnaren](../workload-balancer/assign-work-in-workload-balancer.md).

     >[!NOTE]
     >
     ><span class="preview">Rolltilldelningar visas bara under arbetsobjekt i området Ej tilldelat arbete när inställningen Visa rolltilldelningar är aktiverad. Mer information finns i avsnittet [Anpassa vyn](#customize-the-view) i den här artikeln. Rolltilldelningar har bara alternativet **Tilldela detta till** på menyn **Mer**.</span>

     >[!TIP]
     >
     >Om din Workfront- eller gruppadministratör har aktiverat delegeringar i din miljö använder du fliken Uppdrag för att tilldela användare till uppgiften eller problemet. Mer information om hur du delegerar arbete finns i [Delegera uppgifter och problem](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Redigera allokeringar** och redigera sedan dagliga eller veckovisa allokeringar för användaren. Mer information om hur du hanterar användartilldelningar finns i [Hantera användartilldelningar i Utjämning av arbetsbelastning](../workload-balancer/manage-user-allocations-workload-balancer.md).

   * **Öppna sammanfattning**. Panelen Sammanfattning öppnas till höger, klicka sedan på fältet Uppdrag och börja skriva namnet på en användare, roll eller team i fältet **Sök efter personer, roller eller team** för att tilldela objektet. Mer information finns i avsnittet [Visa mer information om aktiviteter och problem](#display-more-information-about-tasks-and-issues) i den här artikeln.

1. (Valfritt) Dubbelklicka på en daglig eller veckovis tilldelning för en användare i fältet för en arbetsuppgift om du vill redigera antalet allokerade timmar. Klicka sedan på ikonen **Spara** ![Spara](assets/save-allocations-wb.png) om du vill spara allokeringarna eller på ikonen **Avbryt** ![Avbryt](assets/cancel-allocations-wb.png) om du vill ta bort de allokeringar du justerat.

   >[!TIP]
   >
   >Ikonerna Spara och Avbryt visas mot slutet av en uppgift eller ett ärende tidslinjefält.
   >
   >![Spara eller avbryt manuella allokeringar](assets/cancel-and-save-icon-on-adjust-allocation-bar-wb-highlighted.png)

   Mer information om hur du hanterar användartilldelningar finns i [Hantera användartilldelningar i Utjämning av arbetsbelastning](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Klicka på **Gruppera tilldelningar** om du vill tilldela flera arbetsobjekt samtidigt.

   Mer information finns i [Tilldela flera arbeten samtidigt med hjälp av arbetsbelastningsutjämnaren](../workload-balancer/assign-work-in-workload-balancer-in-bulk.md).
1. Dra objekt från området **Ej tilldelat arbete** eller från en användare och släpp dem på en annan användare för att tilldela dem.

   Mer information finns i [Tilldela arbete i Utjämning av arbetsbelastning genom att dra och släppa](../workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

### Visa allokeringar i ett diagram

I stället för att visa tilldelningar i dag- eller veckonummer kan du visa dem i ett diagram.

1. Gå till Utjämning av arbetsbelastning i området Resurser, vilket beskrivs i avsnittet [Öppna Utjämning av arbetsbelastning för flera projekt i området Resurser](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.
1. Klicka på ikonen **Diagram** ![Diagram](assets/user-allocation-chart-icon.png) för att visa användartilldelningen i ett diagramformat.

   Dagar där användaren är överallokerad visas som röda block och dagar där användaren är underallokerad eller vid kapacitet visas som blå block.

   Storleken på blocken anger mängden allokering: ju större ruta, desto mer tid tilldelas användaren till arbetsuppgifter för den dagen eller veckan.

   ![Användartilldelning som diagram](assets/wb-allocation-as-chart.png)

### Visa mer information om uppgifter och problem

Du kan visa mer information om aktiviteterna och problemen i Utjämning av arbetsbelastning.

1. Gå till Utjämning av arbetsbelastning i området Resurser, vilket beskrivs i avsnittet [Öppna Utjämning av arbetsbelastning för flera projekt i området Resurser](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.
1. Om du vill visa mer information på panelen Sammanfattning gör du något av följande:

   * Klicka på fältet för en uppgift eller ett problem för att öppna sammanfattningspanelen till höger.
   * Klicka på ikonen **Öppna sammanfattning** ![Öppna sammanfattning](assets/summary-panel-icon.png) och klicka sedan på fältet för en uppgift eller ett problem för att öppna panelen Sammanfattning.
   * Klicka på menyn **Mer** till höger om en uppgift eller ett problem och klicka sedan på **Öppna sammanfattning**.

   Information om hur du uppdaterar aktivitetsinformation i sammanfattningen i arbetsbelastningsutjämnaren finns i [Uppdatera arbetsobjekt i arbetsbelastningsutjämnaren med hjälp av sammanfattningen](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

1. Håll muspekaren över namnet på en aktivitet eller ett problem för att visa mer information om den. En ruta visas ovanför uppgiften eller problemet med följande information:

   * Namnet på uppgiften eller utgåvan.
   * Projektets namn.
   * Planerade start- och slutförandedatum.
   * Antal planerade timmar.
   * För uppgifter, föregående nummer.
   * För uppgifter, en indikator i det övre hörnet av rutan som anger om aktiviteten är klar att bearbetas eller inte.

   ![Uppgiftsinformation](assets/task-bar-hover-over-detail-wb.png)

1. Klicka på namnet på en arbetsuppgift till vänster för att komma åt den. Arbetsobjektet öppnas på en ny flik i webbläsaren.

### Visa belastningsutjämnaren i helskärmsläge

1. Gå till Utjämning av arbetsbelastning i området Resurser, vilket beskrivs i avsnittet [Öppna Utjämning av arbetsbelastning för flera projekt i området Resurser](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.

1. Klicka på ikonen **Helskärm** ![Helskärm](assets/full-screen.png) om du vill visa belastningsutjämnaren i helskärmsläge.

   Utjämning av arbetsbelastning tar upp hela skärmen. Webbläsarfönster och -flikar tas inte med i vyn.

1. Klicka på ikonen **Avsluta helskärmsläge** ![Avsluta helskärmsikonen](assets/exit-full-screen.png) om du vill återgå till standardskärmen och visa Utjämning av arbetsbelastning på webbläsarfliken.

## Navigera i ett teams arbetsbelastningsfördelning

Att navigera i ett teams belastningsutjämnare påminner om hur du navigerar i belastningsutjämnaren för flera projekt. Mer information finns i avsnittet [Navigera i arbetsbelastningsutjämnaren för flera projekt](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.

{{step1-to-team}}

Sidan i ditt hemteam visas som standard.

1. Klicka på **Utjämning av arbetsbelastning** i den vänstra panelen.

   ![Utjämning av arbetsbelastning för ett team](assets/nwe-balancer-team-350x172.png)

   Arbetsbelastningsutjämnaren för ett team visar följande information som standard:

   * I området **Ej tilldelat arbete**: Arbetsobjekt som tilldelats teamet eller team- och jobbrollerna och som inte är tilldelade användare. <span class="preview">Rolltilldelningar visas under arbetsobjekt i arbetsytan Ej tilldelat arbete när inställningen Visa rolltilldelningar är aktiverad.</span>
   * I området **Tilldelat arbete**: Arbetsobjekt som tilldelats användare visas under användarnas namn.

1. Fortsätt navigera i arbetsbelastningsutjämnaren för ett team enligt beskrivningen i avsnittet [Navigera i arbetsbelastningsutjämnaren för flera projekt i området Resurser](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.

## Navigera i arbetsbelastningsutjämnaren för ett enskilt projekt

{{step1-to-projects}}

1. Klicka på namnet på ett projekt för att öppna projektsidan.
1. Klicka på **Utjämning av arbetsbelastning** i den vänstra panelen.

   ![Utjämning av arbetsbelastning för ett projekt](assets/nwe-balancer-project-350x152.png)

   I arbetsbelastningsutjämnaren för projektet visas följande information som standard:

   * I området **Ej tilldelat arbete**: Arbetsobjekt i projektet som har tilldelats roller eller team och som inte har tilldelats användare. <span class="preview">Rolltilldelningar visas under arbetsobjekt i arbetsytan Ej tilldelat arbete när inställningen Visa rolltilldelningar är aktiverad.</span>
   * I området **Tilldelat arbete**: Arbetsobjekt i projektet som har tilldelats minst en användare.

   Vi rekommenderar att du bara använder filter för att visa användare som är viktiga för dig.

   Du kan till exempel överväga att endast visa användare som tillhör dina team eller grupper. Mer information finns i [Filtrera information i Utjämning av arbetsbelastning](../workload-balancer/filter-information-workload-balancer.md).

1. (Valfritt) Klicka på ikonen **Filter** ![Filtrera &#x200B;](assets/filter-icon.png) i området Tilldelad arbetsyta och välj alternativet **Det här projektets arbetsobjekt** i området **Förslag** i filterpanelen. Det här filtret är som standard avmarkerat.

   När det här alternativet är markerat visas endast de objekt som tilldelats användare i det valda projektet.

   När alternativet inte är markerat visas alla objekt som tilldelats användarna i projektet, oavsett vilka projekt som objekten tillhör.

1. (Valfritt och rekommenderas) Använd ett filter på arbetsytan Tilldelad arbetsyta för att visa användare som är viktiga för dig men som kanske inte är tilldelade till objekt i projektet. Klicka sedan på ikonen **Visa alla användare** ![Visa alla användare &#x200B;](assets/show-all-users-icon-project-workload-balancer.png) .

   Genom att visa alla användare kan du visa alla användare i Workfront som ännu inte är tilldelade till arbete eller andra roller i projektet.

   Du kan använda ett filter först för att minska antalet användare som visas.

   Du kanske först vill filtrera efter användare som tillhör dina team eller grupper och sedan visa alla dessa användare.

   Mer information om hur du skapar ett filter finns i [Filterinformation i Arbetsbelastningsutjämnaren](../workload-balancer/filter-information-workload-balancer.md).

   >[!NOTE]
   >
   > Alternativet Visa alla användare är bara tillgängligt för arbetsbelastningsutjämnaren för ett projekt.

1. (Valfritt) Klicka på ikonen **Visa rollallokeringar** ![Visa rollallokeringar](assets/show-role-allocation-icon.png).

   Panelen Rolltilldelning visas.

   Du kan visa information om planerade timmar som är associerade med projektets jobbroller och de jobbroller som är kopplade till initiativ som är kopplade till projekten från scenarioplaneraren.

   Mer information finns i [Översikt över att stämma av resursallokeringar mellan projekt och initiativ](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!NOTE]
   >
   >Du kan inte visa information om befattningsroll för initiativ om din organisation inte har köpt någon licens för Workfront Scenario Planner. I det här fallet kan du bara visa planerade timmar som är associerade med jobbroller i projektet. Mer information finns i [Åtkomst krävs för att använda scenarioplanen](../../scenario-planner/access-needed-to-use-sp.md).

1. Fortsätt navigera i arbetsbelastningsutjämnaren för ett projekt enligt beskrivningen i avsnittet [Navigera i arbetsbelastningsutjämnaren för flera projekt](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.

<div class="preview">

### Navigera i arbetsbelastningsutjämnaren för en användare

Du kan komma åt arbetsbelastningsutjämnaren på din egen användarprofil.

{{step1-click-profile-pic}}

1. Klicka på **Utjämning av arbetsbelastning** i den vänstra panelen.

   Arbetsbelastningsutjämnaren för användaren visas.

   ![Utjämning av arbetsbelastning för en användare](assets/workload-balancer-user.png)

   I arbetsbelastningsutjämnaren för en användare visas följande som standard:

   * **Tilldelat arbete**: Aktiviteter och ärenden som tilldelats den specifika användaren.

   >[!NOTE]
   >
   >Arbetsbelastningsutjämnaren i en användarprofil är skrivskyddad och tilldelningar och allokeringar kan inte ändras.

1. Fortsätt navigera i arbetsbelastningsutjämnaren för en användare enligt beskrivningen i avsnittet [Navigera i arbetsbelastningsutjämnaren för flera projekt](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) i den här artikeln.

</div>

<!--old content below - this used to be a one-large-procedure article - outdated, and rewrote it above with several smaller procedures: 

# Navigate the Workload Balancer

<!-drafted note for 22.4 release: remove all production/ preview references at Prod release>

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

Use the Workload Balancer to understand the availability of your resources as well as to assign work to your users. This article walks you through using the icons and settings available to update the view for and navigate the Workload Balancer.

>[!NOTE]
>
>The Workload Balancer is a resource scheduling tool that will eventually replace the current resource scheduling tools which are currently deprecated. 
>
>For more information about removing the resource scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
>
>We recommend that you use the Workload Balancer for scheduling your resources.

The Workload Balancer is available in multiple areas of Adobe Workfront. Navigating it is similar in all areas. This article describes how to navigate the Workload Balancer for multiple projects in the Resourcing area. For more information about where the Workload Balancer is located, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

For information about managing resources using the Workload Balancer, also consider reading the following articles:

* [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
* [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, when using the Workload Balancer in all areas in the Production environment</p>
   <p><span class="preview">Work, when using the Workload Balancer of a project, in the Preview environment</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for viewing items in the Workload Balancer

Consider the following when viewing the Workload Balancer:

* Projects display in the Workload Balancer only when the Group by Project setting is enabled. This setting is enabled by default.
* Mousing over a task or an issue displays the following additional information about the task or issue:

  * Project name

  * Task or issue name

  * Parent task

  * Planned Start and Completion Dates

  * Number of Planned Hours

  * Ready to start or Not ready status

  ![task-pop-up-with-additional-info-in-workload-balancer](assets/task-pop-up-with-additional-info-in-global-wb.png)

* When a project has no tasks during a period of time, the bar at the project level becomes a dimmed color.

  ![Break in project timeline](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* When you don't have permissions to see certain items, they display as **Inaccessible work items** or **Inaccessible projects**.

  ![Inaccessible items](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* The names of the work items display on the left and within the timeline selected on the right. 
* The total of Planned Hours for each work item displays to the right of the name of the work items on the left. 
* The total of the Planned Hours for each project displays to the right of the name of the project on the left.

  The Planned Hours information for the project is a total of Planned Hours from all items listed in the Workload Balancer, and not a total of Planned Hours on the project.

## Overview of the Unassigned Work and Assigned Work areas

The Workload Balancer displays work items in two separate areas, depending on their assignments.

The two areas of the Workload Balancer display the following information:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Unassigned Work</td> 
   <td> <p>This area displays tasks <span class="preview">and issues</span> unassigned to users. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>This area does not display any work items by default. We recommend using filters to display relevant information for you in this area.</p> <p>After you apply a filter, this area displays the following work items:</p> 
    <ul> 
     <li>unassigned</li> 
     <li>assigned to a team </li> 
     <li>assigned to a job role</li> 
     <li> <p>assigned to a team and a role at the same time</p> </li> 
    </ul> <p>Tip: Items assigned to a user as the primary assignee do not display in the Unassigned Work area. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assigned Work</td> 
   <td> <p> All active users in the system display in this area by default. We recommend using filters to limit the amount of information in this area.  </p> <p>Both tasks and issues display in the Assigned Work area. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>The work items that the users are assigned to display under their names. </p> <p>If a work item is assigned to multiple users, the item displays under each assigned user. </p> </td> 
  </tr> 
 </tbody> 
</table>

For information about applying a filter in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

![Empty unassigned area](assets/balancer-empty-unassiged-area-350x179.png)

## Navigate the Workload Balancer

You can update the view in the Workload Balancer to display exactly the information you need to focus on in the time frame that makes the most sense to you.

After selecting the settings you want to apply to your view, the Workload Balancer remembers these settings every time you access it from any browser or device.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Resourcing**.
1. Click **Workload Balancer** in the left panel.

   The Workload Balancer displays work assignment information starting with the current week. The names of work items are listed on the left side as well as represented by bars on the right side of the of the Workload Balancer within their respective timelines. By default, blue bars represent the timelines of projects and tasks and maroon bars represent issues.

   >[!TIP]
   >
   >You can change the color of the bars for projects and tasks when you select your color scheme to match the project. For more information, continue reading this procedure.

   The work items that display under the name of users in the Workload Balancer are sorted by the following criteria, in this order:

   1. Planned Start Date (oldest first)
   1. Planned Completion Date (oldest first)
   1. Alphabetical by project (only when the first two criteria are identical for multiple work items)

1. Click the right-pointing arrow to the left of the Unassigned or Assigned areas to expand all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Click the down-pointing arrow to the left of the Unassigned or Assigned areas to collapse all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Use the horizontal scroll to navigate the timelines of work items that extends beyond the limits of the screen. 
1. Use the vertical scroll to display additional users and work items. 
1. Drag and drop the separation line between the left panel and the timeline areas to adjust the size of the left panel.

   ![Separation between left panel and timeline](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. Click the **Filter icon** ![Filter icon](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or the **Assigned Work** areas to select the type of information to display in the Workload Balancer.

   For information about filtering information in the Workload Balancer, see [Manage filters in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md). 

1. Click the right-pointing arrow next to **Unassigned Work** to expand this area or the down-pointing arrow to collapse it.

   >[!TIP]
   >
   >No items display in this area by default. You must apply a filter to view unassigned work items.

1. Drag and drop the separation line between the **Unassigned Work** and **Assigned Work** areas to adjust their size.

   ![Separation line between areas](assets/modern-scheduler-separation-line-between-areas-350x278.png)

1. Click the back or forward icons ![Back and forward icons](assets/back-and-forward-icons.png) to navigate the timeline, then click **Today** to return to the current week. 

1. Click the **time frame drop-down menu** on the toolbar, then click the beginning date of the period you want to display. By default, the first week selected on the calendar is the week you navigated to.

   ![Calander date picker](assets/calendar-date-picker-wb.png)


1. Click one of the following options in the toolbar to display information by different time frames:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Day</td> 
      <td>Displays information by day for four weeks starting with today's date, by default. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Week</td> 
      <td>Displays information by week for four weeks. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Month</td> 
      <td> <p><span>Displays information by month for three months.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Select the number of weeks you want to display at one time in the Workload Balancer from the following options:

   * 1 week
   * 2 weeks
   * 4 weeks. This is the default setting.
   * 6 weeks
   * 3 months
   ![3 months dropdown](assets/3-months-12-weeks-drop-down-wb.png)     

1. Click the **Settings** icon ![Settings icon](assets/settings-gear-icon.png).

   The Settings panel displays.

   ![Settings box](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Select from the options listed below to update the information you view in the Workload Balancer, then click the **X icon** in the upper-right of the Settings box to close it.

   * **Group by Project**: When this is selected, the items in the Unassigned and Assigned Work areas are grouped by project. This is selected by default.

     ![Group by project](assets/group-by-project-350x530.png)

   * **Include hours from issues**: When this is selected, issues assigned to users display under the user's name in the Assigned Work area <span class="preview">and issues that are not assigned to users display in the Unassigned Work area</span>. The Planned Hours from the issues count towards the Planned Hours for the project and for the user in the Assigned Work area. 

        ![Issue on Workload Balancer](assets/issue-on-workload-balancer-350x20.png)

   
      * **Show Projected Dates**: When this is selected, the projected timeline of work items displays in addition to the planned timeline. Notice the following:

         * The projected timeline of project, tasks, and issues displays as a dark blue line above the task, issue, and project bars.
         * The projected timeline that is outside of the planned timeline displays in light blue, even when you update the color theme, as described below.
         * The projected timeline for the items that you have no access to view displays in light gray with a line underneath.
         * When a task or issue completes before the due Planned Completion Date the allocation numbers for the remaining days are struck through and do not count towards the user's allocation. This displays only when both the Show Projected Dates setting and the Show allocation icon are enabled.

         ![Task issue projected timelines](assets/task-issue-projected-timelines-350x91.png)

         >[!TIP]
         >
         >Notice that work items display in the Workload Balancer when either their planned or the projected timelines (not necessarily both at the same time) occur during the timeframe selected.

   * **Show completed work**: When this is enabled, tasks and issues that are completed display in the Assigned Work area. This is enabled by default.

     A green checkmark icon ![Checkmark icon](assets/green-checkmark-icon.png) displays to the upper-right corner of a task or issue bar when they are completed. The same icon displays for a project when the tasks or issues for the selected time frame of the project are completed. 
   
   * **Show remaining time**: When this is enabled, Workfront displays the difference between the daily time for which the user is available to work based on their schedules and the hours for which they are allocated in the Assigned Work area for the users. This is disabled by default and allocated time displays by default.

   * In the **Select color theme** section, select the color that you want for the project and task bars.  

      >[!NOTE]
      >
      >The setting for selecting the color theme  does not affect the color of the issue bars. Issues always display in a maroon-color bar. 


      Select from the following:

      * **Default**: The bars for all projects and their work items display in blue.  
      * **Project**: The bars associated with each project and its tasks change according to the name of the project. All tasks that belong to the project display in bars that match the color of the project. The project bars display in a lighter shade to distinguish them from the tasks. The project bars also include a project icon when choosing not to display allocations.
      * **Project Status**: The bars associated with each project and its work items change to the color of the status of the project.

        >[!TIP]
        >
        >* The project status is that associated with the Group of the project. If the Group does not have group-specific statuses, the color of the work item bars is that of the system-level project status. Both system as well as custom statuses display. For information about group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
        
   * In the **Display user allocation in** section, select from the following:

      * **Hours**: Displays allocated time as hours. This is the default. 
      * **Percentage**: Displays allocated time as a percentage of the total available time

   * In the **Sorting preferences** section, select how you want the items to be sorted in the Workload Balancer. Select from the following options: 

      * **Sort users by Primary Role**: Users display in the alphabetical order of their Primary Roles in the Assigned Work area.

      * **Sort users alphabetically**: Users display in the alphabetical order of their first names in the Assigned Work area.

      * **Sort projects by**: Select a project field from the drop-down menu to sort projects alphabetically by that field in the Unassigned or Assigned Work areas. 

      >[!TIP]
      >
      >You can sort by projects only when the Group by Project setting is enabled. Otherwise, this setting is dimmed.


1. (Optional and conditional) If you changed the color theme to Project Status, hover over the name of a project on the left to view the status of the project.

   ![Project status tooltip](assets/hover-over-project-status-tooltip-350x115.png)

1. <span class="preview">(Conditional and recommended) In the Workload Balancer of a project, apply a filter in the Assigned Work area to display users that are important to you but might not be assigned to items on the project, then click the **Show all users** icon ![Show all users   ](assets/show-all-users-icon-project-workload-balancer.png). This displays other users in the system that are not yet assigned on the project. For information about how to build a filter, see [Manage filters in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md).</span>

 
   >[!TIP]
   >
   ><span class="preview">The Show all users icon is available only for the Workload Balancer of a project.</span> 

1. Click the **Chart icon** ![Chart icon](assets/user-allocation-chart-icon.png) to display the user allocation in a chart format. Days where the user is overallocated display as red blocks, and days where the user is underallocated or at capacity display as blue blocks. The size of the blocks indicates the amount of the allocation: the larger the box, the more time the user is allocated to work items for that day or week.

   ![User allocation chart](assets/user-allocation-chart-350x237.png)

1. Click the **Show allocations icon** ![Show allocations icon](assets/show-allocations-icon-small.png) to view the daily or weekly Planned Hours for work items.

   This replaces the name in the bars of the work items with the amount of daily or weekly Planned Hours in the Unassigned and Assigned Work areas. This setting is disabled by default.

   >[!TIP]
   >
   >* The Show allocations setting only affects what displays for projects, tasks, issues and inaccessible items. Daily Planned Hours for users display by default and cannot be hidden.
   >* You must enable the Group by Project setting to display daily Planned Hours for projects. 
   >* When you view the Workload Balancer by week, the hours displayed are the weekly Planned Hours. 

   Days that show overallocations display in red. 

1. (Optional) Hover over the allocated time in the user line to understand what the capacity and allocation of the user. The capacity is the availability of the user according to their schedule.

   ![Overallocation vs capacity](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Optional) Click the **Hide allocations icon** ![Show allocations icon](assets/show-allocations-icon-small.png) to display the name of the tasks in the bars of the work items. 
1. Click the **More menu** icon ![More icon](assets/more-icon.png) to the right of a task or issue name, then click one of options below. 

   ![More menu](assets/more-menu-right-of-task-350x104.png)

      * **Assign this to**, then start typing the name of a user, role, or team you want to assign the work item to in the **Search people, role, or teams** field.
    
      >[!TIP]
      >
      >You can also use the following shortcuts to assign tasks or issues:
      >
      >* In Windows: CTRL+click the task or issue bar.
      >* In Mac: CMD+click the task or issue bar.

      For more information about assigning work items to users in the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md). 

      >[!TIP]
      >
      >If your Workfront or group administrator enabled delegations in your environment, use the Assignments tab to assign users to the task or issue. For information about delegating work, see [Manage task and issue delegation](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Edit allocations**, then edit the daily or weekly allocations for the user. For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

1. Click the bar of a task or issue to open the Summary panel on the right

   Or

   Click **Open Summary** icon ![Open Summary icon](assets/summary-panel-icon.png), then click the bar of a task or issue to open the Summary panel

   Or

   Click the **More** menu ![More icon](assets/more-icon.png) to the right of a task or issue, then click **Open Summary**.

   For information about updating task information in the Summary in the Workload Balancer, see [Update work items in the Workload Balancer using the Summary](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

    The Summary panel opens on the right. 

1. Click **Bulk Assignments** to assign work items in bulk.

   For more information, see [Assign work in bulk using the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md). 

1. Click the **Full screen** icon ![Full screen icon](assets/full-screen.png) to display the Workload Balancer in full screen, then click the **Exit full screen** icon ![Exit full screen](assets/exit-full-screen.png) to return to the default screen. 
1. (Optional) Double-click a daily or weekly allocation for a user inside the bar of a work item to edit the number of allocated hours, then click the **Save** icon ![Save icon](assets/save-allocations-wb.png) to save the allocations or the **Cancel** icon ![Cancel icon](assets/cancel-allocations-wb.png) to remove the allocations you adjusted.

   >[!TIP]
   >
   >The Save and Cancel icons display towards the end of a task or an issue's timeline bar.

   For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md). 

1. Click the name of a work item on the left to access it. 
1. Click the **Shareable link icon** ![](assets/wb-shearable-link-icon-small.png) to copy the direct URL for the Workload Balancer to your clipboard. 
1. (Optional) Share the link with any user who does not have direct access to the Workload Balancer.

   For information about sharing the Workload Balancer with a link, see [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md). 

1. (Conditional) From the Workload Balancer of a project, click the **Show role allocations** icon ![Show role allocations](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays. You can view information about Planned Hours associated with job roles on the project and job roles associated with initiatives from the Scenario Planner. For more information, see [Overview of reconciling resource allocations between projects and initiatives](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!TIP]
   >
   >You cannot view initiative job role information if your organization has not purchased a license for the Workfront Scenario Planner. In this case, you can only view the planned hours associated with job roles on the project. For more information, see [Access needed to use the Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md).

-->
