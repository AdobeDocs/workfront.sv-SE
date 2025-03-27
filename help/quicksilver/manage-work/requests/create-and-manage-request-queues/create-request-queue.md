---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Skapa en begärandekö
description: Du kan skapa en frågekö där användare kan ange tillfälliga begäranden som inte är planerade för ett projekt. En kö för helpdesk-begäran kan till exempel ställas in så att den fångar upp alla användarförfrågningar som kommer till en IT-avdelning.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '5167'
ht-degree: 0%

---


# Skapa en begärandekö

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Du kan skapa en frågekö där användare kan ange tillfälliga begäranden som inte är planerade för ett projekt. En kö för helpdesk-begäran kan till exempel ställas in så att den fångar upp alla användarförfrågningar som kommer till en IT-avdelning.

Förfrågningar blir problem i Adobe Workfront och de läggs till i projekt.

Genom att ställa in en begärandekö kan du formatera information om problem som ska läggas till i ett projekt. Alla ärenden som skickas in till projektet kommer att skickas på samma sätt och på samma sätt.

Du kan ställa in följande objekt som begärandeköer i Workfront:

* Projekt
* Mallar. Projekt som skapats från mallar som konfigurerats som begärandeköer blir begärandeköer.

Om du vill konfigurera ett projekt eller en mall som en begärandekö måste du redigera området Köinformation för projektet eller mallen.

I den här artikeln beskrivs hur du konfigurerar ett projekt som en begärandekö där användare kan skicka begäranden. Att ställa in köinformation för en mall påminner om att ställa in dem i projektet.

