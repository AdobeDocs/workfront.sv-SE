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
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Konfigurera tidslinjeomberäkningar för projekt

Genom att beräkna om tidslinjer kan chefer se hur krafter utanför projektet påverkar projektets tidslinje. Ett projekts tidslinje hänvisar till planerade och planerade datum för projektet.

Som en [!DNL Adobe Workfront] kan du manuellt beräkna om tidslinjer för alla projekt i systemet. Projektägare kan även manuellt beräkna om tidslinjer för enskilda projekt. Mer information finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

I den här artikeln beskrivs hur du, som [!DNL Workfront] administratör, kan bestämma hur och när [!DNL Workfront] beräknar automatiskt projekttidslinjer genom att konfigurera projektinställningar i [!UICONTROL Setup] område.

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
   <td> <p>Åtkomstnivå för systemadministratör</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera automatiska omberäkningar

Som en [!DNL Adobe Workfront] administratör kan du konfigurera när [!DNL Workfront] beräknar projekttidslinjer automatiskt om. [!DNL Workfront] kan beräkna om projekttidslinjer antingen varje natt eller när projektomfånget ändras, eller både och.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. I **[!UICONTROL Timelines]** aktiverar eller inaktiverar du en eller båda inställningarna nedan. Som standard är båda inställningarna aktiverade.

   * **Varje kväll:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] beräknar om tidslinjer på natten endast för projekt som har statusen [!UICONTROL Current] och uppdaterades de senaste tre månaderna.

      I detta fall [!DNL Workfront] beräknar om tidslinjen för alla projekt som har en [!UICONTROL Update Type] av [!UICONTROL Automatic] eller [!UICONTROL Automatic and On Change].

   * **När ett projekts omfång ändras**: Mer information om vad som utgör en ändring av projektets omfång finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      I detta fall [!DNL Workfront] beräknar om tidslinjen för alla projekt som har uppdateringstypen [!UICONTROL Automatic and On Change] eller [!UICONTROL On Change Only].
Mer information om projektets uppdateringstyper finns i [Översikt över uppdateringstyp för projekt](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klicka på **[!UICONTROL Save]**.

   Tidslinjen för alla projekt i systemet beräknas om automatiskt baserat på uppdateringstypen för varje projekt.

## Beräkna om tidslinjer för hela [!DNL Workfront] instance

Du kan köra [!UICONTROL Recalculate Timeline] diagnostik för att manuellt beräkna om alla tidslinjer i [!DNL Workfront] system. Detta gör att alla projektledare kan se hur externa ändringar påverkar direkt både planerade och planerade datum. Mer information finns i [Använd diagnostik för att starta automatiserade processer](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
