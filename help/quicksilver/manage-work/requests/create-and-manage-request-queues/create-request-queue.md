---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Skapa en begärandekö
description: Du kan skapa en frågekö där användare kan ange tillfälliga begäranden som inte är planerade för ett projekt.
author: Alina
feature: Work Management
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '2551'
ht-degree: 0%

---

# Skapa en begärandekö

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

Du kan skapa en frågekö där användare kan ange tillfälliga begäranden som inte är planerade för ett projekt. En kö för helpdesk-begäran kan till exempel ställas in för att samla in alla användarförfrågningar som kommer till en IT-avdelning.

## Åtkomstkrav

<!--drafted for P&P: replace the table below with this:

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
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Hantera behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har

## Översikt över köer för begäranden

Du ställer in en begärandekö som ett projekt. När du anger projektet som en frågekö blir kön tillgänglig från området med förfrågningar i Adobe Workfront. När du anpassar begärandekön anpassar du också de formuläranvändare som fyller i när de skickar förfrågningarna.

I den här artikeln beskrivs hur du skapar en begärandekö från ett befintligt projekt. För att skapa en konsekvent process för inhämtning av begäranden eller för att lägga till flera lager i den för rapportering och bättre hantering, kan du även konfigurera ytterligare byggstenar i en begärandekö som beskrivs i följande tabell.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Köinformation</td> 
   <td> <p>Du måste konfigurera ett projekt som en begärandekö i området Köinformation. Detta steg är obligatoriskt. </p> <p>Mer information finns i <a href="#create-a-request-queue" class="MCXref xref">Skapa en begärandekö</a> i den här artikeln.</p> </td> 
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

När du ställer in ett projekt som en frågekö måste projektstatusen vara Aktuell för att kunna visas i området Begäranden i Workfront.

Så här skapar du en begärandekö:

