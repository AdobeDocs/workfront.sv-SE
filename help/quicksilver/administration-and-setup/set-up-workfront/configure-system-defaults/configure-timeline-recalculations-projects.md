---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Konfigurera tidslinjeomberäkningar för projekt
description: Genom att beräkna om tidslinjer kan chefer se hur krafter utanför projektet påverkar projektets tidslinje. Ett projekts tidslinje hänvisar till planerade och planerade datum för projektet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Konfigurera tidslinjeomberäkningar för projekt

Genom att beräkna om tidslinjer kan chefer se hur krafter utanför projektet påverkar projektets tidslinje. Ett projekts tidslinje hänvisar till planerade och planerade datum för projektet.

Som [!DNL Adobe Workfront]-administratör kan du manuellt beräkna om tidslinjer för alla projekt i systemet. Projektägare kan även manuellt beräkna om tidslinjer för enskilda projekt. Mer information finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

I den här artikeln beskrivs hur du som [!DNL Workfront]-administratör kan bestämma hur och när [!DNL Workfront] automatiskt beräknar projekttidslinjer genom att konfigurera projektinställningar i området [!UICONTROL Setup].

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Åtkomstnivå för systemadministratör</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera automatiska omberäkningar

Som [!DNL Adobe Workfront]-administratör kan du konfigurera när [!DNL Workfront] automatiskt beräknar om projekttidslinjer. [!DNL Workfront] kan beräkna om projekttidslinjer antingen varje kväll eller när projektomfånget ändras, eller både och.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet eller på ikonen [!UICONTROL **Huvudmeny**] ![](assets/lines-main-menu.png) i det övre vänstra hörnet av [!DNL Workfront], om den är tillgänglig, och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. Aktivera eller inaktivera en eller båda av inställningarna nedan i avsnittet **[!UICONTROL Timelines]**. Som standard är båda inställningarna aktiverade.

   * **Varje kväll:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] beräknar om tidslinjer en gång var 24:e timme, på natten, endast för projekt som har statusen [!UICONTROL Current] och som har uppdaterats de senaste tre månaderna. Beroende på systembelastningen och andra faktorer kan omberäkningstiden fördröjas med mer än 24 timmar.

     I det här fallet beräknar [!DNL Workfront] om tidslinjen för alla projekt som har [!UICONTROL Update Type] [!UICONTROL Automatic] eller [!UICONTROL Automatic and On Change].

   * **När ett projekts omfång ändras**: Mer information om vad som utgör en ändring av projektomfång finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     I det här fallet beräknar [!DNL Workfront] om tidslinjen för alla projekt som har uppdateringstypen [!UICONTROL Automatic and On Change] eller [!UICONTROL On Change Only].
Mer information om typer av projektuppdateringar finns i [Översikt över projektuppdateringstyper](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klicka på **[!UICONTROL Save]**.

   Tidslinjen för alla projekt i systemet beräknas om automatiskt baserat på uppdateringstypen för varje projekt.

## Beräkna om tidslinjer för hela [!DNL Workfront]-instansen

Du kan köra diagnostiken för [!UICONTROL Recalculate Timeline] för att manuellt beräkna om alla tidslinjer i systemet [!DNL Workfront]. Detta gör att alla projektledare kan se hur externa ändringar påverkar direkt både planerade och planerade datum. Mer information finns i [Använda diagnostik för att starta automatiska processer](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
