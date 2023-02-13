---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Konfigurera åtkomst till ritningar
description: Som systemadministratör kan du ge användare åtkomst att begära installation av utkast genom att ställa in en begärandekö där förfrågningarna lagras. Där har du en plats där du kan spåra och uppdatera begäranden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Konfigurera åtkomst till ritningar

Alla [!DNL Adobe Workfront] -användare kan bläddra i katalogen med ritningar.

Som systemadministratör kan du:

* Lägg till [!UICONTROL Blueprints] till huvudmenyn i layoutmallar och tilldela layoutmallen till användare eller grupper. Mer information finns i [Anpassa [!UICONTROL Main Menu] använda en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) och [Tilldela användare till en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* Användare som inte har tilldelats någon layoutmall kan se [!UICONTROL Blueprints] ikonen i [!UICONTROL Main Menu].
   >* När du skapar en ny layoutmall [!UICONTROL Blueprints] ikonen finns i [!UICONTROL Active Items] listan för [!UICONTROL Main Menu] som standard.



* Ge användare åtkomst att begära installation av utkast genom att ställa in en begärandekö där förfrågningarna lagras. Där har du en plats där du kan spåra och uppdatera begäranden. Mer information får du genom att följa proceduren nedan.
* Installera utkast. Mer information finns i [Installera en plan](../../administration-and-setup/blueprints/blueprints-install.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licens</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar {#prerequisites}

* Du måste använda en befintlig begärandekö för att lagra begäranden om utkast. Projektet måste sparas som en begärandekö och måste finnas i [!UICONTROL Current] status.
* Begärandekön måste vara offentlig. I informationen om begärandekön: &quot;[!UICONTROL Who can add requests to this queue?]&quot; måste anges till **[!UICONTROL Anyone]**.

>[!TIP]
>
>Om du vill skapa en ny begärandekö för begäranden om utkast bör du skapa den innan du konfigurerar åtkomst till utkast. Mer information om hur du skapar en frågekö finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Välj begärandekön för att lagra begäran om utkast

Innan användare kan begära att du installerar utkast för dem måste du välja en begärandekö för dessa begäranden. Tills kön med begäranden har definierats kan användare bara bläddra i katalogen med utkast.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Blueprints]**.
1. Klicka **[!UICONTROL Configure blueprint requests]** längst upp till höger på katalogskärmen.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. På **[!UICONTROL Configure blueprints]** börjar du skriva namnet på en aktiv begärandekö och markerar den när den visas i sökresultatet.

   >[!IMPORTANT]
   >
   >Endast offentliga begärandeköer visas i den här listan. Om du vill göra din begärandekö offentlig går du till [Förutsättningar](#prerequisites) ovan.

   Inställningen för begärandekön är inställd och användare kan nu begära installation av utkast.

   ![Konfigurera begärandekö](assets/Blueprints_access_setup_request_queue.png)

1. (Valfritt) Om du vill göra ändringar i den faktiska begärandekön klickar du på **[!UICONTROL Edit this request queue]**.

   Kö-projektet för begäran öppnas på en ny flik i webbläsaren och du kan uppdatera det efter behov.

1. (Valfritt) Om begärandekön innehåller ämnesgrupper eller köämnen kan du välja dem i listan.
1. Om du vill gå tillbaka till katalogen med utkast klickar du på **[!UICONTROL Close]**.

>[!NOTE]
>
>När du installerar en begärd plan bör du ändra utgivningsstatusen till **[!UICONTROL Closed]** eller **[!UICONTROL Resolved]** i begärandekön så att begäraren meddelas. Mer information om hur du installerar en plan finns i [Installera en plan](../../administration-and-setup/blueprints/blueprints-install.md).
