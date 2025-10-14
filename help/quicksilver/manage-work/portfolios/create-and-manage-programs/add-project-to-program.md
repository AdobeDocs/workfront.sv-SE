---
product-area: programs;projects
navigation-topic: create and manage programs
title: Lägg till ett projekt i ett program
description: Du kan ordna dina projekt genom att lägga till dem i program inom portföljer. Du kan ha flera projekt i ett program, men du kan bara associera ett program med ett projekt. Om du lägger till ett projekt i ett program läggs det automatiskt till i programmets portfölj samtidigt.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1fecc4d1-4c24-495c-98f5-824e13967369
source-git-commit: 78b4724ca8d5df15ed76e9e882179e3cb127282c
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Lägga till ett projekt i ett program

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

Du kan ordna dina projekt genom att lägga till dem i program inom portföljer. Du kan ha flera projekt i ett program, men du kan bara associera ett program med ett projekt.

Du måste skapa en portfölj och ett program i den här portföljen innan du kan lägga till ett projekt i ett program.

Om du lägger till ett projekt i ett program läggs det automatiskt till i programmets portfölj samtidigt.

Mer information om hur du skapar portföljer finns i [Skapa en portfölj](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

Mer information om hur du skapar program finns i [Skapa ett program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td><p>Nytt: Standard</p> 
   <p>Aktuell: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] tillgång till Program eller högre</p> <p>[!UICONTROL Edit] behörighet till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till programmet</p> <p>[!UICONTROL Manage] behörigheter till projekten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till ett projekt i ett befintligt program

1. Gå till ett program.

   Klicka på **[!UICONTROL Projects]** i den vänstra panelen.

1. Klicka på **[!UICONTROL New Project]** och välj en metod för att lägga till projektet.

   >[!TIP]
   >
   >Du kan inte lägga till ett projekt när du visar listan med projekt i vyn [!UICONTROL Milestone].

   Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>Lägg till ett projekt som redan har skapats.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>Lägg till ett nytt projekt från grunden. </p> <p>Mer information om hur du skapar ett projekt från grunden finns i <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Skapa ett projekt</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import a Project from [!DNL MS Project]] </td> 
      <td> <p>Lägg till ett projekt som du tidigare har exporterat från [!DNL MS Project] och sparat på datorn. </p> <p>Mer information om hur du skapar ett nytt projekt genom att importera det från [!DNL Microsoft Project] finns i <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Importera ett projekt från [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Begär att det nya projektet godkänns innan du kan börja arbeta med det.</p> <p>Mer information om hur du begär projekt finns i <a href="../../../manage-work/projects/create-projects/request-project.md">Begär ett projekt</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New from Template]</td> 
      <td> <p>Lägg till ett nytt projekt med en befintlig mall. </p> <p>Mer information om hur du skapar ett projekt från en mall finns i <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Skapa ett projekt med en mall</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om du valde **[!UICONTROL Existing Project]** öppnas rutan **Lägg till projekt** . <!--check at unshimming-->

   ![Lägg till befintliga projekt i programrutan](assets/add-projects-to-programs-box.png)<!--check at unshimming-->

1. Gör följande:

   1. I rutan **[!UICONTROL Add Projects]** skriver du namnet på ett projekt i fältet **Lägg till projekt i det här programmet** och markerar det när det visas i listan. <!--check casing on links and buttons-->

      Du kan lägga till fler än ett projekt.
   1. (Valfritt) Klicka på ikonen **Ta bort** ![Ta bort &#x200B;](assets/delete-icon.png) bredvid namnet på ett projekt om du bestämmer dig för att inte lägga till det i programmet.

   1. Klicka på **[!UICONTROL Add Projects]**. <!--check at unshimming-->

      Projektet visas på fliken **[!UICONTROL Projects]** i programmet och är nu associerat med programmet och programmets respektive portfölj.
