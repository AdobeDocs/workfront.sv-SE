---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Extern användarlicenstyp saknas från åtkomstnivåer
description: Jag kan inte längre se licenstypen Extern användare under Åtkomstnivåer i Inställningar.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '124'
ht-degree: 0%

---

# Extern användarlicenstyp saknas på åtkomstnivåer

## Problem

Jag kan inte längre se licenstypen Extern användare under Åtkomstnivåer i Inställningar.

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
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösning

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Preferences]**.

1. Kontrollera att alternativet **[!UICONTROL Collaborate with people without Workfront accounts by using their email address]** är aktiverat i avsnittet **[!UICONTROL Security]**.

   Om det här alternativet inte är aktiverat visas inte den externa användaren i inställningarna för åtkomstnivå.
