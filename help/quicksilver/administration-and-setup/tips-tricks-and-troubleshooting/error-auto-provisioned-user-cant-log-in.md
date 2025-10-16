---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fel: Användare som etablerats automatiskt kan inte logga in'
description: Om en användare med automatisk etablering försöker logga in för första gången och får ett felmeddelande om att systemet inte tilldelar dem en åtkomstnivå, kan det bero på att systemet saknar åtkomstnivåer som är kopplade till begärandelicensen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%

---

# Fel: Automatiskt allokerad användare kan inte logga in

När en användare med automatisk etablering försöker logga in för första gången visas följande fel:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problem

Systemet tilldelar inte den nya användaren någon åtkomstnivå.

Som standard används licenstypen Begär vid automatisk etablering. När det inte finns några åtkomstnivåer med en begärandelicens kan systemet inte tilldela användaren en åtkomstnivå.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösning

Skapa en grundläggande åtkomstnivå med en begärandelicens:

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Access Levels]**.

1. Klicka på **[!UICONTROL New Access Level]**.
1. Ange **[!UICONTROL Name]**.
1. Välj Begär i listrutan **[!UICONTROL License Type]**.
1. Klicka på **[!UICONTROL Save Changes]**.

När du har skapat en åtkomstnivå med en Request-licens måste användaren logga in med sina SSO-autentiseringsuppgifter.


