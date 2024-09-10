---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Lås eller lås upp projektinställningar för alla grupper i systemet
description: Grupper i din organisation kan behöva en projektinställning som är annorlunda konfigurerad för sina unika arbetsflöden. Du kan låsa upp inställningen för alla grupper i hela organisationen så att de kan konfigurera den på egen hand.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Låsa eller låsa upp projektinställningar för alla grupper i systemet

Grupper i din organisation kan behöva en projektinställning som är annorlunda konfigurerad för sina unika arbetsflöden. Du kan låsa upp inställningen för alla grupper i hela organisationen så att de kan konfigurera den på egen hand.

När en inställning är olåst och gruppadministratören ändrar den, hämtas konfigurationen för den inställningen från gruppnivåinställningen i stället för från systemnivåinställningen för de projekt som är kopplade till gruppen.

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

## Om låsta och olåsta inställningar

Genom att låsa ett projekt, en uppgift eller en utgåva som du har konfigurerat på systemnivå kan du vara säker på att alla använder samma inställning för den inställningen. Även om du fortfarande kan konfigurera om en inställning som du låser kan gruppadministratörer inte konfigurera om den för sina grupper.

Om du låser upp ett projekt, en uppgift eller en utgåva blir gruppadministratörerna mer flexibla när det gäller att hantera hur deras grupper arbetar med objekten. När en inställning är olåst kan gruppadministratörer konfigurera om den för sina grupper.

Om ett fält inte har en lås/lås upp-knapp kan det inte låsas upp för gruppadministratörer för att konfigurera inställningar på gruppnivå. Konfigurationen är bara tillgänglig på systemnivå.

Instruktioner om hur du låser eller låser upp ett projekt, en uppgift eller en utgåva på systemnivå finns i [Konfigurera uppgifter och utgåvinställningar för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>När en [!DNL Workfront]-administratör har låst upp en inställning på systemnivå kan alla gruppadministratörer konfigurera den och sedan låsa den för att se till att alla i gruppen och undergrupperna nedan använder samma konfiguration. Detta är parallellt med möjligheten för en [!DNL Workfront]-administratör att konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) och [Lås eller lås upp ett projekt, en aktivitet eller en utgåva för undergrupper](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Lås upp en projektinställning så att grupper kan konfigurera den

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Project Preferences]** och sedan på **[!UICONTROL Projects]**.

1. Gör något av följande:

   * Om du vill att gruppadministratörer ska kunna konfigurera en inställning för sina grupper låser du upp den ![](assets/unlock-toggle-button.png).
   * Om du vill att alla grupper ska använda din konfiguration för en inställning måste du se till att den är låst (detta är standardinställningen).

     >[!IMPORTANT]
     >
     >Vi rekommenderar att du kommunicerar med administratörer och användare i grupper i hela systemet för att säkerställa att alla behov beaktas när du konfigurerar en låst inställning. När du låser den ärvs konfigurationen för den av alla grupper i systemet. Om inställningen har låsts upp under en viss tid ersätter konfigurationen de som gruppadministratörer kan ha gjort.

1. Klicka på **[!UICONTROL Save]**.
