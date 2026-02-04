---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrera en arbetsytans kontrollpanel
description: Du kan använda ett filter på en Canvas-kontrollpanel när den har skapats.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 156e9d3f-49f6-4372-9749-c7124ff5baee
source-git-commit: f8c41105607e972d3395cf8d89fb1fdf29f0da85
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 0%

---

# Filtrera en arbetsytans kontrollpanel

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Delar av funktionen kanske inte är fullständiga eller fungerar som de ska i det här skedet. Skicka feedback om din upplevelse genom att följa instruktionerna i avsnittet [Ge feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) i översiktsartikeln i Canvas Dashboards.<br>
>Om du har synpunkter på ett eventuellt fel eller tekniska problem ber vi dig skicka ett supportärende till Workfront Support. Mer information finns i [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observera att betaversionen inte är tillgänglig för följande molnleverantörer:
>
>* Använd din egen nyckel för Amazon Web Services
>* Azure
>* Google Cloud Platform


Du kan använda ett filter på en Canvas Dashboard som innehåller uppmaningar. En prompt fungerar som en filtermodifierare som tillämpar ytterligare filtervillkor så att du kan begränsa resultaten ytterligare. Dessa uppmaningar kan ändras varje gång du tillämpar filtret, så att du kan justera det visade resultatet utan att behöva redigera huvudfiltervillkoren för kontrollpanelen eller varje enskild rapport.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
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

## Förutsättningar

Du måste skapa en kontrollpanel innan den kan filtreras.

Mer information finns i [Skapa en arbetsytans kontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Filtrera en kontrollpanel

Utför följande steg i den listade ordningen för att filtrera en kontrollpanel:

* [Del 1: Skapa ett kontrollpanelsfilter](#part-1-create-a-dashboard-filter)
* [Del 2: Skapa en kontrollpanel](#part-2-define-a-dashboard-prompt)
* [Del 3: Använda en kontrollpanel](#step-3-apply-a-dashboard-prompt)

>[!NOTE]
>
>Kontrollpanelsfiltret gäller för alla rapporter där kontrollpanelsfilter inte är inaktiverade.  Du kan utesluta enskilda rapporter från att ha filter på kontrollpanelsnivå genom att utöka åtgärdsmenyn för varje rapport och välja alternativet **Inaktivera filter**.


### Del 1: Skapa ett kontrollpanelsfilter

Med ett kontrollpanelsfilter kan du använda ett gemensamt filter för alla rapporter som är tillgängliga på en kontrollpanel utan att behöva ändra filtren för varje enskild rapport.

>[!NOTE]
>
>Dessa filter kan bara konfigureras av en användare med behörigheten Hantera på instrumentpanelen.


{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. På sidan **Kontrollpaneler** på arbetsytan väljer du den kontrollpanel som du vill använda ett filter på.

1. Klicka på **Filter** i det övre vänstra hörnet på sidan med information om kontrollpanelen. Panelen Filtersida öppnas.

1. Välj **Redigera filter**. Dialogrutan **Kontrollpanelsfilter** öppnas.

1. (Valfritt) Följ stegen nedan om du vill lägga till en regel:

   1. Välj ikonen **Redigera** till höger om regelrutan.

      ![Ikonen Redigera](assets/edit-icon.png)

   1. Klicka på **Lägg till villkor** och lägg sedan till följande information:
      * Markera ett fält som du vill filtrera efter.
      * Välj ett alternativ (eller filtermodifierare) för att definiera vilken typ av villkor fältet måste uppfylla.

   1. (Valfritt) Klicka på **Lägg till filtergrupp** om du vill lägga till ytterligare en uppsättning filtervillkor. Standardoperatorn mellan uppsättningarna är AND. Klicka på operatorn för att ändra den till ELLER.

1. Fortsätt till [Del 2: Skapa en instrumentpanelsprompt](#part-2-define-a-dashboard-prompt).


### Del 2: Ange en kontrollpanelsprompt

På en kontrollpanel får användarna möjlighet att lägga till ytterligare anpassade filter för rapporter som är tillgängliga på kontrollpanelen.

>[!NOTE]
>
>Alternativen i instrumentpanelsprompten kan bara konfigureras av en användare med behörigheten Hantera på instrumentpanelen.

1. Följ stegen nedan för att lägga till en fråga:

   1. Välj **Lägg till fråga**. Nya fält visas till höger på skärmen.

   1. Ange en etikett i fältet **Anpassa etikett**.

   1. Markera det fält som du vill att uppmaningen ska baseras på genom att skriva namnet på fältet och sedan markera det när det visas i listan. 

1. Följ stegen nedan om du vill lägga till en anpassad fråga:

   1. Välj **Lägg till anpassad fråga**. Nya fält visas till höger på skärmen.

   1. (Valfritt) Ange en ny etikett i fältet **Anpassa etikett**. Som standard tilldelas etiketten *Ny anpassad fråga*.

   1. Klicka på **Lägg till nytt alternativ**.

   1. Ange promptnamnet i fältet **Alternativvärde**.

   1. Klicka på **Lägg till villkor** och ange sedan fältet som du vill filtrera efter och modifieraren som definierar vilken typ av villkor som fältet måste uppfylla.

      >[!NOTE]
      >
      >Villkoret för en anpassad prompt kan bara redigeras i textläge. Detta gör att flera villkor kan användas i ett enda fält.


   1. (Valfritt) Klicka på **Lägg till filtergrupp** om du vill lägga till ytterligare en uppsättning filtervillkor. Standardoperatorn mellan uppsättningarna är AND. Klicka på operatorn för att ändra den till ELLER.

1. Klicka på **Spara** för att använda filtret på instrumentpanelen.

1. Fortsätt till [Del 3: Ange en instrumentpanelsprompt](#step-3-apply-a-dashboard-prompt).

### Steg 3: Ange en kontrollpanelsprompt

Alla användare som har tillgång till en kontrollpanel kan lägga till en kontrollpanelsfråga på en kontrollpanel för arbetsytan när filtret och uppmaningarna har skapats.

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. På sidan **Kontrollpaneler** på arbetsytan väljer du den kontrollpanel som du vill använda uppmaningen på.

1. Klicka på **Filter** i det övre vänstra hörnet på sidan med information om kontrollpanelen. Panelen Filtersida öppnas.

1. I avsnittet **Visa poster där..** väljer du ett villkor för en eller alla uppmaningar som visas. Uppmaningen tillämpas och en **kontrollpanelsfilter**-tagg visas i hörnet av rapportwidgeten.
   ![Välj villkor](assets/prompts-list.png)

1. Klicka på ikonen **Stäng** ![Stäng &#x200B;](assets/close-icon.png) i det övre högra hörnet om du vill dölja panelen.


