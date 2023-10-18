---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera aktivitetsstatus
description: Du kan uppdatera en uppgifts status för att informera andra om var uppgiften är (och det övergripande projektet) och hur den fortskrider.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Uppdatera aktivitetsstatus

Du kan uppdatera en uppgifts status för att informera andra om var uppgiften är (och det övergripande projektet) och hur den fortskrider.

Standardstatusvärdena är Nytt, Pågår och Fullständigt. Din Adobe Workfront-administratör kan lägga till anpassade statusvärden för din organisation. Mer information finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Du kan uppdatera uppgiftsstatus manuellt eller låta Workfront uppdatera dem automatiskt när vissa åtgärder utförs.

## Åtkomstkrav

<!--drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande åtkomst för att kunna uppdatera uppgifter manuellt:

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för uppgiften</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du uppdaterar aktiviteternas status

* När du markerar en uppgift som slutförd uppdateras procentandelen slutförd till 100 %.
* Följande scenarier finns för överordnade uppgifter:
   * Du kan inte uppdatera statusen för en överordnad aktivitet till Fullständig när läget Sammanfattning av slutförande för projektet är inställt på Automatisk och underaktiviteterna inte slutförs.
   * Du kan uppdatera statusen för en överordnad aktivitet till Fullständig när läget Sammanfattning av slutförande för projektet är inställt på Manuell och underaktiviteterna är slutförda eller ofullständiga.

  Mer information finns i [Redigera projekt](../manage-projects/edit-projects.md).

## Uppdatera aktivitetsstatus manuellt

När du uppdaterar en aktivitetsstatus kan du även skriva en förklaring till den nya statusen och ändra annan aktivitetsinformation, t.ex. förfallodatumet.

1. Gå till en uppgift som du är tilldelad till och som du vill uppdatera statusen för.
1. Klicka på **Status** i uppgiftshuvudet och välj en ny status.
1. (Valfritt) Gör något av följande för att ange ytterligare information om uppdateringen och klicka sedan på **Uppdatera** eller, om uppgiften har **Complete** status, klicka **Klart:**

   * Om du vill lägga till en anteckning om uppdateringen går du till **Uppdateringar** område och klicka **Starta en ny uppdatering** och skriver sedan din anteckning.

   * Om du vill meddela vissa användare om uppdateringen skriver du deras namn i **Meddela** som visas när du skriver en anteckning om uppdateringen. Mer information finns i [Tagga andra för uppdateringar](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Om du vill uppdatera villkoret för uppgiften klickar du på **Välj villkor** till höger om **Meddela** (dessa visas när du skriver en anteckning om uppdateringen) och väljer sedan det villkor som bäst motsvarar det aktuella villkoret för uppgiften.

   * Om du vill uppdatera aktivitetens implementeringsdatum expanderar du **Bekräftelsedatum** och välj ett nytt implementeringsdatum.
   * Om du vill få en visuell indikation på slutförd uppgift drar du bubblan under Procent färdigt eller dubbelklickar på den för att ange ett procentvärde.\
     ![](assets/drag-the-progress-bar-350x155.png)

## Uppdatera aktivitetsstatus automatiskt

Workfront uppdaterar automatiskt den befintliga statusen för en aktivitet till en annan status när åtgärderna som anges i tabellen nedan inträffar.

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
   <td>Uppdatera aktivitetsprocenten slutförd till 100 %</td> 
   <td>Nytt eller Pågående</td> 
   <td>Complete</td> 
  </tr> 
  <tr> 
   <td>Uppdatera procent färdigt för aktiviteten från 100 % till ett lägre tal</td> 
   <td>Complete</td> 
   <td>Pågår</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicka på knappen Starta uppgift för att acceptera att arbeta med en uppgift som du har tilldelats</span> </td> 
   <td><span>Nytt</span> </td> 
   <td> <p>Status som är associerad med knappen Starta uppgift i inställningarna för Hemteam.</p> <p>Mer information om hur du ersätter knappen Arbeta på den med knappen Starta uppgift finns i <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersätta knappen Work On It (Arbeta på) med en Start-knapp</a></span>.</p> <p>Tips: <span>Klicka</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">knappen Ångra</span>när du klickat på Starta uppgift återställs statusen till Ny. </p> </td> 
  </tr> 
 </tbody> 
</table>
