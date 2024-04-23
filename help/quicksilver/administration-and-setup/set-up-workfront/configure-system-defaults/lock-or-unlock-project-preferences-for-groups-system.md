---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Låsa eller låsa upp projektinställningar för alla grupper i systemet
description: Grupper i din organisation kan behöva en projektinställning som är annorlunda konfigurerad för sina unika arbetsflöden. Du kan låsa upp inställningen för alla grupper i hela organisationen så att de kan konfigurera den på egen hand.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 3e97df265df83965d094d8723fe76043ff4af80e
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Låsa eller låsa upp projektinställningar för alla grupper i systemet

Grupper i din organisation kan behöva en projektinställning som är annorlunda konfigurerad för sina unika arbetsflöden. Du kan låsa upp inställningen för alla grupper i hela organisationen så att de kan konfigurera den på egen hand.

När en inställning är olåst och gruppadministratören ändrar den, hämtas konfigurationen för den inställningen från gruppnivåinställningen i stället för från systemnivåinställningen för de projekt som är kopplade till gruppen.

## Åtkomstkrav

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Om låsta och olåsta inställningar

Genom att låsa ett projekt, en uppgift eller en utgåva som du har konfigurerat på systemnivå kan du vara säker på att alla använder samma inställning för den inställningen. Även om du fortfarande kan konfigurera om en inställning som du låser kan gruppadministratörer inte konfigurera om den för sina grupper.

Om du låser upp ett projekt, en uppgift eller en utgåva blir gruppadministratörerna mer flexibla när det gäller att hantera hur deras grupper arbetar med objekten. När en inställning är olåst kan gruppadministratörer konfigurera om den för sina grupper.

Om ett fält inte har en lås/lås upp-knapp kan det inte låsas upp för gruppadministratörer för att konfigurera inställningar på gruppnivå. Konfigurationen är bara tillgänglig på systemnivå.

Instruktioner om hur du låser eller låser upp ett projekt, en uppgift eller en utgåva på systemnivå finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Efter [!DNL Workfront] administratören låser upp en inställning på systemnivå. Alla gruppadministratörer kan konfigurera den och sedan låsa den för att säkerställa att alla i gruppen och undergrupperna nedan använder samma konfiguration. Detta är parallellt med möjligheten att [!DNL Workfront] måste administratören konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) och [Låsa eller låsa upp ett projekt, en uppgift eller en utleverans för undergrupper](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Lås upp en projektinställning så att grupper kan konfigurera den

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka **[!UICONTROL Project Preferences]** och sedan klicka **[!UICONTROL Projects]**.

1. Gör något av följande:

   * Om du vill att gruppadministratörer ska kunna konfigurera en inställning för sina grupper låser du upp den ![](assets/unlock-toggle-button.png).
   * Om du vill att alla grupper ska använda din konfiguration för en inställning måste du se till att den är låst (detta är standardinställningen).

     >[!IMPORTANT]
     >
     >Vi rekommenderar att du kommunicerar med administratörer och användare i grupper i hela systemet för att säkerställa att alla behov beaktas när du konfigurerar en låst inställning. När du låser den ärvs konfigurationen för den av alla grupper i systemet. Om inställningen har låsts upp under en viss tid ersätter konfigurationen de som gruppadministratörer kan ha gjort.

1. Klicka på **[!UICONTROL Save]**.
