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
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '2799'
ht-degree: 0%

---


# Skapa en begärandekö

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--remove/ hide the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   

-->

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

<!-- 

Creating a request queue differs depending on what environment you use. 

### Create a Request Queue in the Production environment

This section describes how you can define Queue Details for the following objects:

* A project in the Production environment
* A template in the Production or Preview environment

-->

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

<!--

<div class="preview">

### Create a Request Queue in the Preview environment

When you set up a project as a Request Queue, the project status must be Current in order to display in the Requests area of Workfront.

>[!TIP]
>
>Your Workfront or group administrator might assign you to a custom Layout Template that might not include some of the sections described in the following steps.

To create a Request Queue:

1. Go to the project that you want to set up as a Request Queue.
1. (Optional) Click **Project Details** in the left panel and add a **Description** to the project in the **Overview** area. This information displays on all new requests.
1. Click **Queue Details** in the left panel. You might need to click **Show More**, then **Queue Details**.

   This opens the Queue Details section.

   ![Queue Type section in Queue Details area](assets/unshimmed-queue-type-section-queue-details-area.png)

1. Specify the following information:

   * **Publish as Help Request Queue**: Select this option to identify this project as a request queue. All incoming issues are considered Requests.  
     When this option is not selected, the project behaves like a standard project in Workfront and all incoming issues are issues.
   
   * **Who can add requests to this queue?**: Select which users have access to add requests to this queue. You can allow the following groups of people to see the Request Queue in their Requests area of the Global Navigation Bar when they add a new request:

     |Who can enter requests | Description|
     |---|---|
     | Anyone  |Any Workfront user with an active account can view this request queue and add requests to it |
     | People with view access to this project |Users with View permissions to the project can view and add requests to this queue |
     | People in this project's company |Users who belong to the company associated with this project can view and add requests to this queue. If there is a company associated with the project, the name of the company is listed in parentheses after this setting.  |
     | People in this project's group |Users who belong to the group associated with this project can view and add requests to this queue. If there is a group associated with the project, the name of the group is listed in parentheses after this setting, in gray font.  |

     {style="table-layout:auto"}

   * (*************removed: **Share with these links:** - asked Lusine if this stays***********) Use the following options to provide direct access to the Request Queue and the forms associated with it to users outside of Workfront or to Workfront users using an embedded external page. 
   
    For information about embedding a request queue in a dashboard as an external page, see [Embed a request queue in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Users must first have permissions to the Request Queue in order to gain direct access. Using either option described here does not automatically grant access to users.

     >[!TIP]
     >
     >Users must first log in to Workfront before gaining access to the request queue when they access the Request Queue page from another application.

      * **Direct Access URL:** When a user accesses this URL from a browser, the user is taken directly to the New Request  section in the Requests area and this request is selected by default for them.

        ![New request box from Direct URL share](assets/new-request-box-from-direct-url-share.png)

        >[!NOTE]
        >
        >You can display a Request Queue in a dashboard as an external page. In this case, the request queue is preselected, but you can select any other request queue from the Request Type field. Users submitting the request can select another Request Type. Topic Groups and Queue Topics also display.

      * **Embed Code:** Use this HTML code to embed the request queue form as an iframe within any HTML page.  
        If users are not already authenticated to Workfront when they view the page where the code is embedded, the Workfront login dialog box is displayed. After users log in, the Request Queue form is displayed.

        >[!NOTE]
        >
        >When displaying a Request Queue in an iframe, only the request form displays, the request name is preselected and dimmed. User cannot change the Request type. Navigation components of the Requests area do not display.

        In order for the request queue form to be displayed when using this embed code, your Workfront administrator must enable the "Allow embedding of Workfront in an iframe" setting in your system Setup area. 
        
        For more information about enabling embedding of Workfront in an iframe, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). If this setting is not enabled, the iframe is displayed as blank.

        You can adjust various aspects of how the embedded form is displayed, as follows:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Functionality</strong> </p> </th> 
           <th> <p><strong>Solution</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Adjust the size of the frame</p> </td> 
           <td> <p>Modify the "width" and "height" attributes.</p> <p>By default, the width is "500" and the height is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direct users to a specific Queue Topic or Topic Group</p> </td> 
           <td> <p>Add the "path" parameter to the src URL. You can find the path parameter by navigating to the desired Queue Topic or Topic Group in the non-embedded form and inspecting the URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Show and allow users to change the pre-configured Topic Group drop-down list</p> </td> 
           <td> <p>Use the "path" parameter by adding the <code>showPreSelectedOptions=true</code> parameter to the <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detect when the form has been submitted</p> </td> 
           <td> <p>Add a "message" event listener to your web page's window and checking if <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> will be set to the ID of the created issue.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Request Types:** In the **Queue Properties** section, select from the following options: 

      * Bug Report
      * Change Order
      * Issue
      * Request

      This is a required field and you must select at least one option.

      The Workfront administrator can rename the default request types. For more information about renaming the request types, see [Customize default issue types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).     

     >[!NOTE]
     >
     >When users access the request queue from the Requests area, the Request Types display as a selection only if the Request Type is selected in both the Queue Details and the Queue Topic pages. 
     >
     >For information about setting up the Queue Topics area of a project, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Each type selected here will be available on the form (you can select more than one). Selecting more than one type can help organize multiple requests coming in.  
     For example, if you are using the form on a request queue for an IT project, the following request types can come in to the queue: hardware, software, bug fixes, and issues.

   * **Default Duration:** Enter a number for the Duration, then select from the drop-down menu one of the following duration units:

      * Days
      * Hours
      * Minutes
      * Weeks
   
    The default duration is the length of time it typically takes to complete an issue submitted to this request queue. This becomes the default for all incoming issues and can be modified manually. 
    The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.  
    If left unchanged, the default for the issue Duration is 1 day or 8 hours. 
    If your Workfront administrator set the Typical Hours per Work Day as less than 8 hours in the Setup area, the Default Duration for issues is still 8 hours. 
    For example, if the Typical Hours per Work Day is set to 7 hours i the Setup area of Workfront, the Default Duration for issues is 1.14 Days or 8 hours. 
    For more information about how to set up the system Typical Hours per Work Day, see the "Timeline Calculations" section in the article [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
   
   * **People from the same company will inherit the same permissions for all requests.**: When selected, all requests submitted to the queue are visible for users in the same company. Users can view these requests in the All Requests  section , located within the Requests area. At the time that this setting is enabled or disabled, it impacts all future requests; it does not retroactively impact information. 
   * **When someone makes a request, automatically grant...:** When a user makes a request to the request queue, the user is automatically granted the level of permission that you choose to that request. Click the Access button to select from the following permissions levels: 

      * **View Access** 
      * **Contribute Access**. This is the default selection and the name of the Access button.
      * **Manage Access**

     For information about the Workfront permissions model, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).   
     Setting permissions here saves time, rather than having to grant permissions individually, for each incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests. 
   
   * **Default Approval**: Click the drop-down menu to select an approval process for this request queue. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this approval process. Your Workfront administrator must define system-level approval processes before you can associate them with request queues. Users with administrative access to Approval processes can also create group-specific approval processes.

     >[!IMPORTANT]
     >
     >If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see [How group and approval process changes affect assigned approval processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     If you have multiple queue topics associated with a request queue, we recommend that you associate approval processes with the queue topics instead. 
     
     For more information about creating queue topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md). 
   
     Consider the following when adding approval processes to request queues:

      * Only active issue approval processes display in the list. 
      * System-wide and group-specific issue approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.

   * **Default Route**: Click the drop-down menu to select a routing rule for this request queue. Routing rules automatically assign new issues submitted to a request queue to the correct resource (user, job role, or team), and to the correct project. All issues submitted to this queue will be associated with this routing rule. You must configure Routing Rules before they display in the Queue Details section and before you can associate them with request queue.  
     If you have multiple queue topics associated with a request queue, we recommend that you associate routing rules with the queue topics instead. For more information about creating routing rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
   
   * **New Issue Fields:** In the **Show the following selected fields to all users** section, select the fields that you want to be visible to all users who submit a request to the project or add an issue to this project or to the project's tasks.

      >[!NOTE]
      >
      >* When you enable any of the Assigned to, Job Role, or the Team fields, they are always renamed to Assignments in the request form when users submit the request. You can only specify the type of assignment in the Queue Details area. 
      >
      >* If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team. 
   
   * **Documents**: Select this option to display the Documents section in the new request form, then select where the document uploading section should be positioned. Select from the following:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">After custom forms</td> 
        <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Before custom forms</td> 
        <td> <p><span>The Documents section displays between the Workfront fields and the custom fields of the request form.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>   
   
     ![New issue fields and documents on Queue Details](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **Show all selected and unselected fields to:** Select which users should see all the fields on the new request form. The following options control the access to the fields on the form.
    
      |Which users can see all fields on the request form | Description|  
      |---|---| 
      | All Users (Plan Licenses) |All users who have a Plan license can see the selected as well as the unselected fields. |
      | People with view access to this project (Plan License) |Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields. |
      | No Users |No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected. This is the default selection. |
  
   * **Custom Forms**: Select a custom form to associate with the Request Queue from the drop-down menu. You can select multiple forms, then drag and drop them in the order you would like them to display in the request form. 
   Only issue custom forms are available to select from this drop-down menu. All issues submitted to this request queue, added to the project or to its tasks will have the selected forms associated with them. 
   You must create issue custom forms before you can see them displayed in the Queue Details section. 
   If you have multiple queue topics associated with a request queue, we recommend that you associate custom forms with the queue topics instead. 
   For more information, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Custom forms box on Queue Details](assets/custom-forms-box-on-queue-details.png)

1. Continue selecting information for the settings in the **Email Queue Settings** area, to allow users to email requests to the request queue project. 

    For more information, see [Enable users to email an issue into a Request Queue project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Click **Save**.  
   Your project has now been configured to be a Request Queue and users can now add requests to it. 

1. (Optional) To enhance the Request Queue functionality, build additional sub-sections for your queue, as well as rules to route the incoming requests to the correct team, assignee or project.

   * For information about creating sub-sections for the Request Queue, see the following articles
    * [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)  
    * [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).  
   
      For information about routing the requests to the appropriate assignee, team, and appropriate project, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).


</div>

-->