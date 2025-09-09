---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Lägga till en Canvas-kontrollpanel i en layoutmall
description: Du kan lägga till en kontrollpanel för arbetsytan i en layoutmall så att den ersätter startsidan, visas i det vänstra objektets panel eller är fäst på det övre fältet.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 91ebcec5-99a4-4096-8d4e-b4ea31755d75
source-git-commit: 56d0b9281387cc7b35055461e7868c7e4a194f81
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Lägga till en Canvas-kontrollpanel i en layoutmall

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Delar av funktionen kanske inte är fullständiga eller fungerar som de ska i det här skedet. Skicka feedback om din upplevelse genom att följa instruktionerna i avsnittet [Ge feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) i översiktsartikeln i Canvas Dashboards.<br>
>>Om du har synpunkter på ett eventuellt fel eller tekniska problem ber vi dig skicka ett supportärende till Workfront Support. Mer information finns i [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>>Observera att betaversionen inte är tillgänglig för följande molnleverantörer:
>
>* Använd din egen nyckel för Amazon Web Services
>* Azure
>* Google Cloud Platform

Du kan lägga till en kontrollpanel för arbetsytan i en layoutmall så att den ersätter startsidan, visas i det vänstra objektets panel eller är fäst på det övre fältet i hela Adobe Workfront.

![Vänster panel](assets/left-panel.png)

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
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td><p>Hantera behörigheter för kontrollpanelen</p>
  </td> 
  </tr> 
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Lägga till en Canvas-kontrollpanel på den vänstra panelen

{{step-1-to-setup}}

1. I den vänstra panelen väljer du **Gränssnitt** och sedan **Layoutmallar**.

1. Välj en mall på sidan **Layoutmallar**.

1. På sidan med mallinformation väljer du det objekt som du vill lägga till instrumentpanelen i listrutan **Anpassa vad användare ser**.

   ![Anpassa vad användarna ser i listrutan](assets/customize-what-users-see.png)

1. Bläddra nedåt till **vänsterpanelen** och klicka sedan på **Lägg till kontrollpanel**.

1. Ange ett **Snabblänknamn** i rutan **Lägg till anpassad kontrollpanel**.

1. I listrutan **Välj en kontrollpanel** väljer du **Kontrollpaneler på arbetsytan**.

1. I listrutan till höger om **Välj en kontrollpanel** väljer du den kontrollpanel på arbetsytan som du vill lägga till i den vänstra panelen.

1. Klicka på **Lägg till**. Kontrollpanelen visas i det vänstra panelavsnittet.

1. Klicka på **Spara**.

   >[!NOTE]
   >
   >När de placeras på ett arbetsobjekt, t.ex. ett projekt, en uppgift, ett ärende, Portfolio eller ett program, begränsas de resultat som visas i respektive rapport till de poster som är tillgängliga i det objektet.


## Lägg till en arbetsytekontrollpanel i det övre fältet

{{step-1-to-setup}}

1. I den vänstra panelen väljer du **Gränssnitt** och sedan **Layoutmallar**.

1. Välj en mall på sidan **Layoutmallar**.

1. Klicka på **Lägg till nytt häftstift** i **övre navigeringsområdet** och välj sedan **Lägg till en instrumentpanel** i listrutan.

1. Ange ett **snabblänksnamn** i rutan **Fäst en sida**.

1. I listrutan **Välj en kontrollpanel** väljer du **Kontrollpaneler på arbetsytan**.

1. I listrutan till höger om **Välj en kontrollpanel** väljer du den kontrollpanel för arbetsytan som du vill lägga till i det övre fältet.

1. Klicka på **Lägg till**. Kontrollpanelen visas i det övre fältet.

1. Klicka på **Spara**.

## Lägg till en Canvas-instrumentpanel som startsida

{{step-1-to-setup}}

1. I den vänstra panelen väljer du **Gränssnitt** och sedan **Layoutmallar**.

1. Välj en mall på sidan **Layoutmallar**.

1. Klicka på **Välj landningssida** i avsnittet **Övre navigering** och välj sedan **Lägg till en instrumentpanel** i listrutan.

1. Ange ett **snabblänknamn** i rutan **Lägg till anpassad kontrollpanel**.

1. I listrutan **Välj en kontrollpanel** väljer du **Kontrollpaneler på arbetsytan**.

1. I listrutan till höger om **Välj en kontrollpanel** väljer du den kontrollpanel på arbetsytan som du vill lägga till som startsida.

1. Klicka på **Lägg till**.

1. Klicka på **Spara**.
