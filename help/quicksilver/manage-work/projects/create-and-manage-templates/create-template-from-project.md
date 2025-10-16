---
product-area: templates
navigation-topic: templates-navigation-topic
title: Skapa mall från projekt
description: Du kan skapa mallar när du sparar ett befintligt projekt som en mall.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Skapa mall från projekt

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
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/qs-more-icon-on-an-object.png) och sedan på **Spara som mall**.
1. Ange följande information för mallen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
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
     <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td>Använd listrutan för att välja anpassade formulär som ska bifogas mallen. Om några anpassade formulär redan har associerats med projektet visas alla datafält från dessa anpassade formulär.<br>Du kan inkludera upp till 10 anpassade formulär i en enda mall.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Hantera Forms** om du vill ta bort eller ordna om formulären. Mer information om hur du tar bort och ändrar ordning på anpassade formulär i mallen finns i [Anpassade formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![Spara som mall, första steget](assets/save-as-template-first-step-350x159.png)

1. Klicka på **Nästa steg.**
1. I avsnittet **Alternativ** markerar du kryssrutan bredvid eventuell information som du vill ta bort från mallen.

   ![Alternativ för Spara som mall](assets/save-as-template-options-step-350x109.png)

1. Klicka på **Nästa steg.**
1. I avsnittet **Uteslut** väljer du de uppgifter du vill utesluta från projektet.

   ![Spara som mall exkludera](assets/save-as-template-exclude-350x205.png)

1. Klicka på **Slutför och spara mall.**

   Mallen visas nu i listan med tillgängliga mallar och kan antingen bifogas till ett befintligt projekt eller användas för att skapa ett nytt.

 
