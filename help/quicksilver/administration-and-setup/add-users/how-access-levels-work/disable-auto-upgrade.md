---
title: Inaktivera alternativet för automatisk uppgradering för icke-betalda användare i den nya licensplanen
user-type: administrator
content-type: reference
product-area: system-administration
keywords: åtkomst,nivå,system,administratör,standard,ljus,medarbetare
navigation-topic: access-levels
description: Alla användare måste ha en åtkomstnivå för att kunna logga in och arbeta i Workfront. Du använder åtkomstnivån för att styra vad en användare kan se och göra med vissa Workfront-objekt och -områden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Inaktivera alternativet för automatisk uppgradering för obetalda användare i den nya licensplanen

Handläggningsbeslut och dokumentbeslut är begränsade för alla obetalda Workfront-licenser för nya planer. När användare når sitt tilldelade antal beslut uppgraderas de som standard till en Light-licens.

Du kan inaktivera alternativet för automatisk uppgradering från inställningsområdet. Mer information om hur automatiska uppgraderingar fungerar finns i [Begränsat dokument och korrekturbeslut för användare som inte är betalande - översikt](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>När detta är inaktiverat uppgraderas inte obetalda användare som överträffar det angivna antalet beslut automatiskt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td>Ny plan: Standard
   <p>eller</p>
   <p>Aktuell plan: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Inaktivera automatiska uppgraderingar för obetalda användare

{{step-1-to-setup}}

1. Expandera [!UICONTROL **System**] i den vänstra navigeringen och klicka sedan på [!UICONTROL **Inställningar**].
1. I avsnittet [!UICONTROL **Allmänna inställningar**] markerar du kryssrutan [!UICONTROL **Inaktivera automatisk uppgradering i åtkomstnivåer**].
1. Klicka på [!UICONTROL **Spara**].
