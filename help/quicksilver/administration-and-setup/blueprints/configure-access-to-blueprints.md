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

Alla [!DNL Adobe Workfront]-användare kan bläddra i katalogen med utkast.

Som systemadministratör kan du:

* Lägg till [!UICONTROL Blueprints] på huvudmenyn i layoutmallar och tilldela layoutmallen till användare eller grupper. Mer information finns i [Anpassa [!UICONTROL Main Menu] med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) och [Tilldela användare till en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Användare som inte har tilldelats någon layoutmall kan se ikonen [!UICONTROL Blueprints] i [!UICONTROL Main Menu].
  >* När du skapar en ny layoutmall inkluderas ikonen [!UICONTROL Blueprints] som standard i listan [!UICONTROL Active Items] för [!UICONTROL Main Menu].


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
   <td role="rowheader"><strong>Adobe [!DNL Workfront]-licens</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar {#prerequisites}

* Du måste använda en befintlig begärandekö för att lagra begäranden om utkast. Projektet måste sparas som en begärandekö och måste ha statusen [!UICONTROL Current].
* Begärandekön måste vara offentlig. I informationen om begärandekön måste [!UICONTROL Who can add requests to this queue?] anges till **[!UICONTROL Anyone]**.

>[!TIP]
>
>Om du vill skapa en ny begärandekö för begäranden om utkast bör du skapa den innan du konfigurerar åtkomst till utkast. Mer information om hur du skapar en begärandekö finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Välj begärandekön för att lagra begäran om utkast

Innan användare kan begära att du installerar utkast för dem måste du välja en begärandekö för dessa begäranden. Tills kön med begäranden har definierats kan användare bara bläddra i katalogen med utkast.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Blueprints]**.
1. Klicka på **[!UICONTROL Configure blueprint requests]** överst till höger på katalogskärmen.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. I dialogrutan **[!UICONTROL Configure blueprints]** börjar du skriva namnet på en aktiv begärandekö och markerar den när den visas i sökresultatet.

   >[!IMPORTANT]
   >
   >Endast offentliga begärandeköer visas i den här listan. Se avsnittet [Förutsättningar](#prerequisites) ovan om du vill göra din begärandekö offentlig.

   Inställningen för begärandekön är inställd och användare kan nu begära installation av utkast.

   ![Konfigurera begärandekö](assets/Blueprints_access_setup_request_queue.png)

1. (Valfritt) Klicka på **[!UICONTROL Edit this request queue]** om du vill göra ändringar i den faktiska begärandekön.

   Kö-projektet för begäran öppnas på en ny flik i webbläsaren och du kan uppdatera det efter behov.

1. (Valfritt) Om begärandekön innehåller ämnesgrupper eller köämnen kan du välja dem i listan.
1. Klicka på **[!UICONTROL Close]** om du vill återgå till katalogen med utkast.

>[!NOTE]
>
>När du installerar en begärd plan bör du ändra utgivningsstatusen till **[!UICONTROL Closed]** eller **[!UICONTROL Resolved]** i kön så att den som gjorde begäran meddelas. Information om hur du installerar en plan finns i [Installera en plan](../../administration-and-setup/blueprints/blueprints-install.md).
