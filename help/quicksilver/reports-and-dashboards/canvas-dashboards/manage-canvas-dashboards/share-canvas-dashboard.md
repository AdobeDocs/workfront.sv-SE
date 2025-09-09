---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Dela en arbetsytans kontrollpanel
description: Du kan dela en Canvas-kontrollpanel med andra Adobe Workfront-användare så att de kan visa eller redigera den.
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: 56d0b9281387cc7b35055461e7868c7e4a194f81
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Dela en arbetsytans kontrollpanel

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Delar av funktionen kanske inte är fullständiga eller fungerar som de ska i det här skedet. Skicka feedback om din upplevelse genom att följa instruktionerna i avsnittet [Ge feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) i översiktsartikeln i Canvas Dashboards.<br>
>&#x200B;>Om du har synpunkter på ett eventuellt fel eller tekniska problem ber vi dig skicka ett supportärende till Workfront Support. Mer information finns i [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>&#x200B;>Observera att betaversionen inte är tillgänglig för följande molnleverantörer:
>
>* Använd din egen nyckel för Amazon Web Services
>* Azure
>* Google Cloud Platform

Du kan dela en Canvas-kontrollpanel med andra Adobe Workfront-användare så att de kan visa eller redigera den.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Alla </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Aktuell: Planera </p> 
<p>Nytt: Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td> 
   <td><p>Visa åtkomst till rapporter, instrumentpaneler och kalendrar</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td><p>Visa behörigheter för instrumentpanelen för att dela kontrollpanelen</p>
   <p>Hantera behörigheter för kontrollpanelen för att tilldela kontrollpanelsbehörigheter</p>
  </td> 
  </tr>
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Att tänka på när det gäller att dela kontrollpaneler

* Kontrollpaneler kan delas med användare, team, grupper, jobbroller eller företagsresurser.

* Som standard har den som skapat en kontrollpanel behörigheten Hantera för kontrollpanelen.

* Systemadministratörer och användare med behörigheten Hantera kan ge åtkomst till en instrumentpanel via Visa eller Hantera.

* Användare med behörigheten Visa på en kontrollpanel kan ge åtkomst till en kontrollpanel.

* När du delar en kontrollpanel ärver resurserna som den delas med behörigheter till de rapporter som visas på kontrollpanelen.

* När en kontrollpanel distribueras via en layoutmall tilldelas alla resurser som tilldelats layoutmallen automatiskt behörigheten Visa för kontrollpanelen (och dess rapporter).


## Dela en arbetsytans kontrollpanel


{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. På sidan **Kontrollpaneler på arbetsytan** väljer du den kontrollpanel som du vill dela.

1. Klicka på knappen **Dela** i det övre högra hörnet på sidan. Dialogrutan **Kontrollpanelsdelning** visas.

1. I fältet **Ge åtkomst till** börjar du med att skriva namnet på en specifik användare, grupp, roll, grupp eller företag som du vill dela arbetsytans kontrollpanel med och markerar det sedan när det visas i listrutan.

1. (Valfritt) Om du vill redigera en resurs åtkomst till instrumentpanelen klickar du på **Visa** bredvid namnet och väljer sedan **Hantera** i listrutan som visas.

   >[!NOTE]
   >
   > Om användare inte har behörigheten Redigera för en kontrollpanel tilldelad via åtkomstnivån, kan de inte tilldelas behörigheten Hantera till en kontrollpanel.

1. Upprepa steg 5-6 för varje resurs som du vill dela kontrollpanelen med.

1. Klicka på knappen **Dela**. Mottagarna får ett e-postmeddelande som informerar dem om att instrumentpanelen har delats med dem, som de nu kan komma åt på **Kontrollpaneler** > **Kontrollpaneler på arbetsytan** > **Delade instrumentpaneler**.

   >[!NOTE]
   >
   > Enskilda användarinställningar och undantag från systemet kan gälla för e-postmeddelanden. <br>
   > Meddelanden skickas bara när de delas direkt med en användare. Delning till grupper, roller, företag och team genererar inga e-postmeddelanden.<br>
   > Behörigheter som ärvts från en layoutmall genererar inga e-postmeddelanden om åtkomst till instrumentpanelen.
