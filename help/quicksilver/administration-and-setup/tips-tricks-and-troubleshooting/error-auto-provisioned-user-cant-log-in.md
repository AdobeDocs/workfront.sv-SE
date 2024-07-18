---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Fel: Automatiskt allokerad användare kan inte logga in"
description: Om en användare med automatisk etablering försöker logga in för första gången och får ett felmeddelande om att systemet inte tilldelar dem en åtkomstnivå, kan det bero på att systemet saknar åtkomstnivåer som är kopplade till begärandelicensen. Automatisk etablering använder licenstypen Begär, så du kan åtgärda problemet genom att skapa en åtkomstnivå som är associerad med en Begär licens.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Fel: Automatiskt allokerad användare kan inte logga in

När en användare med automatisk etablering försöker logga in för första gången visas följande fel:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problem

Systemet tilldelar inte den nya användaren någon åtkomstnivå.

Som standard används licenstypen Begär vid automatisk etablering. När det inte finns några åtkomstnivåer med en begärandelicens kan systemet inte tilldela användaren en åtkomstnivå.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösning

Skapa en grundläggande åtkomstnivå med en begärandelicens:

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Access Levels]**.

1. Klicka på **[!UICONTROL New Access Level]**.
1. Ange **[!UICONTROL Name]**.
1. Välj Begär i listrutan **[!UICONTROL License Type]**.
1. Klicka på **[!UICONTROL Save Changes]**.

När du har skapat en åtkomstnivå med en Request-licens måste användaren logga in med sina SSO-autentiseringsuppgifter.


