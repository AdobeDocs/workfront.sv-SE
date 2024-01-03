---
product-area: projects
navigation-topic: use-predecessors
title: Skapa föregångare mellan projekt
description: En föregångare för flera projekt är en uppgift som en annan aktivitet (som kallas efterföljande aktivitet) i ett annat projekt är beroende av. Föregående är den uppgift som får prioritet framför den beroende (efterföljande) uppgiften. Du kan till exempel skapa ett beroende som kräver att föregående aktivitet markeras med Slutför innan den beroende aktiviteten kan starta.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Skapa föregångare mellan projekt

<!--Audited: 12/2023-->

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

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
 <tr> 
  <td role="rowheader">Adobe Workfront-licens*</td> 
  <td> <p>Nytt: Standard </p>
 <p>eller</p> 
<p>Aktuell: Planera </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteter och projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en föregångare för flera projekt

1. Gå till den uppgift som ska vara din efterföljare (beroende uppgift).
1. Klicka **Föregående** till vänster.
1. Klicka **Lägg till föregående.**
1. I **Överordnat projekt** börjar du skriva namnet på det projekt som innehåller den uppgift som du vill ska vara föregående till den aktuella uppgiften.
1. Klicka på namnet när det visas i listrutan.
1. I **Uppgifter** börjar du skriva namnet på den uppgift som du vill ska vara föregående till den aktuella uppgiften.
1. Ange följande information för att definiera relationen mellan föregående och beroende uppgift:

   * **Beroendetyp:** Välj relationen som du vill att föregående aktivitet ska ha med den beroende aktiviteten. Standardrelationen är &quot;Slutför-Start&quot;, vilket innebär att föregående aktivitet måste slutföras innan den beroende aktiviteten kan startas. Mer information om de olika beroendetyperna finns i [Översikt över typer av uppgiftsberoenden](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Lag:** Ange den tid som måste förflyta efter slutförandet av en framtvingad föregångare tills den beroende aktiviteten kan börja. Mer information om olika typer av fördröjningar finns i [Översikt över fördröjningstyper](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Tvingad:** När det här alternativet är markerat kan beroendeförhållandet mellan de två aktiviteterna inte kringgås av användare som startar aktiviteter tidigt. Om du till exempel tillämpar en relation mellan Aktivitet A och Aktivitet B, kan inte Aktivitet B startas förrän Aktivitet A har slutförts. Mer information om att framtvinga föregående aktiviteter finns i [Tvinga föregående](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Om det här alternativet inte är markerat behandlas beroendet som ett förslag för användarna. Användarna kan t.ex. starta Aktivitet B innan Aktivitet A har slutförts.

1. Klicka **Spara**.

   Uppgifter som har en föregångare för flera projekt visar referensnumret för det projekt som föregångaren tillhör och antalet uppgifter, avgränsade med kolon, i kolumnen Föregående aktiviteter i en uppgiftslista.

   ![Föregångare mellan projekt](assets/cross-project-predecessor-in-list-view.png)

   Föregående-ikonen blir grön när föregående aktivitet har markerats som slutförd. Detta signalerar att den beroende aktiviteten är klar för arbete.

   Hovra över det här värdet om du vill ha mer information om föregående, projektet och datumen. Klicka på den projektövergripande föregångaren i informationsrutan för att öppna uppgiften.

   Klicka nära det övre hörnet av hovringsfönstret för att se mer information om föregående projekt.

   Klicka **Se projekt** för att öppna föregående projekt.

   ![Information om föregångare mellan projekt](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   The **Se projekt** visas bara när du visar en föregångare för flera projekt.

