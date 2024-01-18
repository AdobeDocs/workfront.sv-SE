---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera utgivningsstatus
description: Du kan uppdatera status för ett problem för att informera andra om var problemet finns och hur det utvecklas.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Uppdatera utgivningsstatus

<!--Audited: 01/2024-->

Du kan uppdatera status för ett problem för att informera andra om var problemet finns och hur det utvecklas.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Ny licens: Medarbetare eller högre</p>
   eller
   <p>Aktuell licens: Begär eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Du kan uppdatera problemstatusen i följande områden i Workfront:

* Utgivningsrubriken på uppgiftssidan.
* Rutan Redigera problem när du redigerar ett problem.
* Avsnittet Information på utgivningssidan.
* I en problemlista eller rapport när statusfältet visas i vyn.
* På panelen Sammanfattning av problemet.

Så här uppdaterar du utgivningsstatusen manuellt i utgivningsrubriken:

1. Gå till ett problem som du vill uppdatera statusen för.
1. Klicka på **Status** i utgivningsrubriken och välj en ny status.
1. Dra eller dubbelklicka på bubblan under för att få en visuell indikation på att problemet har åtgärdats **Procent färdigt** i utgåvans rubrik

   eller

   Klicka i bubblan i huvudet på utgåvan för att ange en procentsats.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Valfritt) Gör något av följande för att ange ytterligare information om uppdateringen:

   * Om du vill lägga till en anteckning om uppdateringen går du till **Uppdateringar** och klicka **Ny kommentar** och skriv sedan en anteckning.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Om du vill meddela vissa användare om uppdateringen skriver du deras namn i **Tagga personer eller team** fält som visas när du skriver en kommentar. Mer information finns i [Tagga andra för uppdateringar](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Om du vill uppdatera datumet för implementeringen av felet klickar du på **Ärendeinformation** och sedan redigera **Bekräftelsedatum** fält. Mer information finns i [Redigera problem](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Endast utgivare kan uppdatera implementeringsdatumet.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

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
   <td><b>Åtgärd</b></td> 
   <td><b>Ursprunglig status</b></td> 
   <td><b>Ny status</b></td> 
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
   <td> <p>Olika statusar</p> <p>Mer information om hur du löser objekt och hur de påverkar status för problem finns i avsnittet Synkronisera status för det lösta objektet med statusen för det lösta objektet i artikeln <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över objekt som kan lösas och lösas </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicka på knappen Starta problem för att godkänna att du arbetar med ett problem som du har tilldelats</span> </td> 
   <td><span>Nytt</span> </td> 
   <td> <p>Status som är associerad med knappen Starta problem i inställningarna för ditt hemteam. </p> <p>Mer information om hur du ersätter knappen Work On It (Arbeta på den) med knappen Start Issue (Starta problem) finns i <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersätta knappen Work On It (Arbeta på) med en Start-knapp</a></span><span>.</span> </p> <p>Tips: Klicka <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">knappen Ångra</span> när du klickat på Starta problem återställs statusen till Nytt. </p> </td> 
  </tr> 
 </tbody> 
</table>
