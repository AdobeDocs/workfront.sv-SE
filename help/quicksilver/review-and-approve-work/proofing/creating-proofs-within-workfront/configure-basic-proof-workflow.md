---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Skapa ett avancerat korrektur med ett grundläggande arbetsflöde
description: Med ett grundläggande arbetsflöde kan du skicka flera granskare till ett korrektur, men de är inte ordnade i steg. Alla granskare som du lägger till får tillgång till korrekturet direkt när du har skapat det.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1793'
ht-degree: 0%

---

# Skapa ett avancerat korrektur med ett grundläggande arbetsflöde

<!-- Audited: 1/2024 -->

Med ett grundläggande arbetsflöde kan du skicka flera granskare till ett korrektur, men de är inte ordnade i steg. Alla granskare som du lägger till får tillgång till korrekturet direkt när du har skapat det.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>
   <p>Alla</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
    <p>Arbete eller plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett avancerat korrektur med ett grundläggande arbetsflöde

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på fliken **Dokument** .
1. Klicka på **Lägg till nytt** > Korrektur, ladda upp innehållet och arbeta sedan igenom avsnitten nedan.

   eller

   Håll muspekaren över ett befintligt dokument, klicka på **Skapa korrektur** > **Avancerat korrektur** och gå igenom avsnitten nedan.

## Konfigurera arbetsflödet och lägga till granskare

1. Välj **Grundläggande** i avsnittet Arbetsflödestyp.
1. Ange vilka användare du vill lägga till och välj sedan en korrekturroll.

   ![Nya korrekturroller](assets/new-proof---roles-350x213.png)

1. I följande tabell visas varje roll och de rättigheter som är kopplade till den.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>Visa ett bevis</strong> </p> </th> 
      <th> <p><strong>Lägg till markeringar</strong> </p> </th> 
      <th> <p><strong>Lägg till kommentarer</strong> </p> </th> 
      <th> <p><strong>Redigera egna kommentarer om det inte finns några svar</strong> </p> </th> 
      <th> <p><strong>Fatta ett beslut</strong> </p> </th> 
      <th> <p><strong>Ta bort kommentarer från andra</strong> </p> </th> 
      <th>Lös kommentarer</th> 
      <th>Tillämpa åtgärder på kommentarer</th> 
      <th> <p><strong>Redigera korrekturet</strong> </p> </th> 
      <th>Dela korrekturet med andra</th> 
      <th>Skapa ny version</th> 
      <th> <p><strong>Visa godkännandebegäranden i hemområdet</strong> </p> </th> 
      <th>Lägg till nya granskare</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Skrivskyddad</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Granskare</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Godkännare</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Granskare och godkännare</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Författare</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Moderator</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong> ✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. Användare med nya Workfront-planer kan tilldela författare eller moderatorroller till alla användare i systemet. Användare med äldre planer kan tilldela författare eller moderatorroller till alla användare som har en korrekturlicens i systemet.
1. (Valfritt) Med rullgardinsmenyn fortfarande öppen väljer du eventuella ytterligare behörigheter längst ned på menyn:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lösa kommentarer och tillämpa åtgärder </td> 
      <td> <p>Gör att Workfront-användaren kan göra följande:</p> 
       <ul> 
        <li>Lös en kommentar när den har adresserats, vilket förklaras i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Lös korrekturkommentarer</a>.</li> 
        <li>Tillämpa åtgärder på kommentarer enligt beskrivningen i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Använd åtgärder på korrekturkommentarer</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela korrektur genom att tagga</td> 
      <td> <p>Låter granskaren lägga till valfri Workfront-användare i korrekturet enligt beskrivningen i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Tagga användare för att dela ett korrektur</a>.</p> <p>Obs!  <p>Om de här två alternativen inte är tillgängliga (nedtonade) har användaren redan en behörighetsprofil som gör det möjligt att lösa kommentarer, tillämpa åtgärder på kommentarer och tagga användare. </p> <p>Om alternativen inte visas är den person du har lagt till inte licensinnehavare för Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Upprepa steg 1-3 för alla andra användare som du har lagt till i korrekturet.
