---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Kopiera en kontrollpanel
description: Du kan kopiera en kontrollpanel och allt dess innehåll (rapporter, kalendrar och externa sidor). När du kopierar innehållet på en kontrollpanel kan du välja att behålla dem så som de visas på den ursprungliga kontrollpanelen, eller skapa nya objekt som är kopior av dem på den ursprungliga kontrollpanelen. Du kan också välja att inte överföra eller kopiera objekt på den nya instrumentpanelen.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Kopiera en kontrollpanel

Du kan kopiera en kontrollpanel och allt dess innehåll (rapporter, kalendrar och externa sidor). När du kopierar innehållet på en kontrollpanel kan du välja att behålla dem så som de visas på den ursprungliga kontrollpanelen, eller skapa nya objekt som är kopior av dem på den ursprungliga kontrollpanelen. Du kan också välja att inte överföra eller kopiera objekt på den nya instrumentpanelen.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa åtkomst till en instrumentpanel</p> <p>Du får Hantera-åtkomst till den kopierade instrumentpanelen</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar

Du måste skapa en kontrollpanel innan du kan kopiera den.

Mer information om hur du skapar kontrollpaneler finns i [Skapa en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Kopiera en kontrollpanel

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png)och sedan klicka **Kontrollpaneler**.

1. Markera den kontrollpanel som du vill kopiera och klicka sedan på **Kopiera** ![](assets/copy-icon.png).\
   eller\
   Öppna den kontrollpanel som du vill kopiera och klicka sedan på **Instrumentpanelsåtgärder** > **Kopiera**.\
   Dialogrutan Kopiera kontrollpanel visas. Alla objekt på den ursprungliga instrumentpanelen visas.

1. I **Instrumentpanelsnamn** anger du ett nytt namn för kontrollpanelen.
1. Om du vill markera alla objekt på den befintliga kontrollpanelen och kopiera dem till den kopierade kontrollpanelen, låter du **Markera alla** markerat. Som standard kopieras rapporter, kalendrar eller listor på den befintliga kontrollpanelen till den nya kontrollpanelen.\
   eller\
   Om du bara vill överföra specifika objekt från den ursprungliga kontrollpanelen till den nya avmarkerar du de objekt som du inte vill ska visas på den nya kontrollpanelen och väljer sedan något av följande alternativ för varje valt objekt:

   * **Gör en kopia:** Objektet kopieras från den ursprungliga kontrollpanelen och en ny version av det objektet visas på den nya kontrollpanelen. Ändringar som görs i objektet på den nya kontrollpanelen återspeglas inte i objektet på den ursprungliga kontrollpanelen. På samma sätt återspeglas inte ändringar som görs i objektet på den ursprungliga kontrollpanelen i objektet på den nya kontrollpanelen.\
      Använd det här alternativet när du vill ändra den ursprungliga rapporten på den ursprungliga kontrollpanelen.\
      Du kan till exempel kopiera en kontrollpanel som heter&quot;Team B&quot; och ändra namnet till&quot;Team A.&quot; På kontrollpanelen&quot;Team B&quot; finns en rapport som heter&quot;Team B Report&quot;. Eftersom den här rapporten innehåller data som är specifika för Team B väljer du alternativet att skapa en kopia av den här rapporten så att du kan anpassa den för Team A och senare byta namn på den till&quot;Team A Report&quot;.\
      Med det här alternativet tar du bort delningsbehörigheterna för den ursprungliga rapporten från den kopierade rapporten. Köra den här rapporten med åtkomsträttigheterna för information förblir intakt på den kopierade rapporten.

   * **Använd original:** Visar det ursprungliga objektet på den nya instrumentpanelen. Ändringar som görs i objektet på den nya kontrollpanelen återspeglas även i objektet på den ursprungliga kontrollpanelen. På samma sätt återspeglas ändringar som görs i objektet på den ursprungliga kontrollpanelen i objektet på den nya kontrollpanelen.\
      Med det här alternativet behåller du delningsbehörigheterna för den ursprungliga rapporten. Körningen av den här rapporten med åtkomsträttigheterna för information förblir också intakt.

1. (Valfritt) Byt namn på alla objekt som du har markerat.
1. Klicka **Kopiera instrumentpanel**.
1. (Valfritt) Om du vill redigera någon av de kopierade rapporterna, kalendrarna eller externa sidorna på den kopierade kontrollpanelen gör du något av följande:

   * Om du vill redigera information för någon av de kopierade rapporterna klickar du på rapportnamnet på kontrollpanelen och sedan på **Rapportåtgärder** > **Redigera**.

      Du kan till exempel redigera rapporten Visa, Filter, Gruppering, Fråga eller Diagram eller en kopierad rapport.

   * Om du vill återskapa behörigheter för de kopierade rapporterna klickar du på rapportnamnet på den nya instrumentpanelen och sedan på **Rapportåtgärder** > **Delning** och uppdatera behörigheterna för rapporten.

      När du kopierar en rapport när du kopierar en kontrollpanel tas behörigheterna för den rapporten bort.

   * Om du vill ändra rapporten Kör den här rapporten med åtkomstbehörigheten för information klickar du på namnet på rapporten på den nya instrumentpanelen och sedan på **Rapportåtgärder** > **Redigera** > **Rapportalternativ**.\
      När du har kopierat en rapport behålls rapporten Kör den här rapporten med åtkomstbehörighet endast under följande omständigheter:

      (Om inga av dessa villkor är uppfyllda tas den här rapporten med åtkomstbehörigheterna bort och den nya Kör den här rapporten med åtkomstbehörigheten för ändras till den användare som skapade den kopierade rapporten.)

      Om användaren som kopierar kontrollpanelen och dess rapporter har administratörsbehörighet.

      * Om användaren som kopierar kontrollpanelen och dess rapporter har administratörsbehörighet.
      * Om användaren som kopierar kontrollpanelen och dess rapporter är inställda som Kör den här rapporten med åtkomstbehörigheten för de rapporter som kopieras.
      * Om användaren som kopierar rapporten har behörigheten Hantera för rapporten.
