---
product-area: projects
navigation-topic: use-predecessors
title: Skapa projektövergripande föregångare
description: En föregångare för flera projekt är en uppgift som en annan aktivitet (som kallas efterföljande aktivitet) i ett annat projekt är beroende av. Föregående är den uppgift som får prioritet framför den beroende (efterföljande) uppgiften. Du kan till exempel skapa ett beroende som kräver att föregående aktivitet markeras med Slutför innan den beroende aktiviteten kan starta.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Skapa föregångare mellan projekt

<!--Audited: 12/2024-->

En föregångare mellan projekt är en uppgift som en annan aktivitet (som kallas efterföljande aktivitet) i ett annat projekt är beroende av. Föregående är den uppgift som får prioritet framför den beroende (efterföljande) uppgiften. Du kan till exempel skapa ett beroende som kräver att föregående aktivitet markeras med Slutför innan den beroende aktiviteten kan starta.

Med Adobe Workfront kan uppgifter vara beroende av uppgifter i andra projekt, på samma sätt som föregående aktiviteter i ett och samma projekt.

>[!INFO]
>
>Ett företag som är på väg att gräva har till exempel bara en bakgrund, och två projekt har uppgifter som kräver att bakgrunden används. Projektledaren kan göra uppgiften i det första projektet till en föregångare till uppgiften i det andra projektet. Detta visar att det andra projektet kan börja använda bakgrunden när det första projektet är klart.

När du länkar projekt via föregående projekt påverkas det sekundära projektet (det som har föregående aktivitet) av datumet för det primära projektet (det som har efterföljande aktivitet).

>[!TIP]
>
>Du måste beräkna om tidslinjer för projekten för att kunna se datum som uppdaterats för det sekundära projektet. Mer information om hur du beräknar om tidslinjer finns i [Konfigurera tidslinjeomberäkningar för projekt](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Mer information om föregående relationer finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p> 
  
   <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Skapa en föregångare för flera projekt

>[!TIP]
>
>Även om det liknar att skapa malluppgiftsföregångare när du skapar föregående aktiviteter för en projektuppgift, kan du inte skapa föregående aktiviteter mellan mallar för malluppgifter.


1. Gå till den uppgift som ska vara din efterföljare (beroende uppgift).
1. Klicka på **Föregående** i den vänstra panelen.

   >[!TIP]
   >
   >   Din Workfront- eller gruppadministratör kan ta bort avsnittet **Föregående** eller andra avsnitt från den vänstra panelen.

1. Klicka på **Lägg till föregående.**
1. I fältet **Överordnat projekt** börjar du skriva namnet på projektet som innehåller aktiviteten som du vill ska vara föregående till den aktuella aktiviteten.
1. Klicka på namnet när det visas i listrutan.
1. I fältet **Uppgifter** börjar du skriva namnet på den uppgift som du vill ska vara föregående till den aktuella uppgiften.
1. Ange följande information för att definiera relationen mellan föregående och beroende uppgift:


   * **Beroendetyp:** Välj relationen som du vill att föregående aktivitet ska ha med den beroende aktiviteten. Standardrelationen är &quot;Slutför-Start&quot;, vilket innebär att föregående aktivitet måste slutföras innan den beroende aktiviteten kan startas. Mer information om de olika beroendetyperna finns i [Översikt över aktivitetsberoendetyperna](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Sena:** Ange hur lång tid som måste gå efter det att en framtvingad föregångare har slutförts tills den beroende aktiviteten kan börja. Mer information om de olika fördröjningstyperna finns i [Översikt över fördröjningstyper](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Kräv:** När det här alternativet har valts kan beroendeförhållandet mellan de två aktiviteterna inte kringgås av användare som startar aktiviteter tidigt. Om du till exempel tillämpar en relation mellan Aktivitet A och Aktivitet B, kan inte Aktivitet B startas förrän Aktivitet A har slutförts. Mer information om hur du framtvingar föregångare finns i [Tvinga föregångare](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Om det här alternativet inte är markerat behandlas beroendet som ett förslag för användarna. Användarna kan t.ex. starta Aktivitet B innan Aktivitet A har slutförts.

1. Klicka på **Spara**.

   Uppgifter som har en föregångare för flera projekt visar referensnumret för det projekt som föregångaren tillhör och antalet uppgifter, avgränsade med kolon, i kolumnen Föregående aktiviteter i en uppgiftslista.

   ![Föregångare mellan projekt](assets/cross-project-predecessor-in-list-view.png)

   Föregående-ikonen blir grön när föregående aktivitet har markerats som slutförd. Detta signalerar att den beroende aktiviteten är klar för arbete.

   Hovra över det här värdet om du vill ha mer information om föregående, projektet och datumen. Klicka på den projektövergripande föregångaren i informationsrutan för att öppna uppgiften.

   Klicka nära det övre hörnet av hovringsfönstret för att se mer information om föregående projekt.

   Klicka på **Se Projekt** för att öppna föregående offerts projekt.

   ![Information om föregående tvärprojekt](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   Alternativet **Se projekt** visas bara när du visar en föregångare för flera projekt.