1. För varje användare som du delar med väljer du i den nedrullningsbara listan **E-postaviseringar** vilken typ av e-postaviseringar som användaren får när han/hon gör kommentarer och fattar beslut om korrekturet:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alla aktiviteter</td> 
      <td>Workfront skickar ett e-postmeddelande till granskaren varje gång det finns någon aktivitet i korrekturet, t.ex. en ny kommentar, ett svar eller ett beslut. <p>Detta är ett bra alternativ för den som hanterar korrekturläsningen eftersom det gör att personen kan se aktiviteten som den är. </p><p>Användarna får ingen e-postavisering om sin egen aktivitet.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Svar på mina kommentarer</td> 
      <td>Ett e-postmeddelande skickas till granskaren endast om någon uttryckligen svarar på kommentaren (detta utesluter att personen själv svarar på sina kommentarer). Det innebär att om någon i korrekturet gör en ny kommentar så meddelas inte granskaren.<p>Den här inställningen rekommenderas för dina kunder på korrekturet så att de inte meddelas om några andra kommentarer på korrekturet och endast får svar på sina egna kommentarer.</p><p>Även om granskare med den här e-postaviseringsinställningen inte meddelas om andra nya kommentarer, kan de fortfarande visa alla kommentarer i korrekturläsaren.</p><p>Mer information om kommentarer finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visa och svara på korrekturkommentarer</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beslut</td> 
      <td>Workfront skickar ett e-postmeddelande till granskaren endast när någon fattar ett beslut.<p>Detta kan vara användbart för den som hanterar godkännandeprocessen (t.ex. en projektledare) och måste övervaka korrekturets förlopp och se vilka användare som har fattat sitt beslut.</p><p>Du meddelas inte om ditt eget beslut såvida du inte väljer ett bekräftelsealternativ för e-post när du skickar ditt beslut.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Slutgiltigt beslut</td> 
      <td>Workfront skickar ett e-postmeddelande när den sista godkännaren har fattat sitt beslut.<p>Den här varningen används ofta av designern som vanligtvis inte behöver delta i själva granskningsdiskussionen. När det slutliga beslutet fattas meddelas formgivaren och kan sedan vidta eventuella nödvändiga åtgärder.</p><p>Den här varningen kan även vara användbar för en avdelningsledare som behöver få ett meddelande endast när granskningsprocessen är klar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sammanfattning varje timme</td> 
      <td>Workfront skickar ett mejl till granskaren varje timme med en sammanfattning av alla kommentarer, svar och beslut som har fattats.<p>E-postmeddelandet skickas bara när andra aktiviteter än din egen inträffar under den senaste timmen. </p><p>Den här varningen är ett bra sätt att se en översikt över projektet.</p><p>Ett exempel på hur man kan använda den här sammanfattningen är en erfaren granskare som behöver en översikt över projektet, men som inte behöver underrättas omedelbart om all aktivitet på beviset.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Daglig sammanfattning</td> 
      <td>Workfront skickar ett e-postmeddelande med alla kommentarer, svar och beslut listade endast dagar när det finns någon aktivitet utöver din egen.<p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.</p><p>Ett exempel på hur den här sammanfattningen används är en avdelningsledare som vill övervaka projektets övergripande förlopp.</p><p>Mer information finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Hantera meddelanden om korrekturkommentarer och beslut</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ingen e-post</td> 
      <td>Workfront skickar inga e-postaviseringar.<br>Det här är användbart för en person som bara läggs till i ett korrektur för referens och som inte behöver informeras om några ändringar.<p>Systemets standardvärde är Daglig sammanfattning (visas också som Inte angivet). Om du eller dina granskare inte gör några andra ändringar har alla dina korrektur den här inställningen.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt med [Konfigurera e-postinställningar för korrekturet](#configure-email-settings-for-the-proof) nedan.

## Konfigurera e-postinställningar för korrekturet {#configure-email-settings-for-the-proof}

1. I avsnittet **E-postmeddelande** väljer du om du vill skicka e-postmeddelanden och ett anpassat meddelande till de användare du valde i [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](#workflow) tidigare i den här artikeln:

   <table>
   <tbody>
   <tr>
   <td>Meddela mottagarna om det här beviset</td>
   <td>Välj det här alternativet om du vill skicka ett e-postmeddelande till användarna. När <strong>Grundläggande delning</strong> har valts i avsnittet <strong>Arbetsflöde</strong> skickas ett e-postmeddelande när korrekturet skapas. När <strong>Automatiskt arbetsflöde</strong> har valts i avsnittet <strong>Arbetsflöde</strong> skickas ett e-postmeddelande när korrekturet kommer in i det automatiserade arbetsflöde som användaren är kopplad till.</td>
   </tr>
   <tr>
   <td>Lägg till anpassat meddelande</td>
   <td>Välj det här alternativet om du vill inkludera ett anpassat meddelande i meddelandet. Du kan ange ämne och meddelandetext. Meddelandetexten kan innehålla formaterad text, t.ex. fet stil, punkter och hyperlänkar.</td>
   </tr>
   </tbody>
   </table>


1. Fortsätt med [Konfigurera korrekturinställningar](#configure-proof-settings) nedan.

## Konfigurera korrekturinställningar {#configure-proof-settings}

1. Välj något av följande alternativ i avsnittet **Korrekturinställningar**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kräv inloggning - korrektur kan bara delas med andra användare</td> 
      <td>När det här alternativet är inaktiverat (standard) kan alla med URL-adressen visa korrekturet. <br>När det här alternativet är markerat:
       <ul>
        <li>Endast Workfront Proof-användare kan visa korrekturet.</li>
        <li>Användarna kan inte logga in på korrekturet om de inte har lagts till i korrekturet.</li>
        <li>Det går inte att aktivera prenumerationer.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endast ett beslut krävs för det här beviset</td> 
      <td>När det här alternativet har valts slutförs granskningen efter det att en av beslutsfattarna har fattat sitt beslut.<br>Det här alternativet är inaktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kräv att beslut signeras elektroniskt</td> 
      <td>Användarna måste ange sitt användarnamn och lösenord när de fattar beslut om ett korrektur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås korrektur när alla nödvändiga beslut har fattats</td> 
      <td>När den här inställningen är aktiverad låses korrekturläget när alla beslut har fattats. Läget ändras automatiskt från olåst till låst när den slutliga godkännaren fattar sitt beslut.<br>Det här alternativet är inaktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hämta originalfil</td> 
      <td>När det här alternativet är markerat kan granskarna hämta originalfilen som korrekturet skapades från.<br>När det här alternativet är avmarkerat visas inte längre hämtningsikonen.<br>Det här alternativet är aktiverat som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela korrektur via offentlig URL eller inbäddningskod</td> 
      <td>När det här alternativet är markerat kan korrekturet delas via en offentlig URL eller inbäddningskod.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prenumerera på korrektur via offentlig URL eller inbäddningskod</td> 
      <td>När det här alternativet är markerat kan personer som inte har lagts till explicit i korrekturet prenumerera på korrekturet. Den person som prenumererar på beviset får rollen och e-postadressen som du anger i följande inställningar:
       <ul>
        <li><strong>Prenumerantroll:</strong> Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet. </li>
        <li><strong>E-postaviseringsinställningar för prenumeranter:</strong> Standardaviseringen för e-post som tilldelas alla granskare som prenumererar på korrekturet.</li>
       </ul><p>
        <ul>
         <li><strong>Åtkomst via e-postlänk krävs för:</strong> Konfigurera om prenumeranten får ett e-postmeddelande med en länk till korrekturet. Du kan välja <strong>Inget e-postmeddelande</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>E-postmeddelande för korrektur endast</strong> (prenumeranten får en länk till korrekturet via e-post utan någon verifiering) eller <strong>E-postmeddelanden för validering och korrekturet </strong> (prenumeranten får en länk till korrekturet och måste klicka på ett bevis. Syftet med det här alternativet är att se till personen har angett korrekt e-postadress som de har tillgång till).</li>
        </ul><p>Obs!  Om korrekturet har ett automatiserat arbetsflöde bifogat, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägarna, så att de kan bestämma i vilken fas personen ska läggas till.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Skapa bevis**.

   Workfront börjar generera ett korrektur av de valda dokumenten eller webbplatserna. Beroende på filstorlek och typ kan fördröjningen för en dokumentöverföring variera. Ha tålamod när större filer tar längre tid att generera. Du kan navigera bort från sidan och Workfront fortsätter att generera filen. Den maximala filöverföringsstorleken är 4 GB.

1. När korrekturet har skapats klickar du på **Öppna korrektur** för att starta korrekturläsaren.

   ![Öppna korrektur](assets/open-proof-350x132.png)

   Användare som inte har språkkontroll aktiverat på sitt konto kan fortfarande visa dokumentet och kommentera korrekturet.
