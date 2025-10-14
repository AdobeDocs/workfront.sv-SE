---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Ta bort och inaktivera portföljer
description: Portföljer är samlingar av projekt eller program i Adobe Workfront. Du kan ta bort eller inaktivera en portfölj om du upptäcker att den inte är relevant för ditt system.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 03c1f17504846fc4b8c4114ddc32df687281bc07
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Ta bort och inaktivera portföljer

<!--Audited: 2/2024-->

Portföljer är samlingar av projekt eller program i [!DNL Adobe Workfront]. Du kan ta bort eller inaktivera en portfölj om du upptäcker att den inte är relevant för ditt system.

Vi rekommenderar att du inaktiverar en portfölj som inte längre behöver kopplas till framtida projekt i stället för att ta bort den, för att behålla den historiska informationen om de projekt som för närvarande är kopplade till portföljen och dess program.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] tillgång till projekt och portföljer</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörigheter för portföljen </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över borttagning och inaktivering av portföljer

Tänk på följande när du bestämmer dig för att ta bort eller inaktivera portföljer:

* Om du tar bort en portfölj tas de program som är kopplade till den bort.

  >[!IMPORTANT]
  >
  >Du behöver inte ha behörighet till program för att kunna ta bort portföljen.

* När du tar bort en portfölj tas inte de projekt som är kopplade till den bort.
* Du kan inte återställa borttagna portföljer.
* Genom att inaktivera en portfölj säkerställs att namnet på portföljen och dess program inte längre kan tilldelas till projekt när du skapar ett projekt.
* Om du inaktiverar en portfölj som redan är kopplad till ett projekt tas den inte bort från projektet. Om du tar bort en inaktiverad portfölj från ett projekt måste du återaktivera den innan du kan koppla den till projektet igen.

## Ta bort en portfölj

{{step1-to-portfolios}}

1. Gör något av följande:

   * Markera portföljen i listan och klicka sedan på ikonen **[!UICONTROL Delete]** ![Ta bort](assets/delete.png) .
   * Klicka på portföljen för att öppna den, klicka sedan på menyn **Mer** ![Mer](assets/more-icon.png) till höger om portföljnamnet och klicka sedan på **Ta bort Portfolio**.
1. Bekräfta genom att klicka på **[!UICONTROL Yes, Delete It]**.

   Portföljen tas bort och kan inte återställas.

## Inaktivera en portfölj

När du inaktiverar en portfölj kan du fortfarande komma åt den från området [!UICONTROL Portfolios], men den visas inte längre i listan över portföljer när användare försöker lägga till den i ett projekt.

>[!NOTE]
>
>Beroende på hur din [!DNL Workfront]- eller gruppadministratör konfigurerar din layoutmall kanske [!UICONTROL Portfolios]-området inte visas i [!UICONTROL Main Menu]. Mer information finns i [Anpassa huvudmenyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Klicka på **[!UICONTROL Portfolios]** .
1. Klicka på namnet på portföljen.
1. Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-icon.png) till höger om portföljnamnet och klicka sedan på **[!UICONTROL Deactivate Portfolio]**.
Portföljen inaktiveras omedelbart.
1. (Valfritt) Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-icon.png) till höger om portföljnamnet och klicka sedan på **[!UICONTROL Activate Portfolio]** för att återaktivera det.


