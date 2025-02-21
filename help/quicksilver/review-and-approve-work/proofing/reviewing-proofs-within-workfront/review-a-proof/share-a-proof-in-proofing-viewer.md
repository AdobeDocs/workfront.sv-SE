---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Dela ett korrektur från korrekturläsaren
description: Du kan dela ett korrektur från korrekturläsaren om delning har aktiverats av korrekturägaren eller den som skapat det.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 0%

---

# Dela ett korrektur från korrekturläsaren

Du kan dela ett korrektur från korrekturläsaren om delning har aktiverats av korrekturägaren eller den som skapat det.

>[!IMPORTANT]
>
>Inställningen Tillåt delning av korrektur via offentlig URL eller inbäddningskod måste vara aktiverad.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Dela URL

Du kan dela ett korrektur via en URL om ägaren har konfigurerat korrekturet för delning. Korrekturägare kan uppdatera delningsinställningarna när som helst. Mer information finns i [Redigera korrekturinställningar](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Om den vänstra ikonmenyn inte visas klickar du på ikonen **Meny** i det övre vänstra hörnet i korrekturläsaren.

   ![Menyikon](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Klicka på ikonen **Dela** i den vänstra ikonmenyn i korrekturläsaren.

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. Kontrollera att **Hämta delbar länk** är markerat i alternativen för **Dela korrektur** som visas.

1.  Gör något av följande:

   * Om du vill kopiera länken till Urklipp klickar du på **Kopiera länk**.

     Nu kan du distribuera länken via ett verktyg från tredje part, som en chatt eller ett e-postprogram.

   * Så här skickar du länken direkt från Adobe Workfront:

      1. I fältet **Eller e-postlänk till** börjar du skriva och väljer namnet på mottagaren. Eller ange e-postadressen till en extern användare som du vill dela med.

         >[!NOTE]
         >
         >Om du ser ett alias-e-postmeddelande när du delar ett korrektur ska du inte skapa en ny gästanvändare genom att ange det ursprungliga e-postmeddelandet om det finns ett motsvarande alias-e-postmeddelande.

      1. Välj bland följande alternativ:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Skicka offentlig länk</td>
            <td><p>Inkluderar en knapp i e-postmeddelandet som dirigerar användare till korrekturet i det korrekturläsare som de använder och beviljar visningsåtkomst.</p><p>Om <strong>Prenumerera på korrektur via offentlig URL eller inbäddningskod</strong> är inaktiverat för korrekturet kan användare logga in med sina inloggningsuppgifter för Workfront för att lägga till kommentarer i korrekturet. Om det är aktiverat kan alla som anger sin e-postadress och sitt namn (inget lösenord krävs) signera och lägga till kommentarer i korrekturet.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Skicka nedladdningslänk</td>
            <td>Innehåller en knapp i e-postmeddelandet som dirigerar användare till en hämtningssida med filinformation, filnamn och filstorlek, med filen textbunden. Användarna kan klicka på länken Hämta på nedladdningssidan för att hämta filen.</td>
           </tr>
           <tr>
            <td role="rowheader">Lägg till anpassat meddelande</td>
            <td>Gör att du kan ange ett eget ämne och brödtext för e-postmeddelandet.</td>
           </tr>
          </tbody>
         </table>

      1. Klicka på **Skicka**.

         Mottagarna får ett e-postmeddelande med information om det korrektur och de knappar du valt att inkludera.

         ![](assets/proof-share-email-350x87.png)

## Dela inbäddningskoden

Du kan dela ett korrektur via inbäddningskod om korrekturägaren har konfigurerat det för detta.

Så här delar du ett korrektur via inbäddningskoden:

1. Klicka på ikonen **Dela** i verktygsfältet till vänster om korrekturläsaren.

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. Klicka på **Hämta inbäddningskod** i de **Dela korrektur** som visas och klicka sedan på **Kopiera**.

## Dela ett korrektur genom att lägga till användare

Du kan lägga till användare i ett korrektur när du granskar ett korrektur om du har någon av följande behörigheter:

* Behörigheter för arbetsledare eller administratör
* Hantera behörigheter och du är upphovsperson eller ägare till beviset
* Hantera behörigheter med korrekturrollen Författare eller Moderator

Om korrekturet har ett automatiserat arbetsflöde kan du lägga till användaren i en enskild scen. Mer information finns i [Översikt över automatiserat arbetsflöde](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Som standard lägger användare du till följande i korrekturet:

* Få ett e-postmeddelande med en länk till korrekturet.
* Kan fatta beslut om godkännande av korrekturet från Hem-området, enligt beskrivningen i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Du behöver inte aktivera korrektur för att kunna granska korrekturet.

När Automatiserat arbetsflöde är aktiverat och du lägger till en användare till korrekturet som inte har språkkontroll aktiverat i Workfront, skapas en ny fas i det automatiserade arbetsflödet. Användaren som du lägger till läggs automatiskt till på den nya scenen när han/hon visar korrekturet för första gången. Mer information finns i [Översikt över automatiserat arbetsflöde](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Så här delar du ett korrektur med enskilda användare:

1. Klicka på ikonen **Dela** i verktygsfältet till vänster om korrekturläsaren.

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Klicka på **Lägg till mottagare** i listan till vänster.
1. Under **Nya korrekturmottagare** börjar du skriva namnet på en användare som du vill dela korrekturet med och klickar sedan på namnet när det visas i listrutan.
1. (Valfritt) Ändra eventuella alternativ för granskare till höger om personens namn:

   * **Korrekturroll**: Mer information finns i [Hantera korrekturroller i Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Stage**: (Endast tillgängligt om korrekturet har ett automatiserat arbetsflöde). Mer information finns i  [Översikt över automatiska arbetsflödessteg](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **E-postaviseringar**: Välj ett av följande alternativ för att ange hur personen ska meddelas om aktivitet på korrekturet.

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
        <td>Ett e-postmeddelande skickas till granskaren endast om någon uttryckligen svarar på kommentaren (detta utesluter att personen själv svarar på sina kommentarer). Det innebär att om någon i korrekturet gör en ny kommentar så meddelas inte granskaren.<p>Den här inställningen rekommenderas för dina kunder på korrekturet så att de inte meddelas om några andra kommentarer på korrekturet och endast får svar på sina egna kommentarer.</p><p>Även om granskare med den här e-postaviseringsinställningen inte meddelas om andra nya kommentarer, kan de fortfarande visa alla kommentarer i korrekturläsaren.</p><p>Mer information om kommentarer finns i <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visa och svara på korrekturkommentarer</a>.</p></td> 
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
        <td>Workfront skickar ett e-postmeddelande med alla kommentarer, svar och beslut listade endast dagar när det finns någon aktivitet utöver din egen.<p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.</p><p>Ett exempel på hur den här sammanfattningen används är en avdelningsledare som vill övervaka projektets övergripande förlopp.</p><p>Mer information finns i <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Hantera meddelanden om korrekturkommentarer och beslut</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Ingen e-post</td> 
        <td>Workfront skickar inga e-postaviseringar.<br>Det här är användbart för en person som bara läggs till i ett korrektur för referens och som inte behöver informeras om några ändringar.<p>Systemets standardvärde är Daglig sammanfattning (visas också som Inte angivet). Om du eller dina granskare inte gör några andra ändringar har alla dina korrektur den här inställningen.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Valfritt) Upprepa de två föregående stegen för att lägga till flera användare till korrekturet. 
1. (Valfritt) Ange en **tidsgräns** för granskarna (endast tillgängligt om korrekturet inte har ett automatiserat arbetsflöde).
1. (Valfritt) Välj **Skicka e-postmeddelanden till nya mottagare** för att tala om att du har lagt till dem i korrekturet.
1. När du är klar med att lägga till användare i korrekturet klickar du på **Klar.**
