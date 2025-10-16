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
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 1%

---

# Extern användarlicenstyp saknas på åtkomstnivåer

## Problem

Jag kan inte längre se licenstypen Extern användare under Åtkomstnivåer i Inställningar.

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

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Preferences]**.

1. Kontrollera att alternativet **[!UICONTROL Security]** är aktiverat i avsnittet **[!UICONTROL Collaborate with people without Workfront accounts by using their email address]**.

   Om det här alternativet inte är aktiverat visas inte den externa användaren i inställningarna för åtkomstnivå.
