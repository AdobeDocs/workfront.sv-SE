---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Konfigurera tidslinjeomberäkningar för projekt
description: Genom att beräkna om tidslinjer kan chefer se hur krafter utanför projektet påverkar projektets tidslinje. Ett projekts tidslinje hänvisar till planerade och planerade datum för projektet.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Konfigurera tidslinjeomberäkningar för projekt

Genom att beräkna om tidslinjer kan chefer se hur krafter utanför projektet påverkar projektets tidslinje. Ett projekts tidslinje hänvisar till planerade och planerade datum för projektet.

Som [!DNL Adobe Workfront]-administratör kan du manuellt beräkna om tidslinjer för alla projekt i systemet. Projektägare kan även manuellt beräkna om tidslinjer för enskilda projekt. Mer information finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

I den här artikeln beskrivs hur du som [!DNL Workfront]-administratör kan bestämma hur och när [!DNL Workfront] automatiskt beräknar projekttidslinjer genom att konfigurera projektinställningar i området [!UICONTROL Setup].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: [!UICONTROL Standard]</p>
   eller
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera automatiska omberäkningar

Som [!DNL Adobe Workfront]-administratör kan du konfigurera när [!DNL Workfront] automatiskt beräknar om projekttidslinjer. [!DNL Workfront] kan beräkna om projekttidslinjer antingen varje kväll eller när projektomfånget ändras, eller både och.

{{step-1-to-setup}}

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
