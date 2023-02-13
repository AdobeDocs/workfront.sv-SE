---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera utleveransstatus
description: Du kan uppdatera status för ett problem för att informera andra om var problemet finns och hur det utvecklas.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Uppdatera utleveransstatus

Du kan uppdatera status för ett problem för att informera andra om var problemet finns och hur det utvecklas.

## Åtkomstkrav

<!--drafted for P&P;

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
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Hantera behörigheter för problemet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Utfärdandestatus

Följande är standardstatusvärden för problem i Workfront:

* Nytt
* Pågår
* Väntar på feedback
* Parkerad
* Lös inte
* Återöppnad
* Stängd
* Löst

Din Adobe Workfront-administratör kan lägga till anpassade statusvärden för problem i din organisation. De kan också göra statusar tillgängliga beroende på vilken typ av problem det gäller.

Mer information om anpassade statusvärden och problemtyper finns i följande artiklar:

* [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Skapa problem](../../../manage-work/issues/manage-issues/create-issues.md)

Du kan uppdatera utgivningsstatus manuellt eller låta Workfront uppdatera dem automatiskt när vissa åtgärder utförs.

## Uppdatera utgivningsstatus manuellt

När du uppdaterar en utgivningsstatus kan du även lägga till en förklaring om den nya statusen och ändra annan utgivningsinformation, t.ex. utfästelsedatumet.

1. Gå till en utgåva som du har tilldelats och som du vill uppdatera statusen för.
1. Klicka på **Status** i utgivningsrubriken och välj en ny status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. Dra eller dubbelklicka på bubblan under för att få en visuell indikation på att problemet har åtgärdats **Procent färdigt** i ärendets rubrik.

   eller

   Klicka i bubblan i huvudet på utgåvan för att ange en procentsats.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Valfritt) Gör något av följande för att ange ytterligare information om uppdateringen och klicka sedan på **Uppdatera** eller, om utgåvan har en status som är lika med Fullständig, klicka på **Klart:**

   * Om du vill lägga till en anteckning om uppdateringen går du till **Uppdateringar** och klicka **Starta en ny uppdatering** och skriver sedan din anteckning.

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Om du vill meddela vissa användare om uppdateringen skriver du deras namn i **Meddela** som visas när du skriver en anteckning om uppdateringen. Mer information finns i [Tagga andra för uppdateringar](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Om du vill uppdatera problemets skick klickar du på **Villkor** väljer du det villkor som bäst återspeglar problemets aktuella tillstånd. Välj bland följande alternativ:

      * Går smidigt
      * Vissa bekymmer
      * Större vägspärrar
   * Om du vill uppdatera datumet för implementeringen av utgåvan expanderar du **Bekräftelsedatum** och välj ett nytt datum.


## Uppdatera utgivningsstatus automatiskt

Workfront uppdaterar automatiskt status för en utgåva till en annan status när åtgärderna som listas i tabellen nedan inträffar.

>[!NOTE]
>
>Statuserna i följande tabell är standardsystemstatusar. Din Workfront-administratör eller en gruppadministratör kan byta namn på statusarna i din instans av Workfront. Mer information om hur du skapar och hanterar statusar i Workfront finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Åtgärd</td> 
   <td>Ursprunglig status</td> 
   <td>Ny status</td> 
  </tr> 
  <tr> 
   <td>Uppdatera utleveransprocenten till 100 %</td> 
   <td>Nytt eller Pågående</td> 
   <td>Stängd</td> 
  </tr> 
  <tr> 
   <td>Uppdatera utleveransprocenten från 100 % till ett lägre antal</td> 
   <td>Stängd </td> 
   <td>Pågår</td> 
  </tr> 
  <tr> 
   <td>Uppdatera statusen för ett objekt som är kopplat till problemet</td> 
   <td>Olika statusar</td> 
   <td> <p>Olika statusar</p> <p>Mer information om hur du löser objekt och hur de påverkar status för problem finns i avsnittet Synkronisera status för det lösta objektet med statusen för det lösta objektet i artikeln <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över upplösta och upplösta objekt </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicka på knappen Starta problem för att godkänna att du arbetar med ett problem som du har tilldelats</span> </td> 
   <td><span>Nytt</span> </td> 
   <td> <p>Status som är associerad med knappen Starta problem i inställningarna för ditt hemteam. </p> <p>Mer information om hur du ersätter knappen Work On It (Arbeta på den) med knappen Start Issue (Starta problem) finns i <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersätta knappen Work On It (Arbeta på) med en Start-knapp</a></span><span>.</span> </p> <p>Tips: Klicka <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">knappen Ångra</span> när du klickat på Starta problem återställs statusen till Nytt. </p> </td> 
  </tr> 
 </tbody> 
</table>