Mer information om hur du skickar en ny begäran till en begärandekö finns i [Kopiera och skicka begäranden](../create-requests/copy-and-submit-requests.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Ny licens: Standard </p>
   eller
   <p>Aktuell licens: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Hantera behörigheter för projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över köer för begäranden

Du ställer in en begärandekö som ett projekt. När du anger projektet som en frågekö blir kön tillgänglig från området med förfrågningar i Adobe Workfront. När du anpassar begärandekön anpassar du också de formuläranvändare som fyller i när de skickar förfrågningarna.

I den här artikeln beskrivs hur du skapar en begärandekö från ett befintligt projekt. För att skapa en konsekvent process för inhämtning av begäranden eller för att lägga till flera lager i den för rapportering och bättre hantering, kan du även konfigurera ytterligare byggstenar i en begärandekö som beskrivs i följande tabell.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Köinformation</td> 
   <td> <p>Du måste konfigurera ett projekt som en begärandekö i området Köinformation. Detta steg är obligatoriskt. </p> <p>Mer information finns i avsnittet <a href="#create-a-request-queue" class="MCXref xref">Skapa en frågekö</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ämnesgrupper</td> 
   <td> <p>Det är ytterligare menyer som klassificerar begäranden baserat på gemensamma funktioner. För en IT-frågekö kanske du vill ha ämnesgrupper"på plats" och"på fjärrplats". </p> <p>Mer information finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Skapa ämnesgrupper</a>. </p> <p>Detta är valfritt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Köämnen</td> 
   <td> <p>Det är ytterligare menyer som klassificerar begäranden som tillhör samma ämnesgrupp baserat på gemensamma funktioner. En ämnesgrupp kan innehålla flera köämnen. </p> <p>Ämnesgruppen "På plats" för IT-frågekö kan till exempel innehålla avsnitten "Maskinvara", "Programvara" och "Nätverk". </p> <p>Mer information finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Skapa köämnen</a>. </p> <p>Detta är valfritt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Routningsregler</td> 
   <td> <p>De gör att du kan dirigera varje begäran till en användare, en jobbroll, ett team eller ett projekt. </p> <p>Mer information finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Skapa routningsregler</a>. </p> <p>Detta är valfritt.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Skapa en begärandekö

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

Hur du skapar en frågekö varierar beroende på vilken miljö du använder.

### Skapa en begärandekö i produktionsmiljön

I det här avsnittet beskrivs hur du kan definiera köinformation för följande objekt:

* Ett projekt i produktionsmiljön
* En mall i produktions- eller förhandsvisningsmiljön

När du ställer in ett projekt som en frågekö måste projektstatusen vara Aktuell för att kunna visas i området Begäranden i Workfront.

>[!TIP]
>
>Din Workfront- eller gruppadministratör kan tilldela dig till en anpassad layoutmall som kanske inte innehåller några av de avsnitt som beskrivs i följande steg.


Så här skapar du en begärandekö:

1. Gå till det projekt som du vill konfigurera som en frågekö.
1. (Valfritt) Klicka på **Projektinformation** i den vänstra panelen och lägg till en **beskrivning** i projektet i området **Översikt**. Den här informationen visas för alla nya begäranden.
1. Klicka på **Köinformation** i den vänstra panelen. Du kan behöva klicka på **Visa mer** och sedan på **Köinformation**.

   Då öppnas avsnittet Köinformation.

   ![Köinformation högst upp i avsnittet](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Ange följande information:

   * **Publicera som kö för hjälpbegäran:** Välj det här alternativet om du vill identifiera det här projektet som en begärandekö. Alla inkommande problem betraktas som begäranden.\
     När det här alternativet inte är markerat fungerar projektet som ett standardprojekt i Workfront och alla inkommande problem är problem.

   * **Vem kan lägga till begäranden i den här kön:** Välj vilka användare som har åtkomst att lägga till begäranden i den här kön. Du kan tillåta följande grupper av personer att se begärandekön i området Förfrågningar i det globala navigeringsfältet när de lägger till en ny begäran:

     | Vem kan skriva in förfrågningar? | Beskrivning |
     |---|---|
     | Alla | Alla Workfront-användare med ett aktivt konto kan visa den här begärandekön och lägga till begäranden i den |
     | Personer med visningsåtkomst till det här projektet | Användare med behörigheten Visa i projektet kan visa och lägga till begäranden i den här kön |
     | Personer i det här projektets företag | Användare som tillhör det företag som är associerat med det här projektet kan visa och lägga till begäranden i den här kön. Om det finns ett företag som är associerat med projektet visas företagets namn inom parentes efter den här inställningen. |
     | Personer i det här projektets grupp | Användare som tillhör gruppen som är kopplad till det här projektet kan visa och lägga till begäranden i den här kön. Om det finns en grupp som är associerad med projektet visas gruppens namn inom parentes efter den här inställningen, i grått teckensnitt. |

     {style="table-layout:auto"}

   * **Dela med de här länkarna:** Med följande alternativ kan du ge direktåtkomst till begärandekön och de formulär som är kopplade till den till användare utanför Workfront eller till Workfront-användare via en extern sida. Mer information om hur du bäddar in en begärandekö i en instrumentpanel som en extern sida finns i [Bädda in en begärandekö i en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Användarna måste redan ha åtkomstbehörighet till begärandekön för att få direkt åtkomst. Om du använder något av de alternativ som beskrivs här beviljas inte automatiskt åtkomst till användare.

     >[!TIP]
     >
     >Användarna måste först logga in på Workfront innan de får åtkomst till kön när de öppnar sidan Begärandekö från ett annat program.

      * **URL för direktåtkomst:** När en användare öppnar den här URL:en från en webbläsare, dirigeras användaren direkt till avsnittet Ny begäran i området Begäranden och denna begäran väljs som standard för dem.

        ![Dela begärandekö med direkt URL inbäddad i instrumentpanelen](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >Du kan visa en frågekö i en instrumentpanel som en extern sida. I det här fallet är begärandekön förvald, men du kan välja vilken annan begärandekö som helst från fältet Typ av begäran. -användare kan ändra frågetypen. Navigeringskomponenterna för begäranden visas också.

      * **Bädda in kod:** Använd den här HTML-koden för att bädda in formuläret för begärandekön som en iframe på en HTML-sida.\
        Om användare inte redan är autentiserade i Workfront när de visar sidan där koden är inbäddad, visas inloggningsdialogrutan för Workfront. När användarna har loggat in visas formuläret Begärandekö.

        >[!NOTE]
        >
        >När du visar en begärandekö i en iframe visas endast begärandeformuläret, begärandenamnet är förmarkerat och nedtonat. Användaren kan inte ändra typen för begäran. Navigeringskomponenterna i området Begäranden visas inte.

        För att formuläret för begärandekön ska kunna visas när du använder den här inbäddningskoden måste du aktivera inställningen&quot;Tillåt inbäddning av Workfront i en iframe&quot; i systeminställningarna. Mer information om hur du aktiverar inbäddning av Workfront i en iframe finns i [Konfigurera systemsäkerhetsinställningar](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Om den här inställningen inte är aktiverad visas iframe-elementet som tomt.

        Du kan justera olika aspekter av hur det inbäddade formuläret visas enligt följande:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funktionalitet</strong> </p> </th> 
           <th> <p><strong>Lösning</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Justera ramens storlek</p> </td> 
           <td> <p>Ändra attributen för bredd och höjd.</p> <p>Som standard är bredden"500" och höjden"600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direktanvändare till en viss ämnesgrupp eller ämnesgrupp i kön</p> </td> 
           <td> <p>Lägg till parametern "path" i src-URL:en. Du kan hitta parametern path genom att navigera till önskad köämnesgrupp eller ämnesgrupp i det ej inbäddade formuläret och kontrollera URL:en.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Visa och tillåt användare att ändra den förkonfigurerade listrutan Ämnesgrupp</p> </td> 
           <td> <p>Använd parametern "path" genom att lägga till parametern <code>showPreSelectedOptions=true</code> i <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Identifiera när formuläret har skickats</p> </td> 
           <td> <p>Lägg till en meddelandehändelseavlyssnare i webbsidans fönster och kontrollera om <code>event.data.type</code> är <code>requestSubmitted</code>. <code>event.data.newIssueID</code> anges till ID:t för det skapade problemet.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Begärantyper:** Välj bland standardalternativen nedan.

     Workfront-administratören kan byta namn på standardförfrågningstyperna. Mer information om hur du byter namn på typer av förfrågningar finns i [Anpassa standardproblemtyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Felrapport
      * Ändra ordning
      * Problem
      * Begäran

        Detta är ett obligatoriskt fält och du måste välja minst ett alternativ.

     >[!NOTE]
     >
     >Begärantyper visas bara som ett urval i området Förfrågningar om frågetypen har valts både på sidorna Köinformation och på sidorna Köämne. Mer information om hur du konfigurerar området Köinformation för ett projekt finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Alla typer som markeras här är tillgängliga i formuläret (du kan markera fler än en). Om du väljer mer än en typ kan du ordna flera förfrågningar som kommer in.\
     Om du till exempel använder formuläret i en begärandekö för ett IT-projekt kan följande typer av begäranden placeras i kön: maskinvara, programvara, felkorrigeringar och problem.

   * **Standardvaraktighet:** Standardlängden är den tid det normalt tar att slutföra ett problem. Detta blir standard för alla inkommande ärenden och kan ändras manuellt. Varaktigheten anges vanligtvis i timmar, dagar eller veckor. Standardlängden för ett problem är densamma som de planerade timmarna för problemet. Det planerade slutförandedatumet för problemet beräknas utifrån det här fältet.\
     Standardvärdet för utfärdandevaraktighet är 1 dag eller 8 timmar. Om Workfront-administratören ställer in Normal timma per arbetsdag till mindre än 8 timmar är standardvaraktigheten för utgåvor fortfarande 8 timmar. Om t.ex. antalet timmar per arbetsdag är 7 timmar är standardlängden för utleveranser 1,14 dagar eller 8 timmar. Mer information om hur du ställer in systemet för beräkning av normaltimmar per arbetsdag finns i avsnittet &quot;Beräkningar av tidslinje&quot; i artikeln [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Personer från samma företag ärver samma behörigheter för alla begäranden.:** Om du väljer det här alternativet visas alla begäranden som skickas till kön för användare i samma företag. Användare kan visa dessa begäranden i avsnittet Alla begäranden, som finns i området Begäranden. När den här inställningen är aktiverad eller inaktiverad påverkas alla framtida förfrågningar. Informationen påverkas inte retroaktivt.
   * **När någon gör en begäran tilldelar automatiskt:** När en användare gör en begäran till kön, tilldelas användaren automatiskt den behörighetsnivå som du väljer för den begäran. Välj bland följande behörighetsnivåer:

      * **Visa åtkomst**
      * **Contribute Access**. Det här är standardvalet.
      * **Hantera åtkomst**

     Mer information om Workfront behörighetsmodell finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Om du anger behörigheter här sparar du tid i stället för att behöva bevilja behörigheter för varje enskild inkommande begäran. Om du väljer det här alternativet påverkas alla framtida förfrågningar, men befintliga förfrågningar påverkas inte retroaktivt.

   * **Standardgodkännande**: Associera en godkännandeprocess med den här begärandekön. Endast godkännandeprocesser för problem visas i den här listrutan. Alla utleveranser som skickas till den här kön kommer att associeras med den här godkännandeprocessen. Workfront-administratören måste definiera godkännandeprocesser på systemnivå innan du kan koppla dem till begärandeköer. Användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser.

     >[!IMPORTANT]
     >
     >Om projektgruppen ändras blir den gruppspecifika godkännandeprocess som är kopplad till befintliga utgåvor en godkännandeprocess för engångsbruk. Mer information om hur ändringar i projektgruppen eller ändringar i godkännandeprocessen påverkar godkännandeinställningarna finns i [Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Om du har flera köämnen associerade med en begärandekö rekommenderar vi att du i stället kopplar godkännandeprocesser till köämnena. Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Tänk på följande när du lägger till godkännandeprocesser i begärandeköer:

      * Endast aktiva godkännandeprocesser visas i listan.
      * Systemomfattande och gruppspecifika godkännandeprocesser visas i listan. En godkännandeprocess som är associerad med en annan grupp än den som projektet har visas inte i listan.

   * **Standardflöde**: Associera en routningsregel med den här begärandekön. Använd routningsregler för att automatiskt tilldela nya ärenden som skickas till en begärandekö till rätt resurs (användare, jobbroll eller team) och till rätt projekt. Alla utleveranser som skickas till den här kön kommer att associeras med den här routningsregeln. Du måste konfigurera routningsregler innan de visas i avsnittet Köinformation och innan du kan associera dem med begärandekön.\
     Om du har flera köämnen som är associerade med en frågekö rekommenderar vi att du i stället kopplar routningsregler till köämnena. Mer information om hur du skapar routningsregler finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nya fält för problem:** I avsnittet **Visa följande markerade fält för alla användare** markerar du de fält som du vill ska vara synliga för alla användare som skickar en begäran till projektet eller lägger till ett problem i projektet eller aktiviteterna.

     >[!TIP]
     >
     >Nya fält för problem som har valts i avsnittet Köinformation är också associerade med nya problem som har lagts till i projektet <!--this is confusing: or to the tasks in the Issues section-->.

     När du aktiverar något av fälten Tilldelad till, Jobbroll eller Team ändras alltid namnen till Tilldelningar i formuläret för begäran, men du kan bara ange vilken typ av uppdrag som har valts här.

     >[!NOTE]
     >
     >Om du markerade Tilldelad till i området Köinformation kan du bara ange användare i fältet Uppdrag i formuläret för begäran. I det här fallet kan du inte ange jobbroller eller ett team.

   * **Dokument**: Om du väljer att visa avsnittet Dokument i det nya formuläret för begäran, väljer du var avsnittet för dokumentöverföring ska placeras. Välj bland följande:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Efter anpassade formulär</td> 
        <td><span>Avsnittet Dokument visas längst ned i formuläret för begäran.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Före anpassade formulär</td> 
        <td> <p><span>Avsnittet Dokument visas mellan Workfront-fälten och de anpassade fälten i det begärda formuläret.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Nytt fältområde för utgåva med dokument](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Visa alla markerade och omarkerade fält till:** Välj vilka användare du vill visa alla fält i det nya begärandeformuläret. Följande alternativ styr åtkomsten till fälten i formuläret.

     | Vilka användare som kan se alla fält i det begärda formuläret | Beskrivning |
     |---|---| 
     | Alla användare (Planera licenser) | Alla användare som har en planlicens kan se både det markerade och de omarkerade fälten. |
     | Personer med visningsåtkomst till det här projektet (planlicens) | De användare som har en planlicens som även har visningsbehörighet för det här projektet kan se både det valda och de omarkerade fälten. Resten av användarna som kan skicka begäranden till det här projektet kan se endast de valda fälten. |
     | Inga användare | Inga användare kan se de omarkerade fälten. Alla användare som kan skicka begäranden till det här projektet kan bara se de markerade fälten. |

   * **Anpassad Forms**: Välj ett anpassat formulär som ska associeras med begärandekön. Det är bara Issue Custom Forms (Utforma anpassad) som du kan välja i den här listrutan. Alla utleveranser som skickas till begärandekön har de valda formulären kopplade till sig. Du måste skapa anpassade formulär innan du kan se dem i avsnittet Köinformation.
Om du har flera köämnen kopplade till en frågekö rekommenderar vi att du i stället kopplar anpassade formulär till köämnen. Mer information om hur du skapar underavsnitt för begärandekön finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Anpassade formulär i köinformation](assets/custom-forms-on-queue-details.png)

     Om du har flera anpassade formulär kopplade till frågekö drar och släpper du formulären för att sortera dem i önskad ordning i avsnittet **Ändra ordning på Forms**.

     >[!TIP]
     >
     >Anpassade formulär som läggs till i avsnittet Köinformation är också associerade med nya problem som har lagts till i projektet <!--this is confusiong: or the tasks in the Issues  section-->.

1. Fortsätt att välja information för inställningarna i området **Inställningar för e-postkö** så att användare kan skicka begäranden via e-post till begärandeköprojektet.

   Mer information finns i [Gör det möjligt för användare att skicka ett problem via e-post till ett begärandeköprojekt](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Klicka på **Spara**.\
   Ditt projekt har nu konfigurerats som en frågekö och användare kan nu lägga till begäranden i det.

1. (Valfritt) Om du vill förbättra funktionen för begärandekö skapar du ytterligare underavsnitt för kön samt regler som dirigerar inkommande begäranden till rätt team, uppdragsgivare eller projekt.

   * Mer information om hur du skapar underavsnitt för begärandekön finns i artiklarna [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) och [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Mer information om hur du dirigerar begäranden till lämplig tilldelare, team och lämpligt projekt finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

<div class="preview">

### Skapa en begärandekö i förhandsgranskningsmiljön

När du ställer in ett projekt som en frågekö måste projektstatusen vara Aktuell för att kunna visas i området Begäranden i Workfront.

>[!TIP]
>
>Din Workfront- eller gruppadministratör kan tilldela dig till en anpassad layoutmall som kanske inte innehåller några av de avsnitt som beskrivs i följande steg.

Så här skapar du en begärandekö:

1. Gå till det projekt som du vill konfigurera som en frågekö.
1. (Valfritt) Klicka på **Projektinformation** i den vänstra panelen och lägg till en **beskrivning** i projektet i området **Översikt**. Den här informationen visas för alla nya begäranden.
1. Klicka på **Köinformation** i den vänstra panelen. Du kan behöva klicka på **Visa mer** och sedan på **Köinformation**.

   Då öppnas avsnittet Köinformation.

   ![Avsnittet Kötyp i området Köinformation](assets/unshimmed-queue-type-section-queue-details-area.png)

1. Ange följande information:

   * **Publicera som kö för hjälpbegäran**: Välj det här alternativet om du vill identifiera det här projektet som en begärandekö. Alla inkommande problem betraktas som begäranden.\
     När det här alternativet inte är markerat fungerar projektet som ett standardprojekt i Workfront och alla inkommande problem är problem.

   * **Vem kan lägga till begäranden i den här kön?**: Välj vilka användare som har åtkomst att lägga till begäranden i den här kön. Du kan tillåta följande grupper av personer att se begärandekön i området Förfrågningar i det globala navigeringsfältet när de lägger till en ny begäran:

     | Vem kan skriva in förfrågningar? | Beskrivning |
     |---|---|
     | Alla | Alla Workfront-användare med ett aktivt konto kan visa den här begärandekön och lägga till begäranden i den |
     | Personer med visningsåtkomst till det här projektet | Användare med behörigheten Visa i projektet kan visa och lägga till begäranden i den här kön |
     | Personer i det här projektets företag | Användare som tillhör det företag som är associerat med det här projektet kan visa och lägga till begäranden i den här kön. Om det finns ett företag som är associerat med projektet visas företagets namn inom parentes efter den här inställningen. |
     | Personer i det här projektets grupp | Användare som tillhör gruppen som är kopplad till det här projektet kan visa och lägga till begäranden i den här kön. Om det finns en grupp som är associerad med projektet visas gruppens namn inom parentes efter den här inställningen, i grått teckensnitt. |

     {style="table-layout:auto"}

   * Använd följande alternativ för att ge direktåtkomst till begärandekön och tillhörande formulär till användare utanför Workfront eller till Workfront-användare via en inbäddad extern sida.

   Mer information om hur du bäddar in en begärandekö i en instrumentpanel som en extern sida finns i [Bädda in en begärandekö i en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

   Användarna måste först ha behörighet till begärandekön för att få direkt åtkomst. Om du använder något av de alternativ som beskrivs här beviljas inte automatiskt åtkomst till användare.

   >[!TIP]
   >
   >Användarna måste först logga in på Workfront innan de får åtkomst till kön när de öppnar sidan Begärandekö från ett annat program.

   * **URL för direktåtkomst:** När en användare öppnar den här URL:en från en webbläsare, dirigeras användaren direkt till avsnittet Ny begäran i området Begäranden och denna begäran väljs som standard för dem.

     ![Ny begäranderuta från direktwebbadressresurs](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >Du kan visa en frågekö i en instrumentpanel som en extern sida. I det här fallet är begärandekön förvald, men du kan välja vilken annan begärandekö som helst från fältet Typ av begäran. Användare som skickar begäran kan välja en annan typ av begäran. Ämnesgrupper och Köämnen visas också.

   * **Bädda in kod:** Använd den här HTML-koden för att bädda in formuläret för begärandekön som en iframe på en HTML-sida.\
     Om användare inte redan är autentiserade i Workfront när de visar sidan där koden är inbäddad, visas inloggningsdialogrutan för Workfront. När användarna har loggat in visas formuläret Begärandekö.

     >[!NOTE]
     >
     >När du visar en begärandekö i en iframe visas endast begärandeformuläret, begärandenamnet är förmarkerat och nedtonat. Användaren kan inte ändra typen för begäran. Navigeringskomponenterna i området Begäranden visas inte.

     För att formuläret för begärandekön ska kunna visas när du använder den här inbäddningskoden måste Workfront-administratören aktivera inställningen Tillåt inbäddning av Workfront i en iframe i systemkonfigurationsområdet.

     Mer information om hur du aktiverar inbäddning av Workfront i en iframe finns i [Konfigurera systemsäkerhetsinställningar](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Om den här inställningen inte är aktiverad visas iframe-elementet som tomt.

     Du kan justera olika aspekter av hur det inbäddade formuläret visas enligt följande:

     <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funktionalitet</strong> </p> </th> 
           <th> <p><strong>Lösning</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Justera ramens storlek</p> </td> 
           <td> <p>Ändra attributen för bredd och höjd.</p> <p>Som standard är bredden"500" och höjden"600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direktanvändare till en viss ämnesgrupp eller ämnesgrupp i kön</p> </td> 
           <td> <p>Lägg till parametern "path" i src-URL:en. Du kan hitta parametern path genom att navigera till önskad köämnesgrupp eller ämnesgrupp i det ej inbäddade formuläret och kontrollera URL:en.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Visa och tillåt användare att ändra den förkonfigurerade listrutan Ämnesgrupp</p> </td> 
           <td> <p>Använd parametern "path" genom att lägga till parametern <code>showPreSelectedOptions=true</code> i <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Identifiera när formuläret har skickats</p> </td> 
           <td> <p>Lägg till en meddelandehändelseavlyssnare i webbsidans fönster och kontrollera om <code>event.data.type</code> är <code>requestSubmitted</code>. <code>event.data.newIssueID</code> anges till ID:t för det skapade problemet.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Typ av begäran:** Välj bland följande alternativ i avsnittet **Egenskaper för kö**:

   * Felrapport
   * Ändra ordning
   * Problem
   * Begäran

   Detta är ett obligatoriskt fält och du måste välja minst ett alternativ.

   Workfront-administratören kan byta namn på standardförfrågningstyperna. Mer information om hur du byter namn på typer av förfrågningar finns i [Anpassa standardproblemtyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

   >[!NOTE]
   >
   >När användare öppnar kön med begäranden från området med förfrågningar visas frågetyper som ett urval endast om frågetypen har valts både på sidorna Köinformation och på sidorna med köämnen.
   >
   >Mer information om hur du konfigurerar området Köämnen i ett projekt finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   Alla typer som markeras här är tillgängliga i formuläret (du kan markera fler än en). Om du väljer mer än en typ kan du ordna flera förfrågningar som kommer in.\
   Om du till exempel använder formuläret i en begärandekö för ett IT-projekt kan följande typer av begäranden placeras i kön: maskinvara, programvara, felkorrigeringar och problem.

   * **Standardvaraktighet:** Ange ett värde för Varaktighet och välj sedan en av följande varaktighetsenheter i listrutan:

      * Dagar
      * Timmar
      * Minuter
      * Veckor

   Standardlängden är den tid det normalt tar att slutföra ett problem som skickas till den här begärandekön. Detta blir standard för alla inkommande ärenden och kan ändras manuellt.
Standardlängden för ett problem är densamma som de planerade timmarna för problemet. Det planerade slutförandedatumet för problemet beräknas utifrån det här fältet.\
   Om det inte ändras är standardvärdet för problemets varaktighet 1 dag eller 8 timmar.
Om Workfront-administratören ställer in Normala timmar per arbetsdag till mindre än 8 timmar i inställningsområdet är standardvaraktigheten för utgåvor fortfarande 8 timmar.
Om t.ex. antalet timmar per arbetsdag är inställt på 7 timmar under Konfigurera i Workfront, är standardlängden för utgåvor 1,14 dagar eller 8 timmar.
Mer information om hur du ställer in systemet för beräkning av normaltimmar per arbetsdag finns i avsnittet &quot;Beräkningar av tidslinje&quot; i artikeln [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Personer från samma företag ärver samma behörigheter för alla begäranden.**: När du väljer det här alternativet visas alla begäranden som skickas till kön för användare i samma företag. Användare kan visa dessa begäranden i avsnittet Alla begäranden, som finns i området Begäranden. När den här inställningen är aktiverad eller inaktiverad påverkas alla framtida förfrågningar. Informationen påverkas inte retroaktivt.
   * **När någon gör en begäran, beviljar automatiskt...:** När en användare gör en begäran i kön, tilldelas användaren automatiskt den behörighetsnivå som du väljer för den begäran. Klicka på knappen Åtkomst för att välja mellan följande behörighetsnivåer:

      * **Visa åtkomst**
      * **Contribute Access**. Det här är standardinställningen och namnet på åtkomstknappen.
      * **Hantera åtkomst**

     Mer information om Workfront behörighetsmodell finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Genom att ange behörigheter här sparar du tid, i stället för att behöva tilldela behörigheter separat, för varje inkommande begäran. Om du väljer det här alternativet påverkas alla framtida förfrågningar, men befintliga förfrågningar påverkas inte retroaktivt.

   * **Standardgodkännande**: Klicka på listrutan för att välja en godkännandeprocess för den här begärandekön. Endast godkännandeprocesser för problem visas i den här listrutan. Alla utleveranser som skickas till den här kön kommer att associeras med den här godkännandeprocessen. Workfront-administratören måste definiera godkännandeprocesser på systemnivå innan du kan koppla dem till begärandeköer. Användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser.

     >[!IMPORTANT]
     >
     >Om projektgruppen ändras blir den gruppspecifika godkännandeprocess som är kopplad till befintliga utgåvor en godkännandeprocess för engångsbruk. Mer information om hur ändringar i projektgruppen eller ändringar i godkännandeprocessen påverkar godkännandeinställningarna finns i [Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Om du har flera köämnen associerade med en begärandekö rekommenderar vi att du i stället kopplar godkännandeprocesser till köämnena.

     Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Tänk på följande när du lägger till godkännandeprocesser i begärandeköer:

      * Endast aktiva godkännandeprocesser visas i listan.
      * Godkännandeprocesserna för systemomfattande och gruppspecifika problem visas i listan. En godkännandeprocess som är associerad med en annan grupp än den som projektet har visas inte i listan.

   * **Standardflöde**: Klicka på den nedrullningsbara menyn för att välja en routningsregel för den här begärandekön. Routningsregler tilldelar automatiskt nya utgåvor som skickas till en begärandekö till rätt resurs (användare, jobbroll eller team) och till rätt projekt. Alla utleveranser som skickas till den här kön kopplas till den här routningsregeln. Du måste konfigurera routningsregler innan de visas i avsnittet Köinformation och innan du kan associera dem med begärandekön.\
     Om du har flera köämnen som är associerade med en frågekö rekommenderar vi att du i stället kopplar routningsregler till köämnena. Mer information om hur du skapar routningsregler finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nya fält för problem:** I avsnittet **Visa följande markerade fält för alla användare** markerar du de fält som du vill ska vara synliga för alla användare som skickar en begäran till projektet eller lägger till ett problem i det här projektet eller i projektets aktiviteter.

     >[!NOTE]
     >
     >* När du aktiverar något av fälten Tilldelad till, Jobbroll eller Team, får de alltid nya namn till Uppdrag i formuläret när användarna skickar begäran. Du kan bara ange typen av tilldelning i området Köinformation.
     >
     >* Om du markerade Tilldelad till i området Köinformation kan du bara ange användare i fältet Uppdrag i formuläret för begäran. I det här fallet kan du inte ange jobbroller eller ett team.

   * **Dokument**: Välj det här alternativet om du vill visa avsnittet Dokument i det nya begärandeformuläret, och välj sedan var avsnittet för dokumentöverföring ska placeras. Välj bland följande:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Efter anpassade formulär</td> 
        <td><span>Avsnittet Dokument visas längst ned i formuläret för begäran.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Före anpassade formulär</td> 
        <td> <p><span>Avsnittet Dokument visas mellan Workfront-fälten och de anpassade fälten i det begärda formuläret.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Nya utgivningsfält och dokument i köinformation](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **Visa alla markerade och omarkerade fält till:** Välj vilka användare som ska se alla fält i det nya begärandeformuläret. Följande alternativ styr åtkomsten till fälten i formuläret.

     | Vilka användare som kan se alla fält i det begärda formuläret | Beskrivning |
     |---|---| 
     | Alla användare (Planera licenser) | Alla användare som har en planlicens kan se både det markerade och de omarkerade fälten. |
     | Personer med visningsåtkomst till det här projektet (planlicens) | De användare som har en planlicens som även har visningsbehörighet för det här projektet kan se både det valda och de omarkerade fälten. Resten av användarna som kan skicka begäranden till det här projektet kan se endast de valda fälten. |
     | Inga användare | Inga användare kan se de omarkerade fälten. Alla användare som kan skicka begäranden till det här projektet kan bara se de markerade fälten. Det här är standardvalet. |

   * **Anpassad Forms**: Välj ett anpassat formulär som ska associeras med begärandekön i listrutan. Du kan markera flera formulär och sedan dra och släppa dem i den ordning som du vill att de ska visas i formuläret för begäran.
Det går bara att välja anpassade formulär från den här listrutan. Alla utleveranser som skickas till den här begärandekön, som läggs till i projektet eller i dess uppgifter, kommer att ha de valda formulären kopplade till sig.
Du måste skapa anpassade formulär innan du kan se dem i avsnittet Köinformation.
Om du har flera köämnen som är associerade med en frågekö rekommenderar vi att du i stället kopplar anpassade formulär till köämnena.
Mer information finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Rutan Anpassade formulär i Köinformation](assets/custom-forms-box-on-queue-details.png)

1. Fortsätt att välja information för inställningarna i området **Inställningar för e-postkö** så att användare kan skicka begäranden via e-post till begärandeköprojektet.

   Mer information finns i [Gör det möjligt för användare att skicka ett problem via e-post till ett begärandeköprojekt](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Klicka på **Spara**.\
   Ditt projekt har nu konfigurerats som en frågekö och användare kan nu lägga till begäranden i det.

1. (Valfritt) Om du vill förbättra funktionen för begärandekö skapar du ytterligare underavsnitt för kön samt regler som dirigerar inkommande begäranden till rätt team, uppdragsgivare eller projekt.

   * Mer information om hur du skapar underavsnitt för begärandekön finns i följande artiklar
   * [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

     Mer information om hur du dirigerar begäranden till lämplig tilldelare, team och lämpligt projekt finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

</div>
