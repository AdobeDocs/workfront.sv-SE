---
product-area: documents;setup
navigation-topic: review-a-proof
title: Konfigurera inställningar för korrekturläsare
description: Du kan konfigurera inställningar för både Web Proofing Viewer och Desktop Proofing Viewer.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 0%

---

# Konfigurera inställningar för korrekturläsare

Du kan konfigurera följande inställningar för både Web Proofing Viewer och Desktop Proofing Viewer:

* Anger om kommentarmarkeringar och punkter visas på korrektur.
* Om markeringsverktygen visas längst upp i korrekturläsaren eller i en nedrullningsbar meny.
* Vilka e-postmeddelanden du får som granskare på det korrektur du har öppnat.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

Du kan konfigurera följande inställningar för Desktop Proofing Viewer:

* Hur du vill att länkar i webbplatsinnehåll ska öppnas i visningsprogrammet.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* Vad händer när du klickar på en länk som är inställd på att öppnas på en ny webbläsarflik eller i ett nytt fönster.
* Rensa cachedata som kan sparas med det korrektur som du visar för att aktivera visning av innehåll som popup-fönster (som kan blockeras av webbläsarens cachedata) i visningsprogrammet.

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

## Konfigurera inställningar för korrekturläsare

Så här konfigurerar du visningsinställningar för språkkontroll:

1. Öppna Web Proofing Viewer eller Desktop Proofing Viewer på något av följande sätt:

   * Om du har korrektur i Adobe Workfront går du till en dokumentlista som innehåller ett korrektur som du vill visa, för muspekaren över dokumentet och klickar sedan på **Öppna korrektur**.
   * Om du använder Workfront Proof klickar du på ikonen **Gå till korrektur** för korrekturet på kontrollpanelen eller en visningslista ![](assets/go-to-proof-blue-icon.png) .

1. Om det vänstra verktygsfältet inte visas klickar du på ikonen **Meny** som finns i det övre vänstra hörnet i Web Proofing Viewer.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Klicka på ikonen **Inställningar** ![](assets/settings-icon-in-pv.png) i det vänstra verktygsfältet.

1. Konfigurera någon av följande **inställningar** som visas.

   Vilka inställningar som är tillgängliga beror på vilken typ av korrektur du har öppnat.

   * **Visa markeringar** (alltid tillgängligt i Web Proofing Viewer och Desktop Proofing Viewer): Det här är de kommentarmarkeringar som granskarna lägger till i korrektur när de använder markeringsverktygen. Om du inaktiverar dem kan du fortfarande se dem när du klickar på en kommentar i kommentarlistan.

     Den här inställningen påverkar alla korrektur som du öppnar.

   * **Visa punkter** (alltid tillgängligt i Web Proofing Viewer och Desktop Proofing Viewer): Detta är de numrerade punkter som granskare lägger till i korrektur när de använder markeringsverktygen. De visar var och i vilken ordning granskaren lade till kommentarer. Om du inaktiverar dem kan du fortfarande se dem när du klickar på en kommentar i kommentarlistan.

     Den här inställningen påverkar alla korrektur som du öppnar.

   * **Använd utökade markeringsverktyg** (alltid tillgängligt i Web Proofing Viewer och Desktop Proofing Viewer): Som standard visas markeringsverktygsalternativen längst upp i korrekturläsaren. Du kan konfigurera dem så att de visas på en lodrät meny som bara öppnas när du klickar på den.

     Den här inställningen används för alla korrektur som du öppnar.

   * **Skicka mig e-postmeddelanden om** (alltid tillgängligt i Web Proofing Viewer och Desktop Proofing Viewer): Klicka på ett av alternativen nedan. Den här inställningen påverkar bara det korrektur som är öppet. Mer information finns i [Översikt över meddelanden om korrekturkommentarer och beslut](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

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

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **När du klickar på hyperlänkar i ett korrektur** (endast tillgängligt i Desktop Proofing Viewer): Välj ett alternativ för att ange vad som ska hända i Desktop Proofing Viewer när du klickar på en länk som är inställd på att öppnas på en ny webbläsarflik eller i ett nytt fönster.

     Den här inställningen gäller för alla interaktiva korrektur som du öppnar.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Öppna i korrekturläsaren</td> 
        <td>Länkarna öppnas alltid i Desktop Proofing Viewer och du kan kontrollera att det länkade innehållet är korrekt. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Öppna i webbläsaren</td> 
        <td>Länkarna öppnas alltid i webbläsaren, inte i ett korrekturläsare. Det går inte att korrekturgranska det länkade innehållet.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Fråga mig varje gång</td> 
        <td> <p>Du får en fråga varje gång om du vill öppna länken i Desktop Proofing Viewer eller i webbläsaren. Om du öppnar länken i Desktop Proofing Viewer kan du göra ett korrektur av det länkade innehållet. Om du öppnar länken i webbläsaren kan du inte bevisa att det länkade innehållet är korrekt.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>Den här inställningen påverkar bara det korrektur som är öppet.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Rensa cache**: Rensar webbläsarens cachedata som kan sparas med ett interaktivt korrektur som du visar. Detta gör att innehåll som popup-fönster (som kan blockeras av webbläsarens cachedata) kan visas i Desktop Proofing Viewer.

     De data som rensas inkluderar HTTP-cachen (t.ex. bilder som ska återanvändas efter nästa siduppdatering) och webblagringsdatacachen (t.ex. cookies och data som identifierar användare).

     Den här inställningen påverkar bara det korrektur som är öppet.
