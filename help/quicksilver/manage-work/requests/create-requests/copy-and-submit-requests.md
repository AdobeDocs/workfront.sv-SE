---
title: Kopiera och skicka begäranden
description: När du skickar in liknande begäranden ofta kan du kopiera en befintlig skickad begäran. I det här fallet kan du kopiera en befintlig begäran, göra minimala ändringar i den och skicka den igen som en ny begäran.
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: bb68f15c2d8ffabfb67a7789de14ef916cd2dbef
workflow-type: tm+mt
source-wordcount: '1367'
ht-degree: 0%

---

# Kopiera och skicka begäranden

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön.</span>

När du skickar in liknande begäranden ofta kan du kopiera en befintlig skickad begäran. I det här fallet kan du kopiera en befintlig begäran, göra minimala ändringar i den och skicka den igen som en ny begäran.

## Åtkomstkrav

<!--drafted - replace table with P&P:

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
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
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
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Åtkomst att lägga till begäranden i en begärandekö</p> <p>Visa eller högre behörigheter för den befintliga begäran</p> <p>Mer information om hur du ställer in en begärandekö finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha en begäran om att du eller någon i din organisation som tidigare har skickats in ska kunna kopiera den och skicka den igen. Om begäran tillhör någon annan måste du ha åtminstone behörighet att visa den för att kunna kopiera och skicka den som ny.

## Att tänka på när det gäller att kopiera och skicka begäranden som nya

* Du kan bara kopiera och skicka skickade begäranden. Du kan inte kopiera utkast.
* Du kan kopiera och skicka in begäranden som du ursprungligen skickade, eller förfrågningar som andra skickat och du har tillgång till åtminstone Visa.
* Du har alltid tillgång till att kopiera och skicka in en kopia av dina egna förfrågningar, såvida inte någon har tagit bort dina behörigheter till dem.
* Åtkomst till kopierings- och sändningsbegäranden som ursprungligen skickats in av andra personer kan beviljas automatiskt till personer i samma företag när den som skapade kön för begäran aktiverar **Personer från samma företag ärver samma behörigheter för alla begäranden** under Köinformation eller Redigera projekt. Om du inaktiverar den här inställningen kan endast den som gjorde originalet visa sina egna förfrågningar.

  Mer information finns i följande artiklar:

   * [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md)

* Du kan uppdatera kopian av den ursprungliga begäran innan du skickar in den igen som en ny begäran.
* Om följande ändringar inträffar efter att den ursprungliga begäran har skickats kan du inte längre kopiera den och skicka den igen:

   * Begärandekön togs bort.
   * Köämnet togs bort.

     >[!TIP]
     >
     >Om köämnet var det enda i begärandekön kan du fortfarande kopiera och skicka begäran, och den kommer att sparas i själva begärandekön.

   * Begärandekön publiceras inte längre som en kö för hjälpbegäranden. Mer information finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Om begärandekön inte har något köämne och den ursprungliga begäran skickades före januari 2022.

   * Status för det projekt som är associerat med begärandekön är inte längre Aktuell.

* Du kan kopiera och skicka en kopia av en konverterad begäran om den bevaras i konverteringsprocessen. Mer information finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >Den kopierade begäran är inte länkad till ett matchande objekt.

## Kopiera och skicka begäranden

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Begäranden**.
1. (Villkorligt) Om avsnittet Skickat inte visas som standard klickar du på **Skickat** i den vänstra panelen.
1. Leta reda på den begäran som du vill kopiera och skicka som ny, och gör något av följande:

   * Markera den och klicka sedan på <span class="preview"> **Kopiera** ![](assets/copy-and-submit-as-new-requests-area-nwe.png)</span> i det övre vänstra hörnet i listan Skickade begäranden.

   >[!TIP]
   >
   > <span class="preview">Om du inte valde någon begäran först är ikonen Kopiera nedtonad.</span>

   * Klicka på **Mer** meny ![](assets/more-icon.png) till höger om namnet på begäran och klicka sedan på **Kopiera och skicka som nya**

     eller

     Högerklicka på den valda begäran och klicka sedan på **Kopiera och skicka som nya**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Om du inte har behörighet att skapa problem får du en varning om att administratören har begränsat dig från att skapa förfrågningar.

1. (Valfritt) Uppdatera följande information vid behov:

   * **Typ av begäran**: begärandekön där den kopierade begäran sparas. Som standard sparas den kopierade begäran i begärandekön för den ursprungliga begäran.
   * **Ämnesgrupper** och **Köämnen**, om de är markerade. Namnen eller ämnesgrupperna och köämnena är anpassade för din miljö. Som standard sparas den kopierade begäran i ämnesgrupperna och i köämnena i den ursprungliga begäran.

     >[!TIP]
     >
     >Om sökvägen ändras från sökvägen till den ursprungliga begäran har kön ändrats av den som skapade kön.

