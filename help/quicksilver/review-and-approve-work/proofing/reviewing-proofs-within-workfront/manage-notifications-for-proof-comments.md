---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Hantera meddelanden för korrekturkommentarer och beslut
description: När du arbetar med ett korrektur, oavsett om du är en Adobe Workfront-användare eller en extern medarbetare, kan du ange vilka e-postmeddelanden du vill få om kommentarer och beslut som fattas på korrekturet. Mer information finns i Notifications for proof comments and Decision overview.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 385f4a6663cacfdcf519bf5699fc1840c2cb2adc
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 0%

---

# Hantera meddelanden för korrekturkommentarer och beslut

<!-- Audited: 4/2025 -->

När du arbetar med ett korrektur, oavsett om du är en Adobe Workfront-användare eller en extern medarbetare, kan du ange vilka e-postmeddelanden du vill få om kommentarer och beslut som fattas på korrekturet. Mer information finns i [Översikt över meddelanden om korrekturkommentarer och beslut](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Dessa meddelanden skiljer sig från de e-postaviseringar som du kan få om flödet av ett korrektur mellan granskare och de e-postaviseringsinställningar som du kan konfigurera i Workfront.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturroll </td> 
   <td>Granskare, granskare och godkännare, författare, moderator</td> 
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

## Hantera meddelanden för korrekturkommentarer och beslut

1. Öppna det korrektur som du vill konfigurera meddelanden för.
1. Om det vänstra verktygsfältet inte visas klickar du på ikonen **Meny** i det övre vänstra hörnet i Web Proofing Viewer.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Klicka på ikonen **Inställningar** ![Settings_icon.png](assets/settings-icon.png) i det vänstra verktygsfältet.

1. I avsnittet **Skicka mig e-postmeddelanden om** väljer du meddelandeinställningen för det här korrekturet.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alla aktiviteter</td> 
      <td>Ett e-postmeddelande skickas till granskaren varje gång det finns någon aktivitet i korrekturet, t.ex. en ny kommentar, ett svar eller ett beslut.<br><p>Den här inställningen rekommenderas för personen som hanterar korrekturläsningen eftersom det gör att personen kan se aktiviteten allt eftersom den sker. Användarna får ingen e-postavisering om sin egen aktivitet (t.ex. kommentarer, svar eller beslut).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Svar på mina kommentarer</td> 
      <td>Ett e-postmeddelande skickas till granskaren endast om någon svarar direkt på kommentaren (exklusive sina svar på egna kommentarer).<p>Den här inställningen rekommenderas för dina kunder så att de endast meddelas om svar på sina egna kommentarer och inte om andra kommentarer som gjorts på korrekturet, även om de fortfarande kan visa alla kommentarer i korrekturläsaren.</p>
      <p>Mer information finns i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Visa och svara på korrekturkommentarer</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beslut</td> 
      <td>Ett e-postmeddelande skickas till granskaren endast när någon fattar ett beslut.<br><p>Den här e-postvarningen kan vara användbar för den som hanterar godkännandeprocessen eftersom den person som hanterar godkännandeprocessen kan övervaka korrekturets förlopp och se vilka användare som har fattat sitt beslut.<br></p><p>Du meddelas inte om ditt eget beslut såvida du inte väljer ett bekräftelsealternativ för e-post när du skickar ditt beslut.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Slutgiltigt beslut</td> 
      <td>Ett e-postmeddelande skickas när det slutliga beslutet fattas om beviset.<br><p>Den här varningen används ofta av designern eftersom designern inte behöver delta i själva granskningsdiskussionen. När det slutliga beslutet fattas meddelas formgivaren och kan sedan vidta eventuella nödvändiga åtgärder.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sammanfattning varje timme</td> 
      <td>Ett e-postmeddelande skickas till granskaren varje timme med en sammanfattning av alla kommentarer, svar och beslut som har fattats under den senaste timmen.<br><p>E-postmeddelandet skickas bara när andra aktiviteter än din egen inträffar under den senaste timmen. Om det inte finns någon aktivitet från andra användare skickas inget e-postmeddelande.<br></p><p>Den här varningen är ett bra sätt att se en översikt över projektet allt eftersom det utvecklas.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Daglig sammanfattning</td> 
      <td>(Standardinställning): Ett e-postmeddelande skickas varje dag med alla kommentarer, svar och beslut listade. Detta skickas endast på dagar när det finns aktiviteter utöver din egen.<br><p>Den här varningen är ett bra sätt att se en sammanfattning av projektet utan att behöva överbelastas med flera uppdateringar under dagen.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingen e-post</td> 
      <td>Inga e-postaviseringar skickas.<br><p>Den här inställningen är användbar för en person som bara läggs till i ett korrektur för referens och som inte behöver informeras om några ändringar.</p><p>Obs! <p>Med det här alternativet inaktiveras endast e-postvarningar om korrekturkommentarer och beslut. Det innebär inte att de e-postvarningar du kan få om korrekturflödet inaktiveras, till exempel e-postmeddelandet Nytt korrektur eller Försenat korrektur. Mer information finns i följande artiklar: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nytt korrekturmeddelande</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-postmeddelandet Ny version</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">Sena korrekturrundor via e-post</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-postmeddelande om korrekturet</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
