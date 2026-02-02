---
product-area: requests
navigation-topic: create-requests
title: Skapa och skicka begäranden
description: Planerat arbete representeras i Adobe Workfront av projekt och uppgifter. Du kan dock arbeta i en miljö där oplanerat arbete - i form av slumpmässiga begäranden - kan komma in när som helst. Workfront tillhandahåller ett arbetsflöde för den här typen av miljö genom att använda frågeköer.
author: Becky
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '2575'
ht-degree: 0%

---

# Skapa och skicka begäranden

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->


Planerat arbete representeras i Adobe Workfront av projekt och uppgifter. Du kan dock arbeta i en miljö där oplanerat arbete, i form av förfrågningar, kan komma in när som helst. Workfront tillhandahåller ett arbetsflöde för den här typen av miljö genom att använda frågeköer.

När du har skapat en begäran i en begärandekö kan du antingen tilldela den för slutförande eller konvertera den till en uppgift eller ett projekt.\
Mer information om hur du konverterar problem till en uppgift eller ett projekt finns i artikeln [Översikt över hur du konverterar problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Du kan skapa en Workfront-begäran på följande sätt:

* Från början enligt beskrivningen i den här artikeln.
* Från utkast. Mer information finns i [Skapa begäranden från utkast](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* Från en befintlig begäran genom att kopiera och skicka en kopia. Mer information finns i [Kopiera och skicka begäranden](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

Du kan skapa en ny Workfront Planning-begäran om du vill skapa poster i Workfront Planning på följande sätt:

* Från en länk till ett begärandeformulär för Workfront Planning.

* Från ett Workfront Planning-begärandeformulär i området Begäranden i Workfront.

  Din organisation måste köpa ett Workfront Planning-paket. Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Du måste ha Adobe Workfront Planning för att kunna visa planeringsförfrågningar eller begära formulär</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar för att använda frågeköer

En Workfront-administratör måste skapa begärandeköer och göra dem tillgängliga för användare innan de kan använda den här funktionen. En användare med en planerarlicens och med behörigheten Redigera för projekt och Hantera för ett visst projekt kan också skapa begärandeköer.

Mer information om hur du skapar frågeköer finns i artikeln [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

En Workfront-administratör måste skapa följande komponenter i en frågekö:

* Ett projekt med statusen Aktuell, publicerat som en kö för hjälpbegäran.
* Köämnen.\
  Mer information finns i artikeln [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Routningsregler.\
  Mer information finns i artikeln [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Valfritt) Ämnesgrupper.\
  Mer information finns i artikeln [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Valfritt) Begär eget formulär.\
  Mer information finns i artikeln [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* (Valfritt) Begär godkännandeprocess.\
  Mer information finns i artikeln [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Skapa förfrågningar och generera utkast i Workfront webbprogram

När du skapar en begäran i Workfront webbprogram sparar Workfront begäran som ett utkast innan du skickar den. Workfront skapar ett utkast så snart du har valt din begärandekö och börjar ange information om det.

Du kan fortsätta skicka begäran eller så kan du fylla i så mycket information du har och navigera bort från den för att slutföra den senare. Workfront sparar den ifyllda förfrågan som du har startat. Du kan hitta dem i:

* Ny begärande upplevelse: Listan över förfrågningar
* Äldre begärande upplevelse: Mappen Utkast

>[!IMPORTANT]
>
>Tänk på följande när du arbetar med utkast:
>
>* Workfront skapar inte utkastbegäranden när du skickar dem från ett tredjepartsprogram, som att skicka dem till Workfront eller skapa dem med något annat program. När du skickar en begäran utanför Workfront webbprogram sparas begäran i avsnittet Skickat.
>* Om strukturen för en begärandekö ändras kan du inte längre komma åt befintliga utkast. Om till exempel ett köämne tas bort, eller om en ämnesgrupp läggs till, är de sparade utkasten inte längre tillgängliga.
>

Mer information om hur du skapar begäranden från befintliga utkast finns i [Skapa begäranden från utkast](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Mer information om hur du tar bort utkast för begäranden finns i [Ta bort ett utkast för en begäran](../../../manage-work/requests/create-requests/delete-request-draft.md).

Så här skapar du en begäran i Workfront webbprogram:

{{step1-to-requests}}

1. (Valfritt och villkorligt) Välj inställningen **Växla till ny upplevelse** i skärmens övre högra hörn.

1. Klicka på **Ny begäran** i det övre högra hörnet på sidan.

   >[!TIP]
   >
   >* Du kommer åt alternativet Ny begäran från vilket avsnitt som helst i området Begäranden.
   >* Alternativet Ny begäran är nedtonat när du inte har behörighet att skapa problem.

   Rutan **Ny begäran** öppnas.

1. (Villkorligt) Om du växlade till det nya gränssnittet väljer du en av sökvägarna eller formulären i Workfront-frågekö eller klickar på sökfältet.

   När du klickar på sökfältet visas en listruta med de senast använda köerna och formulären först. Välj en från listan eller börja skriva och välj kön eller formuläret när det visas.

   >[!NOTE]
   >
   >Tänk på följande när det gäller den nya upplevelsen som begär:
   >* Listan innehåller både Workfront begärandeköer och Workfront Planning-förfrågningsformulär.
   >* Du kan filtrera listan efter objekttyp.
   >* I den nya begärandeupplevelsen finns utkast i samma lista som skickade begäranden.

1. (Villkorligt) Om du växlade till den nya versionen väljer du ämnesgrupper och köämnen och fortsätter att uppdatera formuläret.

   Annars klickar du i fältet **Typ av begäran** och gör något av följande:

   * I avsnittet **Senaste sökvägar** väljer du en sökväg som du nyligen använde för att öppna en frågekö. En sökväg innehåller begärandekön, ämnesgrupperna och det köämne som du skickade till nyligen. De sista tre banorna visas som standard.

     >[!NOTE]
     >
     >Workfront sparar bara en sökväg när du har skickat in en förfrågan. Det skapar inte vägar för utkast.

     ![Lista över senaste sökvägar och frågeköer när en ny begäran anges](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * Välj en begärandekö i avsnittet **Begärandeköer**.
   * Ange ett nyckelord som tillhör en tidigare använd sökväg för att söka efter en begärandekö.

     Om du till exempel har en frågekö med namnet &quot;Help Desk&quot; med namnet &quot;Location&quot; och ett köämne med namnet &quot;Remote&quot;, kan du skriva &quot;remote&quot; och alla begärandeköer som innehåller &quot;remote&quot; i alla element i sökvägsvisningen.

     >[!TIP]
     >
     >När du skriver ett namn som innehåller ett specialtecken visas begärandekön, köämnet eller ämnesgruppen även om du utelämnar att skriva tecknet.

     ![Begär sökresultat i kön med markerade resultat](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     Listan över tillgängliga begärandeköer och de senaste sökvägarna uppdateras dynamiskt så att endast sökvägar som innehåller nyckelordet som är markerat i resultaten inkluderas.

     Resultatet av sökningen visas under följande områden:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Begärandeköer</td> 
        <td>Begär köer som innehåller nyckelordet i deras namn</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Sökvägar för begäran</td> 
        <td> <p>Sökvägar (som innehåller begärandeköer, ämnesgrupper, köämnen) som innehåller nyckelordet i något av elementens namn</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* De första 200 begärandeköerna visas som standard i alfabetisk ordning.
   >* Namnet på begärandekön är namnet på det projekt som har publicerats som en kö för hjälpbegäran.
   >* Beskrivningen av projektet som konfigurerats som den valda begärandekön visas till höger om begärandeköns namn.
   >   
   >Mer information om hur du publicerar ett projekt som en hjälpfrågekö finns i artikeln [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Gör något av följande i formuläret **Ny begäran**:

   * (Villkorligt) Välj ett tillgängligt utkast i det meddelande som visas under fältet Typ av begäran.

     Det här området visas bara om du har sparat utkast innan utan att skicka dem.

     De tre senaste utkasten från tre olika köämnen visas som standard.

     ![Nya utkast efter att det nya begärandeområdet har tagits bort](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Börja ange en ny begäran i den valda kön.

     Ett nytt utkast sparas automatiskt i avsnittet Utkast när du har börjat ange information för den nya begäran och du ger begäran ett namn i fältet Ämne.

1. (Valfritt) Om din frågekö innehåller ämnesgrupper väljer du namnet på ämnesgruppen i det första nedrullningsbara fältet. Annars väljer du ett köämne.

   >[!TIP]
   >
   >När du hovrar över en ämnesgrupp eller ett köämne visas fältet Beskrivning till höger. Detta innehåller ytterligare information om ämnesgruppen eller köämnet.
   >
   >
   >![Visa beskrivning av köämne när begäran skickas](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)
   >

   Du kan ha upp till 10 nivåer av ämnesgrupper inbyggda i din frågekö.\
   Mer information om hur du skapar ämnesgrupper finns i artikeln [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Mer information om hur du skapar köämnen finns i artikeln [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   >
   >Om du har valt ett utkast eller en tidigare sökväg är ämnesgrupperna och köämnena redan markerade. Du kan välja en annan om det behövs.

1. Beroende på vilka fält som Workfront-administratören har aktiverat i avsnittet **Fält för nya problem** på underfliken **Köinformation** i projektet, kan du hitta något av följande fält när du skickar en ny begäran:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ämne</strong> </td> 
      <td>Ange ett namn för din begäran. Detta är ett obligatoriskt fält.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td>Ange en beskrivning av din begäran.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Ange en URL som kan relatera till din begäran.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioritet</strong> </td> 
      <td> <p>Ange en prioritet för din begäran. Prioriteten bör definiera hur snabbt du anser att denna begäran bör lösas. Standardalternativen är: </p> 
       <ul> 
        <li>Ingen</li> 
        <li>Låg </li> 
        <li>Normal</li> 
        <li>Hög</li> 
        <li>Urgent</li> 
       </ul> <p>Din systemadministratör kan ändra namnen på prioriteter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Allvarlighetsgrad</strong> </td> 
      <td> <p>Ange en allvarlighetsgrad för din begäran. Allvarlighetsgraden bör definiera hur den här förfrågan påverkar ditt arbete om den inte kan lösas i tid. Standardalternativen är:</p> 
       <ul> 
        <li>Kosmetisk</li> 
        <li>Orsakar förvirring</li> 
        <li>Fel med tillfälliga lösningar</li> 
        <li>Fel utan någon lösning</li> 
        <li>Allvarligt fel</li> 
       </ul> <p>Systemadministratören kan ändra namnen på allvarlighetsgraden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primär kontakt</strong> </td> 
      <td>Den primära kontaktpersonen för en begäran är dig som standard, eftersom du är den person som ska besvara eventuella frågor som rör begäran. Du kan dock ändra detta till vilken annan Workfront-användare som helst.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Uppdrag</strong> </td> 
      <td> <p><span>Ange namnet på en aktiv användare, jobbroll eller ett team som begäran ska tilldelas.</span> </p> <p>Du kan bara ange ett team.</p>

   <p> Beroende på hur frågekö konfigurerades kan du kanske bara tilldela en eller två typer av resurser till begäran i stället för alla tre (du kanske bara kan tilldela begäran till användarna).</p>

   <p>Om en routningsregel även är associerad med begärandekön och den automatiskt dirigerar begäran till en annan typ av resurs (till exempel ett team), tilldelas din begäran både till den enhet som du anger manuellt när du skickar begäran (användare) och den resurs som anges i routningsregeln (teamet). </p>

   <p> Mer information finns i följande artiklar:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Skapa routningsregler</a> <br> </p> </li> 
      </ul> </p>

   <p><span>Vi rekommenderar att du använder routningsregler för dina begärandeköer så att de automatiskt kan dirigeras till rätt resurser.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Planerade timmar</strong> </td> 
      <td> <p>Beräkna hur många timmar det skulle ta för den här begäran att slutföras.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planerat startdatum</strong> </td> 
      <td> <p>Ange det datum då arbetet med denna begäran ska starta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planerat slutförandedatum</strong> </td> 
      <td>Ange det datum då du vill att den här begäran ska lösas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>Standardstatusen för en ny begäran är "Ny". Systemadministratören kan ha ändrat namnet på den här statusen. Du kan också ändra statusen till något annat i den här nedrullningsbara menyn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dokument</strong> </td> 
      <td> <p>Lägg till dokument i din begäran. </p> <p> Beroende på hur frågekö konfigurerades kan avsnittet Dokument visas före eller efter de anpassade fälten. </p> <p>Dokument som du överför till Workfront lagras i 24 timmar som utkast. Därefter måste du bifoga dem igen när du går tillbaka och redigerar och skickar utkastet. Dokument som är länkade från andra enheter sparas permanent i utkastet. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Om din Workfront-administratör har kopplat ett anpassat formulär till begärandekön eller till avsnittet Kö anger du fälten i det anpassade formuläret.\
   Anpassade formulär är olika för alla Workfront-instanser.
1. (Valfritt och villkorligt) Klicka på [!UICONTROL **Ignorera utkast**] när som helst när du anger begäran om du vill ta bort det utkast som skapas automatiskt. Detta tar bort utkastet som inte kan återställas. Ett bekräftelsemeddelande visas som bekräftar att du håller på att ta bort utkastet.

1. (Valfritt) Klicka på [!UICONTROL **Ångra**] i bekräftelsemeddelandet om du vill återställa åtgärden och behålla utkastet.

1. Gör något av följande:

   * Klicka på **Skicka** om du är redo att skicka begäran. Begäran sparas i avsnittet Skickat. Beroende på hanteringsregeln för begärandekön kan den här begäran dirigeras till ett annat projekt än det som angetts som en begärandekö. Mer information om routningsregler finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     eller

     Klicka på **Stäng** om du inte är redo att skicka det och du kanske kommer tillbaka och slutför det senare. Din begäran sparas i avsnittet Utkast och blir tillgänglig nästa gång du skickar en begäran för den här kön.

     ![Skicka, stäng, ignorera utkastknapp på ny begäran](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   När du skickar begäran tas utkastet automatiskt bort och kan inte återställas.

   Skickade begäranden visas i avsnittet **Skickade** i området Begäranden. Om du använder den nya versionen visas de förfrågningar som Workfront har skickat på fliken **Workfront** i området Förfrågningar.

   Mer information om hur du hanterar inkommande begäranden finns i artikeln [Hantera arbets- och teamförfrågningar](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Mer information om hur du söker efter skickade eller skrivna begäranden finns i [Leta reda på skickade begäranden](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Skapa förfrågningar utanför Workfront

Du kan dela en direktlänk till en begärandekö när du skickar en ny begäran och bädda in den i andra program. Användare som kommer åt den här länken från webben eller från andra program måste också vara inloggade med ett aktivt Workfront-konto för att kunna komma åt den här kön och skicka begäranden till den. Mer information finns i [Dela en länk till en begärandekö](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Skapa förfrågningar genom att mejla till Workfront

Om din begärandekö är aktiverad för att ta emot begäranden via e-post, kan du skicka dina begäranden direkt till den e-postadress som är kopplad till begärandekön.

Brödtexten i e-postmeddelandet läggs till som begärandebeskrivning.

>[!NOTE]
>
>HTML-formatering tas bort när begäran kommer in i Workfront, men signaturer och befintligt svarstrådinnehåll tas inte bort och visas i begärandebeskrivningen.

Mer information om hur du aktiverar en begärandekö för att ta emot begäranden via e-post finns i [Ge användare behörighet att skicka ett problem via e-post till ett begärandeköprojekt](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Skapa förfrågningar med Workfront mobilapp

Du kan skicka begäranden med mobilappen på din smarttelefon. Du kan skapa en ny begäran och skicka den till de begärandeköer som du har åtkomst till för att se i webbprogrammet.

Mer information om hur du skickar begäranden via mobilappen finns i avsnittet med förfrågningar i artiklarna:

* [Adobe Workfront för Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests)
* [Adobe Workfront för iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## Skapa förfrågningar från andra program

Du kan skicka in begäranden med alla program som har integrerats med Workfront:

* Du kan skapa en anpassad integrering mellan Workfront och ett annat program som gör att du kan skicka begäranden till Workfront från det andra programmet.\
  Mer information om anpassade Workfront-integreringar finns i artikeln [Adobe Workfront-integreringar](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

## Skapa begäranden med hjälp av ett Workfront Planning-formulär

Du kan lägga till en Workfront Planning-begäran med ett Planning-begärandeformulär. Om du lägger till Workfront Planning-begäranden kan Planning-poster skapas, om begärandeformuläret har godkänts eller om det inte kräver godkännande.

Din organisation måste köpa ett Workfront Planning-paket för att kunna skicka in planeringsförfrågningar.

Mer information finns i följande artiklar:

* [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Sök efter skickade begäranden

Mer information om hur du söker efter skickade eller skrivna begäranden finns i [Leta reda på skickade begäranden](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
