---
title: Översikt över Adobe Workfront-licenser
user-type: administrator
content-type: reference
product-area: system-administration
keywords: licens,typ
navigation-topic: access-levels
description: Organisationen köpte ett visst antal licenser när den förvärvade Adobe Workfront. Som Workfront-administratör ger du en av fyra typer av betalda Workfront-licenser till varje användare när du tilldelar användaren en åtkomstnivå.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f30e2d8-f5c3-4811-b780-49a2b0d058e7
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Översikt över Adobe Workfront-licenser

Organisationen köpte ett visst antal licenser när den förvärvade Adobe Workfront. Som Workfront-administratör ger du en av fyra typer av betalda Workfront-licenser till varje användare när du tilldelar användaren en åtkomstnivå.

## Hur Workfront licenser och åtkomstnivåer knyts ihop

De fyra typerna av betalda Workfront-licenser ger olika åtkomstnivåer till Workfront. Varje åtkomstnivå är kopplad till en av dessa licenser.

Som Workfront-administratör tilldelar du en användare den åtkomstnivå som är kopplad till licensen i stället för att tilldela en licens till en användare.

Tabellen och diagrammet visar de viktigaste åtkomstnivåerna till Workfront:

| Licens | Associerad åtkomstnivå |
|--- |--- |
| Plan | Systemadministratör, planerare |
| Arbete | Arbetare |
| Granska | Granskare |
| Extern* | Extern användare |

>[!NOTE]
>
>Extern licens är inte en betald licens. Den är främst avsedd för dokumentutbyte med medarbetare som inte använder Workfront. Mer information finns i [Inbyggda åtkomstnivåer i Adobe Workfront](default-access-levels-in-workfront.md).

![](assets/licenses-and-access-levels.png)

## Så här definierar en licens en åtkomstnivå

Licensen som är kopplad till en åtkomstnivå avgör det totala antalet funktioner som är tillgängliga på åtkomstnivån.

Du kan kopiera en standardåtkomstnivå och anpassa kopian efter dina användares behov. Inom ramen för de funktioner som tillåts av licensen för den kopierade åtkomstnivån kan du justera åtkomstinställningarna så att de passar användarens behov.

Mer information finns i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) och [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Antal licenser

När du tilldelar en åtkomstnivå till en användare minskas antalet tillgängliga licenser med 1.

Om du till exempel tilldelar en användare åtkomstnivån Planering, minskas antalet tillgängliga Planera-licenser med 1.

Du kan visa licenser och åtkomstnivåer som tilldelats dina användare. Mer information finns i [Visa användarnas åtkomstnivåer och licenser](../../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md).

Mer information om hur du hanterar licenser finns i [Hantera tillgängliga licenser i ditt system](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
