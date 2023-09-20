---
title: Inaktivera alternativet för automatisk uppgradering för obetalda användare i den nya licensplanen
user-type: administrator
content-type: reference
product-area: system-administration
keywords: åtkomst,nivå,system,administratör,standard,ljus,medarbetare
navigation-topic: access-levels
description: Alla användare måste ha en åtkomstnivå för att kunna logga in och arbeta i Workfront. Du använder åtkomstnivån för att styra vad en användare kan se och göra med vissa Workfront-objekt och -områden.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 1ff727f1-bc26-4ffe-a510-615bebfe5b96
source-git-commit: 8807636d2309435cb5f4e08d6a7d27246342200d
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Inaktivera alternativet för automatisk uppgradering för obetalda användare i den nya licensplanen

Handläggningsbeslut och dokumentbeslut är begränsade för alla obetalda Workfront-licenser för nya planer. När användare når sitt tilldelade antal beslut uppgraderas de som standard till en Light-licens.

Du kan inaktivera alternativet för automatisk uppgradering från inställningsområdet. Mer information om hur automatiska uppgraderingar fungerar finns i [Begränsat dokument och bevisbeslut för obetalda användare - översikt](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>När detta är inaktiverat uppgraderas inte obetalda användare som överträffar det angivna antalet beslut automatiskt.


## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Aktuell plan: Standard
   <p>eller</p>
   <p>Gammal plan: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

## Inaktivera automatiska uppgraderingar för obetalda användare

{{step-1-to-setup}}

1. Expandera [!UICONTROL **System**] i den vänstra navigeringen klickar du på [!UICONTROL **Inställningar**].
1. I [!UICONTROL **Allmänna inställningar**] -avsnittet, kontrollera [!UICONTROL **Inaktivera automatisk uppgradering på åtkomstnivåer**] box.
1. Klicka [!UICONTROL **Spara**].
