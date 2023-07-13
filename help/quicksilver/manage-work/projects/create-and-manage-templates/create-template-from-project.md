---
product-area: templates
navigation-topic: templates-navigation-topic
title: Skapa mall från projekt
description: Du kan skapa mallar när du sparar ett befintligt projekt som en mall.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '477'
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

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mallar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i ett projekt </p> <p>Du får behörigheten Hantera för mallen när du har skapat den</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa mall från projekt

1. Gå till det projekt som du vill spara som en mall.
1. Klicka på **Mer** meny ![](assets/qs-more-icon-on-an-object.png)sedan **Spara som mall**.
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
      <td>Använd listrutan för att välja anpassade formulär som ska bifogas mallen. Om några anpassade formulär redan har associerats med projektet visas alla datafält från dessa anpassade formulär.<br>Du kan inkludera upp till 10 anpassade formulär i en och samma mall.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Hantera Forms** för att ta bort eller ordna om formulären. Mer information om hur du tar bort och ändrar ordning på anpassade formulär i mallen finns i [Egna formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Klicka **Nästa steg.**
1. I **Alternativ** markerar du kryssrutan bredvid information som du vill ta bort från mallen.

   ![](assets/save-as-template-options-step-350x109.png)

1. Klicka **Nästa steg.**
1. I **Exkludera** väljer du de uppgifter som du vill utesluta från projektet.

   ![](assets/save-as-template-exclude-350x205.png)

1. Klicka **Slutför och spara mall.**

   Mallen visas nu i listan med tillgängliga mallar och kan antingen bifogas till ett befintligt projekt eller användas för att skapa ett nytt.

 
