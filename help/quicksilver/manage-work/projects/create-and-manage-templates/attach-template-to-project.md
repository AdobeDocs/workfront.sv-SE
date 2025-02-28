---
product-area: templates
navigation-topic: templates-navigation-topic
title: Bifoga en mall till ett projekt
description: Du kan bifoga en mall till ett projekt antingen under den inledande fasen av projektet eller efter att det har skapats.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Bifoga en mall till ett projekt

Du kan bifoga en mall till ett projekt antingen under den inledande fasen av projektet eller efter att det har skapats.

Mer information om hur du skapar ett projekt med en mall finns i [Skapa ett projekt med en mall](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Åtkomstkrav

Du måste ha följande för att kunna utföra de steg som beskrivs i den här artikeln:

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
   <td> <p>Redigera åtkomst till projekt </p> <p>Mer information om projektåtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Bevilja åtkomst till projekt</a>.</p> <p>Visa åtkomst till mallar</p> <p>Mer information om mallbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Dela en mall</a>. </p> <p>Mer information om mallåtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Bevilja åtkomst till mallar</a>.</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet</p> <p>Mer information om projektbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>. </p> <p>Visa behörigheter eller högre till mallen</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Koppla en mall till ett befintligt projekt {#attach-a-template-to-an-existing-project}

Du kan bifoga en mall till ett projekt i Workfront från projektsidan eller från en projektlista eller rapport.

1. Gå till projektet där du vill bifoga en mall och klicka på ikonen **Mer** ![Mer ](assets/qs-more-icon-on-an-object.png) till höger om projektnamnet

   ![Fler listrutor](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   eller

   Gå till en projektlista eller rapport och välj ett projekt och klicka sedan på ikonen **Mer** ![Mer](assets/qs-more-icon-on-an-object.png) högst upp i listan.

   ![Mer meny utökad](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Klicka på **Bifoga mall**.

   Rutan Bifoga mall visas.

1. Börja skriva namnet på mallen som du vill bifoga i fältet **Sökmallar** och klicka sedan på den när den visas.i listan

   eller

   Klicka på namnet på en mall i området **Andra mallar**.

   En förhandsgranskning av mallen visas till höger som innehåller följande information om mallen:

   * Varaktighet
   * Ägare
   * Antalet uppgifter på den översta nivån (innehåller en lista över de tre första uppgifterna på den översta nivån)
   * Totalt antal uppgifter
   * Namn på kopplade anpassade formulär

   ![Koppla mallruta](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Valfritt) Klicka på ikonen **Favoriter** ![Favoriter](assets/favorites-icon-small.png) till vänster om mallnamnet för att markera det som en favorit. Detta flyttar mallen i favoritlistan.

   ![Ikonen Favoriter i malllistan](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Valfritt) Klicka på ikonen **Favoriter** ![Favoriter](assets/favorites-icon-selected.png) igen för att ta bort den från favoritlistan.
1. Klicka på **Anpassa och bifoga**.

   ![Koppla mall](assets/attach-template-large-box-nwe-350x262.png)

1. Uppdatera informationen i följande avsnitt innan du bifogar mallen (eller klicka på **Koppla mall** när som helst):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Avsnittet Uppgifter</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De valda malluppgifterna nedan importeras till projektet. Avmarkera de som du vill utesluta. </td> 
      <td>Avmarkera alla uppgifter som du vill utesluta från mallen innan du bifogar den till projektet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Välj den projektuppgift som du vill ha som föregångare för aktiviteterna i den här mallen.</td> 
      <td> <p>Klicka på fältet för att visa en lista med projektuppgifter. Välj vilken projektuppgift du vill avsluta innan malluppgifterna kan starta. Du kan också hoppa över det här steget och ställa in relationer inom projektet efter att mallen har bifogats. </p> <p> Välj informationen om <strong>beroendetyp</strong>, <strong>fördröjning</strong> och om du vill att föregående <strong>ska framtvingas</strong> eller inte. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Välj den projektuppgift som du vill ska vara överordnad uppgifterna i den här mallen.</td> 
      <td> Välj vilken projektuppgift som du vill ange som överordnad uppgift för alla malluppgifter. Om du inte gör något val visas alla malluppgifter i slutet av de aktuella projektaktiviteterna. Du kan hoppa över det här steget och flytta runt aktiviteter i projektet när mallen har bifogats.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Alternativavsnitt</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De valda objekten nedan överförs till projektet. Avmarkera de som du vill utesluta.</td> 
      <td> <p>Avmarkera kryssrutorna bredvid den information du vill ta bort från mallen innan du bifogar den till projektet. Den här informationen överförs inte från mallen till projektet. Mer information om varje fält finns i <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Översikt över hur du bifogar en mall till ett projekt</a>. </p> <p>Viktigt! Om du markerar kryssrutan <strong>Köegenskaper och inställningar för problem</strong> skriver köinformationen för mallen över projektets. I det här fallet läggs reglerna för routning, köämnen och ämnesgrupper i mallen till i projektets. <br>Om projektet har konfigurerats som en begärandekö och mallen som du bifogar till projektet inte har ställts in som en begärandekö, tas köinformationen bort om du inte markerar kryssrutan <strong>Köegenskaper och inställningar för problem</strong> . <br>Om du avmarkerar kryssrutan <strong>Köegenskaper och Utfärdandeinställningar</strong> bevaras alla inställningar för köinställningar för projektet och inga köinställningar från mallen bifogas. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Anpassat Forms-avsnitt</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td> <p>När anpassade formulär bifogas till mallen visas deras namn på den vänstra panelen. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Uppdatera information i anpassade formulär. Den här informationen överförs till projektet.

   >[!TIP]
   >
   >* Det här steget är obligatoriskt när de anpassade formulären i mallen innehåller obligatoriska fält som är tomma.
   >* Om fälten från de anpassade mallformulären redan finns i projektet och innehåller information, bevaras den information som redan finns i projektet. Du kan inte redigera dem när du bifogar mallen.

1. Klicka på **Bifoga mall.**
1. Klicka på **Avbryt bifogad fil** om du vill sluta koppla mallen.

   eller

   Tillåt att den bifogade filen slutförs för att lägga till mallen i projektet.

   När du har bifogat mallen kan du redigera projektet och justera uppgifter, information och inställningar efter behov.

1. (Valfritt) Klicka på **Projektinformation** och sedan på **Översikt** för att visa namnet på mallen som du bifogade i området **Projektrelationer**.

   >[!TIP]
   >
   >Om du kopplar mer än en mall till projektet visas bara den mall som du bifogade först i det här fältet. Mer information finns i avsnittet [Koppla flera mallar till ett befintligt projekt och visa mallinformation](#attach-multiple-templates-to-an-existing-project-and-view-template-information) i den här artikeln.

1. (Valfritt) Ta bort mallinformation från projektet där du bifogade mallen. Mer information finns i [Ta bort mallinformation från ett projekt](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Bifoga flera mallar till ett befintligt projekt och visa mallinformation {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Du kan bifoga flera mallar (en åt gången) till samma projekt, enligt stegen som beskrivs i avsnittet [Koppla en mall till ett befintligt projekt](#attach-a-template-to-an-existing-project) i den här artikeln. Detta lägger till uppgifter och annan information från varje mall i projektet.

>[!TIP]
>
>När du bifogar flera mallar till ett projekt visas endast den som du bifogade först i området Projektinformation.

Så här förstår du vilken mall som används i ett projekt:

1. Navigera till ett projekt som har en bifogad mall.
1. Klicka på **Projektinformation** i den vänstra panelen.
1. Hitta namnet på mallen som är kopplad till projektet i fältet **Mall** längst ned i avsnittet **Översikt** under **Projektrelationer** .

   ![Mallinformation i projekt](assets/nwe-template-info-on-project-350x356.png)


