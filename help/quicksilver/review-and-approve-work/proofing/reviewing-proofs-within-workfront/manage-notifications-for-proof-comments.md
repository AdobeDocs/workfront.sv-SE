---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Hantera meddelanden för korrekturkommentarer och beslut
description: När du arbetar med ett korrektur, oavsett om du är en Adobe Workfront-användare eller en extern medarbetare, kan du ange vilka e-postmeddelanden du vill få om kommentarer och beslut som fattas på korrekturet. Mer information finns i Notifications for proof comments and Decision overview.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 0%

---

# Hantera meddelanden för korrekturkommentarer och beslut

När du arbetar med ett korrektur, oavsett om du är en Adobe Workfront-användare eller en extern medarbetare, kan du ange vilka e-postmeddelanden du vill få om kommentarer och beslut som fattas på korrekturet. Mer information finns i [Översikt över meddelanden om korrekturkommentarer och beslut](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Dessa meddelanden skiljer sig från de e-postaviseringar som du kan få om flödet av korrektur mellan granskare. De skiljer sig också från e-postaviseringsinställningarna som du kan konfigurera i Workfront. 

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
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Hantera meddelanden för korrekturkommentarer och beslut

1. Öppna det korrektur som du vill konfigurera de meddelanden du får.
1. Om det vänstra verktygsfältet inte visas klickar du på ikonen **Meny** som finns i det övre vänstra hörnet i Web Proofing Viewer.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Klicka på ikonen **Inställningar** i det vänstra verktygsfältet. ![Settings_icon.png](assets/settings-icon.png)

1. Under **Skicka mig e-postmeddelanden om** klickar du på inställningen som du vill använda för korrekturet.

   Den inställning du väljer gäller bara för det korrektur du har öppnat.

   Systemstandarden är **Daglig sammanfattning**. Om du eller dina granskare inte gör några andra ändringar har alla dina korrektur den här inställningen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alla aktiviteter</td> 
      <td>Ett e-postmeddelande skickas till granskaren varje gång det finns någon aktivitet i korrekturet, t.ex. en ny kommentar, ett svar eller ett beslut.<br><p>Detta är ett bra alternativ för den som hanterar korrekturläsningen eftersom det gör att personen kan se aktiviteten som den är. Användarna får ingen e-postavisering om sin egen aktivitet (t.ex. kommentarer, svar och beslut).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Svar på mina kommentarer</td> 
      <td>Ett e-postmeddelande skickas till granskaren endast om någon uttryckligen svarar på kommentaren (detta utesluter att personen själv svarar på sina kommentarer). Det innebär att om någon i korrekturet gör en ny kommentar så meddelas inte granskaren.<p>Den här inställningen rekommenderas för dina kunder på korrekturet så att de inte meddelas om några andra kommentarer på korrekturet och endast får svar på sina egna kommentarer.</p><p>Även om granskare med den här e-postaviseringsinställningen inte meddelas om andra nya kommentarer, kan de fortfarande visa alla kommentarer i korrekturläsaren.<br></p><p>Mer information finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visa och svara på korrekturkommentarer</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beslut</td> 
      <td>Ett e-postmeddelande skickas till granskaren endast när någon fattar ett beslut.<br><p>Den här e-postvarningen kan vara användbar för den som hanterar godkännandeprocessen (till exempel en projektledare) eftersom den person som hanterar godkännandeprocessen kan övervaka korrekturens förlopp och se vilka användare som har fattat sitt beslut.<br></p><p>Du meddelas inte om ditt eget beslut såvida du inte väljer ett bekräftelsealternativ för e-post när du skickar ditt beslut.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Slutgiltigt beslut</td> 
      <td>Ett e-postmeddelande skickas när det slutliga beslutet fattas om beviset (när den sista godkännaren har fattat sitt beslut).<br><p>Den här varningen används ofta av designern eftersom designern inte behöver delta i själva granskningsdiskussionen. När det slutliga beslutet fattas meddelas formgivaren och kan sedan vidta eventuella nödvändiga åtgärder.<br></p><p>Den här varningen kan även vara användbar för en avdelningsledare som behöver få ett meddelande endast när granskningsprocessen är klar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sammanfattning varje timme</td> 
      <td>Ett e-postmeddelande skickas till granskaren varje timme med en sammanfattning av alla kommentarer, svar och beslut som har fattats under den senaste timmen.<br><p>E-postmeddelandet skickas bara när andra aktiviteter än din egen inträffar under den senaste timmen. Om det inte finns någon aktivitet från andra användare skickas inget e-postmeddelande.<br></p><p>Den här varningen är ett bra sätt att se en översikt över projektet.<br></p><p>Ett exempel på hur man kan använda den här sammanfattningen är en erfaren granskare som behöver en översikt över projektet, men som inte behöver underrättas omedelbart om all aktivitet på beviset.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Daglig sammanfattning</td> 
      <td>(Standardinställning): Ett e-postmeddelande skickas varje dag med alla kommentarer, svar och beslut listade. Ett e-postmeddelande skickas endast på dagar när det finns aktiviteter utöver din egen.<br><p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.<br></p><p>Ett exempel på hur den här sammanfattningen används är en avdelningsledare som vill övervaka projektets övergripande förlopp.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingen e-post</td> 
      <td>Inga e-postaviseringar skickas.<br><p>Den här inställningen är användbar för en person som bara läggs till i ett korrektur för referens och som inte behöver underrättas om några ändringar.</p><p>Obs! <p>Med det här alternativet inaktiveras endast e-postaviseringar som du kan få om korrekturkommentarer och beslut. Det inaktiverar inte e-postaviseringar som du kan få om flödet av ett korrektur, som Nytt korrektur eller Sent Korrektur. Mer information om e-postvarningar om provflödet finns i följande artiklar: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nytt korrekturmeddelande</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-postmeddelandet Ny version</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">Sena korrekturrundor via e-post</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-postmeddelande om korrekturet</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