1. Gå till det projekt som du vill konfigurera som en frågekö.
1. (Valfritt) Klicka på **Projektinformation** i den vänstra panelen och lägga till en **Beskrivning** till projektet i **Översikt** område. Den här informationen visas för alla nya begäranden.
1. Klicka **Köinformation** i den vänstra panelen. Du kan behöva klicka **Visa fler** sedan **Köinformation**.

   Då öppnas avsnittet Köinformation.

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Ange följande information:

   * **Publicera som kö för hjälpbegäran:** Välj det här alternativet om du vill identifiera det här projektet som en begärandekö. Alla inkommande problem betraktas som begäranden.\
      När det här alternativet inte är markerat fungerar projektet som ett standardprojekt i Workfront och alla inkommande problem är problem.

   * **Vem kan lägga till begäranden i den här kön?** Välj vilka användare som har åtkomst att lägga till begäranden i den här kön. Du kan tillåta följande grupper av personer att se begärandekön i området Förfrågningar i det globala navigeringsfältet:

      | Alla | Alla Workfront-användare med ett aktivt konto kan visa den här begärandekön och lägga till begäranden i den |
      |---|---|
      | Personer med visningsåtkomst till det här projektet | Användare med behörigheten Visa i projektet kan visa och lägga till begäranden i den här kön |
      | Personer i det här projektets företag | Användare som tillhör det företag som är associerat med det här projektet kan visa och lägga till begäranden i den här kön. Om det finns ett företag som är associerat med projektet visas företagets namn inom parentes efter den här inställningen. |
      | Personer i det här projektets grupp | Användare som tillhör gruppen som är kopplad till det här projektet kan visa och lägga till begäranden i den här kön. Om det finns en grupp som är associerad med projektet visas gruppens namn inom parentes efter den här inställningen. |

      {style=&quot;table-layout:auto&quot;}

   * **Dela med dessa länkar:** Med följande alternativ kan du ge direktåtkomst till begärandekön och de formulär som är kopplade till den till användare utanför Workfront eller till Workfront-användare via en extern sida. Mer information om hur du bäddar in en begärandekö i en instrumentpanel som en extern sida finns i [Bädda in en begärandekö i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

      Användarna måste redan ha åtkomstbehörighet till begärandekön för att få direkt åtkomst. Om du använder något av de alternativ som beskrivs här beviljas inte automatiskt åtkomst till användare.

      >[!TIP]
      >
      >Användarna måste först logga in på Workfront innan de får åtkomst till kön när de öppnar sidan Begärandekö från ett annat program.

      * **URL för direktåtkomst:** När en användare öppnar den här URL:en från en webbläsare, dirigeras användaren direkt till avsnittet Ny begäran i området Begäranden och denna begäran väljs som standard för dem.

         ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

         >[!NOTE]
         >
         >Du kan visa en frågekö i en instrumentpanel som en extern sida. I det här fallet är begärandekön förvald, men du kan välja vilken annan begärandekö som helst från fältet Typ av begäran. -användare kan ändra frågetypen. Navigeringskomponenterna för begäranden visas också.

      * **Bädda in kod:** Använd den här HTML-koden för att bädda in formuläret för begärandekön som en iframe på en HTML-sida.\
         Om användare inte redan är autentiserade i Workfront när de visar sidan där koden är inbäddad, visas inloggningsdialogrutan för Workfront. När användarna har loggat in visas formuläret Begärandekö.

         ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

         >[!NOTE]
         När du visar en begärandekö i en iframe visas endast begärandeformuläret, begärandenamnet är förmarkerat och nedtonat. Användaren kan inte ändra typen för begäran. Navigeringskomponenterna i området Begäranden visas inte.

         För att formuläret för begärandekön ska kunna visas när du använder den här inbäddningskoden måste du aktivera inställningen&quot;Tillåt inbäddning av Workfront i en iframe&quot; i systeminställningarna. Mer information om hur du aktiverar inbäddning av Workfront i en iframe finns i [Konfigurera säkerhetsinställningar för system](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Om den här inställningen inte är aktiverad visas iframe-elementet som tomt.

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
           <td> <p>Ändra attributen "width" och "height".</p> <p>Som standard är bredden"500" och höjden"600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direktanvändare till en viss ämnesgrupp eller ämnesgrupp i kön</p> </td> 
           <td> <p>Lägg till parametern "path" i src-URL:en. Du kan hitta parametern path genom att navigera till önskad köämnesgrupp eller ämnesgrupp i det ej inbäddade formuläret och kontrollera URL:en.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Visa och tillåt användare att ändra den förkonfigurerade listrutan Ämnesgrupp</p> </td> 
           <td> <p>Använd parametern "path" genom att lägga till <code>showPreSelectedOptions=true</code> parametern till <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Identifiera när formuläret har skickats</p> </td> 
           <td> <p>Lägg till en meddelandehändelseavlyssnare i webbsidans fönster och kontrollera om <code>event.data.type</code> är <code>requestSubmitted</code>. <code>event.data.newIssueID</code> ställs in på ID:t för den skapade utgåvan.</p> </td> 
          </tr> 
         </tbody> 
        </table>
   * **Typ av begäran:** Välj bland standardalternativen nedan.

      Workfront-administratören kan byta namn på standardförfrågningstyperna. Mer information om hur du byter namn på typer av begäranden finns i [Anpassa standardproblemtyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Ändra ordning
      * Problem
      * Begäranden
      * risk

         Detta är ett obligatoriskt fält och du måste välja minst ett alternativ.
      >[!NOTE]
      Begärantyper visas bara som ett urval i området Förfrågningar om frågetypen har valts både på sidorna Köinformation och på sidorna Köämne. Mer information om hur du ställer in området Köinformation för ett projekt finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Alla typer som markeras här är tillgängliga i formuläret (du kan markera flera). Om du väljer mer än en typ kan du ordna flera förfrågningar som kommer in.\
      Om du till exempel använder formuläret i en begärandekö för ett IT-projekt kan följande typer av begäranden placeras i kön: maskinvara, programvara, felkorrigeringar och problem.

   * **Standardvaraktighet:** Standardlängden är den tid det normalt tar att slutföra ett problem. Detta blir standard för alla inkommande ärenden och kan ändras manuellt. Varaktigheten anges vanligtvis i timmar, dagar eller veckor. Standardlängden för ett problem är densamma som de planerade timmarna för problemet. Det planerade slutförandedatumet för problemet beräknas utifrån det här fältet.\
      Standardvärdet för utfärdandevaraktighet är 1 dag eller 8 timmar. Om Workfront-administratören ställer in Normal timma per arbetsdag till mindre än 8 timmar är standardvaraktigheten för utgåvor fortfarande 8 timmar. Om t.ex. antalet timmar per arbetsdag är 7 timmar är standardlängden för utleveranser 1,14 dagar eller 8 timmar. Mer information om hur du ställer in systemet för beräkning av normaltimmar per arbetsdag finns i avsnittet &quot;Beräkningar av tidslinje&quot; i artikeln [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Personer från samma företag ärver samma behörigheter för alla begäranden.:** När du väljer det här alternativet visas alla begäranden som skickas till kön för användare i samma företag. Användare kan visa dessa begäranden i avsnittet Alla begäranden, som finns i området Begäranden. När denna inställning är aktiverad eller inaktiverad påverkas alla framtida förfrågningar. inte retroaktivt påverkar informationen.
   * **När någon gör en förfrågan tilldelar automatiskt** När en användare gör en begäran i kön med begäranden, tilldelas användaren automatiskt den behörighetsnivå som du väljer för den begäran. Välj bland följande behörighetsnivåer:\
      **- Visa**

      **- Contribute**
      **- Hantera**

      Mer information om Workfront behörighetsmodell finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
      Om du anger behörigheter här sparar du tid i stället för att behöva bevilja behörigheter för varje enskild inkommande begäran. Om du väljer det här alternativet påverkas alla framtida förfrågningar, men befintliga förfrågningar påverkas inte retroaktivt.

   * **Standardgodkännande**: Associera en godkännandeprocess med den här begärandekön. Endast godkännandeprocesser för problem visas i den här listrutan. Alla utleveranser som skickas till den här kön kommer att associeras med den här godkännandeprocessen. Workfront-administratören måste definiera godkännandeprocesser på systemnivå innan du kan koppla dem till begärandeköer. Användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser.

      >[!IMPORTANT]
      Om projektgruppen ändras blir den gruppspecifika godkännandeprocess som är kopplad till befintliga utgåvor en godkännandeprocess för engångsbruk. Mer information om hur ändringar i projektgruppen eller i godkännandeprocessen påverkar godkännandeinställningarna finns i [Hur ändringar i gruppering och godkännandeprocess påverkar tilldelade godkännandeprocesser](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

      Om du har flera köämnen associerade med en begärandekö rekommenderar vi att du i stället kopplar godkännandeprocesser till köämnena. Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Tänk på följande när du lägger till godkännandeprocesser i begärandeköer:

      * Endast aktiva godkännandeprocesser visas i listan.
      * Systemomfattande och gruppspecifika godkännandeprocesser visas i listan. En godkännandeprocess som är associerad med en annan grupp än den som projektet har visas inte i listan.
   * **Standardflöde**: Associera en routningsregel med den här begärandekön. Använd routningsregler för att automatiskt tilldela nya ärenden som skickas till en begärandekö till rätt resurs (användare, jobbroll eller team) och till rätt projekt. Alla utleveranser som skickas till den här kön kommer att associeras med den här routningsregeln. Du måste konfigurera routningsregler innan du kan associera dem med begärandekön.\
      Om du har flera köämnen som är associerade med en frågekö rekommenderar vi att du i stället kopplar routningsregler till köämnena. Mer information om hur du skapar routningsregler finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nya fält:** I avsnittet Visa följande markerade fält för alla användare väljer du de fält som du vill ska vara synliga för alla användare som skickar en begäran till projektet eller lägger till ett problem i projektet eller aktiviteterna.

      >[!TIP]
      Nya fält för ärenden som har valts i avsnittet Köinformation är också kopplade till nya problem som har lagts till i projektet eller till uppgifterna i avsnittet Problem.

      När du aktiverar något av fälten Tilldelad till, Jobbroll eller Team ändras alltid namnen till Tilldelningar i formuläret för begäran, men du kan bara ange vilken typ av uppdrag som har valts här.

      **Exempel:** Om du markerade Tilldelad till i området Köinformation kan du bara ange användare i fältet Uppdrag i formuläret för begäran. I det här fallet kan du inte ange jobbroller eller ett team.

   * **Dokument**: Om du väljer att visa avsnittet Dokument i det nya formuläret för begäran, ska du välja var avsnittet för dokumentöverföring ska placeras. Välj bland följande:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Efter anpassade formulär</td> 
        <td><span>Avsnittet Dokument visas längst ned i formuläret.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Före anpassade formulär</td> 
        <td> <p><span>Avsnittet Dokument visas mellan Workfront-fälten och de anpassade fälten i det begärda formuläret.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

      ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Visa alla markerade och omarkerade fält till:** Välj vilka användare du vill visa alla fält i formuläret. Följande alternativ styr åtkomsten till fälten i formuläret.

      | Alla användare (Planera licenser) | Alla användare som har en planlicens kan se både det markerade och de omarkerade fälten. |
      |---|---|
      | Personer med visningsåtkomst till det här projektet (planlicens) | De användare som har en planlicens som även har visningsbehörighet för det här projektet kan se både det valda och de omarkerade fälten. Resten av användarna som kan skicka begäranden till det här projektet kan se endast de valda fälten. |
      | Inga användare | Inga användare kan se de omarkerade fälten. Alla användare som kan skicka begäranden till det här projektet kan bara se de markerade fälten. |

      {style=&quot;table-layout:auto&quot;}

   * **Anpassad Forms**: Välj ett anpassat formulär som ska associeras med begärandekön. Det är bara Issue Custom Forms (Utforma anpassad) som du kan välja i den här listrutan. Alla utleveranser som skickas till begärandekön har de valda formulären kopplade till sig.\
      Om du har flera köämnen kopplade till en frågekö rekommenderar vi att du i stället kopplar anpassade formulär till köämnen. Mer information om hur du skapar underavsnitt för begärandekön finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Om du har flera anpassade formulär kopplade till frågekö drar och släpper du formulären för att sortera dem i önskad ordning i dialogrutan **Ändra ordning på Forms** -avsnitt.

      >[!TIP]
      Anpassade formulär som läggs till i avsnittet Köinformation associeras också med eventuella nya problem som läggs till i projektet eller aktiviteterna i avsnittet Problem.

   * **Tillåt att ärenden läggs till via e-post:** Välj det här alternativet om du vill tillåta att begäranden skickas via e-post.\
      Mer information finns i [Gör det möjligt för användare att skicka ett ärende via e-post till ett begärandeköprojekt](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).




1. Klicka **Spara**.\
   Ditt projekt har nu konfigurerats som en frågekö och användare kan nu lägga till begäranden i det.

1. (Valfritt) Om du vill förbättra funktionen för begärandekö skapar du ytterligare underavsnitt för kön samt regler som dirigerar inkommande begäranden till rätt team, uppdragsgivare eller projekt.

   Mer information om hur du skapar underavsnitt för begärandekön finns i artiklarna [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) och [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).\
   Mer information om hur du dirigerar begäranden till lämplig uppdragstagare, team och lämpligt projekt finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
