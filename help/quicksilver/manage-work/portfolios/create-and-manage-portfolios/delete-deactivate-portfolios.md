---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Ta bort och inaktivera portföljer
description: Portfolio är samlingar av projekt eller program i Adobe Workfront. Du kan ta bort eller inaktivera en portfölj om du upptäcker att den inte är relevant för ditt system.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Ta bort och inaktivera portföljer

Portfolio är samlingar av projekt eller program i [!DNL Adobe Workfront]. Du kan ta bort eller inaktivera en portfölj om du upptäcker att den inte är relevant för ditt system.

Vi rekommenderar att du inaktiverar en portfölj som inte längre behöver kopplas till framtida projekt i stället för att ta bort den, för att behålla den historiska informationen om de projekt som för närvarande är kopplade till portföljen och dess program.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL Edit] behörighet till projekt och Portfolio</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörigheter för portföljen </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Översikt över borttagning och inaktivering av portföljer

Tänk på följande när du bestämmer dig för att ta bort eller inaktivera portföljer:

* Om du tar bort en portfölj tas de program som är kopplade till den bort.

  >[!IMPORTANT]
  >
  >Du behöver inte ha behörighet till program för att kunna ta bort portföljen.

* När du tar bort en portfölj tas inte de projekt som är kopplade till den bort.
* Du kan inte återställa borttagna portföljer.
* Genom att inaktivera en portfölj säkerställs att namnet på portföljen och dess program inte längre kan tilldelas till projekt när du skapar ett projekt.

## Inaktivera en portfölj

När du inaktiverar en portfölj kan du fortfarande komma åt den från [!UICONTROL Portfolios] men visas inte längre i portföljlistan när användare försöker lägga till den i ett projekt.

>[!NOTE]
>
>Beroende på hur [!DNL Workfront] eller gruppadministratören konfigurerar layoutmallen [!UICONTROL Portfolios] området kanske inte visas i [!UICONTROL Main Menu]. Mer information finns i [Anpassa huvudmenyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront].

1. Klicka på **[!UICONTROL Portfolios]** .
1. Klicka på namnet på portföljen.
1. Klicka på Mer-menyn ![](assets/more-icon.png) till höger om portföljnamnet och klicka sedan på **[!UICONTROL Deactivate Portfolio]**.

## Ta bort en portfölj

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn.

1. Klicka på **[!UICONTROL Portfolios]** .
1. Välj portföljen och klicka sedan på **[!UICONTROL Delete]**&#x200B; [!UICONTROL Delete] icon ![](assets/delete.png).
1. Klicka i rutan som visas **[!UICONTROL Yes, Delete It]** för att bekräfta.