1. (Valfritt) Uppdatera eventuell information från den kopierade begäran. Beroende på vilka fält som skaparen av begärandekön har aktiverat i **Nya fält** i **Köinformation** kan du hitta något av följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ämne</strong> </td> 
      <td>Visar namnet på den ursprungliga begäran. Uppdatera den om det behövs. Annars namnger Workfront den kopierade begäran <b>Kopia av &lt;name of="" original="" request=""&gt;</b>. Detta är ett obligatoriskt fält.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td>Visar beskrivningen av den ursprungliga begäran. Uppdatera den om det behövs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Visar URL:en för den ursprungliga begäran. Uppdatera den om det behövs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioritet</strong> </td> 
      <td> <p>Ange prioriteten för din begäran. Prioriteten bör definiera hur snabbt du anser att denna begäran bör lösas. Standardalternativen är:</p> 
       <ul> 
        <li>Ingen</li> 
        <li>Låg</li> 
        <li>Normal</li> 
        <li>Hög</li> 
        <li>Urgent</li> 
       </ul> <p>Din Workfront-administratör kan ändra namnen på prioriteter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Allvarlighetsgrad</strong> </td> 
      <td> <p>Ange allvarlighetsgraden för din begäran. Allvarlighetsgraden bör definiera hur den här förfrågan påverkar ditt arbete om den inte kan lösas i tid. Standardalternativen är:</p> 
       <ul> 
        <li>Kosmetisk</li> 
        <li>Orsakar förvirring</li> 
        <li>Fel med tillfälliga lösningar</li> 
        <li>Fel utan någon lösning</li> 
        <li>Allvarligt fel</li> 
       </ul> <p>Din Workfront-administratör kan ändra namn på allvarlighetsgrader.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primär kontakt</strong> </td> 
      <td>Den primära kontaktpersonen för en begäran är dig som standard, eftersom du är den person som ska besvara eventuella frågor som rör begäran. Du kan dock ändra detta till vilken annan Workfront-användare som helst.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Uppdrag</strong></span> </td> 
      <td> <p>Ange namnet på en aktiv användare, jobbroll eller team som förfrågan ska tilldelas. </p> <p> Du kan ange fler än en användare, jobbroll eller team. </p> <p>Beroende på hur frågekö konfigurerades kan du kanske bara tilldela begäran till en eller två typer av resurser, i stället för till alla tre. </p> <p>Vi rekommenderar att du använder routningsregler för dina begärandeköer så att de automatiskt kan dirigeras till rätt resurser. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Beroende på hur frågekö konfigurerades kan du kanske bara tilldela en typ av resurs till begäran (till exempel användare). Om en routningsregel även är associerad med begärandekön och den automatiskt dirigerar begäran till en annan typ av resurs (till exempel ett team), tilldelas din begäran både till den enhet som du anger manuellt när du skickar begäran (användare) och den resurs som anges i routningsregeln (teamet).</p> <p style="font-weight: normal;">Mer information finns i följande artiklar:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en begärandekö</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Skapa routningsregler</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planerade timmar</strong> </td> 
      <td> <p>Beräkna hur många timmar det skulle ta för den här begäran att slutföras.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planerat startdatum</strong> </td> 
      <td> <p>Det datum då arbetet med denna begäran ska starta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planerat slutförandedatum</strong> </td> 
      <td>Det datum då du vill att den här begäran ska lösas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>Standardstatusen för en ny begäran är "Ny". Din Workfront-administratör kan ha ändrat namnet på den här statusen. Du kan också ändra statusen till något annat i den här listrutan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dokument</strong> </td> 
      <td> <p>Lägg till dokument i din begäran. Dokumenten som bifogas den ursprungliga begäran överförs inte till den kopierade begäran.</p> <p><b>TIPS</b>

   Beroende på hur frågekö konfigurerades kan avsnittet Dokument visas före eller efter de anpassade fälten.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Valfritt) Uppdatera eventuell information i de anpassade formulären, om det behövs.

   >[!TIP]
   >
   >* Alla anpassade formulär som är kopplade till den ursprungliga begäran och värdena som är inkluderade i de anpassade fälten överförs till den kopierade begäran. Detta inkluderar fält som innehåller logik.
   >* Du kan inte ta bort anpassade formulär från den kopierade begäran.

1. Klicka **Skicka**.

   Den kopierade begäran skickas som en ny begäran i den begärandekö som du angav.
