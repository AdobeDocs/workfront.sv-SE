---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Gruppadministratörer måste ha högre åtkomst än de som de hanterar
description: Om en gruppadministratör har behörigheter på åtkomstnivån som är lägre än de som de hanterar, kan de inte visa, ändra eller tilldela lägre åtkomstnivåer.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Gruppadministratörer måste ha högre åtkomst än de som de hanterar

Om en gruppadministratör har behörigheter på åtkomstnivån som är lägre än de som de hanterar, kan de inte visa, ändra eller tilldela lägre åtkomstnivåer.

## Problem

Om en gruppadministratör har tilldelats en modifierad planeringsåtkomstnivå med visningsbehörighet för team, men vissa användare har tilldelats en arbetaråtkomstnivå med redigeringsbehörighet för team, kan gruppadministratören inte interagera med den ändrade arbetaråtkomstnivån.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Den här logiken gäller även för den nedrullningsbara menyn Finjustera inställningarna. Båda åtkomstnivåerna kan ha åtkomst till Redigera, men inställningarna i den nedrullningsbara menyn Finjustera inställningarna måste vara högre för gruppadministratören.
> ![](assets/fine-tune-your-settings.png)

## Lösning

Gruppadministratörer måste ha högre behörigheter i alla områden på åtkomstnivån än de som de hanterar.