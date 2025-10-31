---
product-area: templates
navigation-topic: templates-navigation-topic
title: Skapa mall från projekt
description: Du kan skapa mallar när du sparar ett befintligt projekt som en mall.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Skapa mall från projekt

<!--Audited: 10/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

Du kan skapa mallar när du sparar ett befintligt projekt som en mall.

När du har sparat ett befintligt projekt som en mall kan du använda den nya mallen för att skapa nya projekt. Detta förenklar och snabbar upp processen att skapa projekt.

>[!NOTE]
>
>När du sparar ett projekt som en mall sparas inte de faktiska datumen för uppgifterna och projektet för mallen.
>
>En mall och dess uppgifter har inga faktiska datum, utan snarare en indikation på vilken dag (från när det framtida projektet kan starta) en aktivitet kan starta och vilken dag aktiviteten kan behöva slutföras. När du använder mallar för att skapa framtida projekt får projekten faktiska datum. Mer information finns i [Skapa ett projekt](../create-projects/create-project.md).

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
   <td> <p>Redigera åtkomst till mallar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i ett projekt </p> <p>När du har skapat mallen får du behörigheten Hantera</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Skapa mall från projekt

1. Gå till det projekt som du vill spara som en mall.
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) och sedan på **Spara som mall**.
1. Ange följande information för mallen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mallnamn</td> 
      <td>Ange ett namn för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Ja</strong>: Andra användare kan hitta mallen och bifoga den till projekt.</p> </li> 
        <li><strong>Nej</strong>: Andra användare kan inte hitta mallen och kan inte bifoga den till projekt.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Egen Forms** i den vänstra panelen.
1. Klicka på fältet **Lägg till anpassat formulär** och börja skriva namnet på ett projekt som är anpassat för, eller välj ett från listan.

   Om det redan finns anpassade formulär kopplade till projektet visas all information i de befintliga fälten från dessa anpassade formulär i formulären.

   Du kan inkludera upp till 10 anpassade formulär i en och samma mall.

1. Håll muspekaren över namnet på ett formulär och klicka sedan för att dra och släppa det på en ny plats.

   ![Spara projektet som mallsida högst upp i rutan](assets/save-project-as-template-top-of-the-form.png)

1. Klicka på **Alternativ** i den vänstra panelen och markera sedan de fält eller objekt som du vill överföra till mallen.

   Alla objekt är markerade som standard. Avmarkerade objekt överförs inte till mallen.

   ![Alternativ för Spara som mall](assets/save-project-as-template-options-area.png)

1. Klicka på **Uteslut** i den vänstra panelen och välj sedan de uppgifter som du vill utesluta från projektet.

   ![Spara som mall exkludera](assets/save-project-as-template-exclude-area.png)

1. Klicka på **Slutför och spara mall.**

   Mallen visas nu i listan över tillgängliga mallar. Användarna kan antingen bifoga den nya mallen till ett befintligt projekt eller använda den för att skapa ett projekt.


