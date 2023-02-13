---
title: Dela en portfölj
description: Du kan dela en portfölj med andra användare om du har behörighet att komma åt den.
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: e608cf5bdb0227ea5b8d3109db411e98145aaa38
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Dela en portfölj

Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera portföljer när du tilldelar din åtkomstnivå. Du måste ha en planlicens för att kunna redigera en portfölj. Mer information finns i [Bevilja åtkomst till portföljer](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

Förutom den åtkomstnivå du har beviljats kan du även få behörighet att visa eller hantera specifika portföljer från användare som kan dela dem med dig. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder som användare kan vidta för det objektet.

## Att tänka på när det gäller att dela portföljer

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

* Skaparen av en portfölj har som standard behörigheten Hantera.
* Du kan dela en portfölj individuellt eller dela flera portföljer samtidigt. Att dela en portfölj är detsamma som att dela andra objekt i Workfront. Mer information finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Du kan bara bevilja behörigheterna Visa eller Hantera på Portfolio.

   ![](assets/screen-shot-2014-01-23-at-12.45.15-pm.png)    ![](assets/screen-shot-2014-01-22-at-10.03.43-am-190x167.png)

* När du delar en portfölj ärver användarna som standard samma behörigheter till alla underordnade objekt som är kopplade till portföljen.

   Mer information om objekthierarkin i Workfront finns i [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Du kan ta bort ärvda behörigheter från Portfolio. Mer information om hur du tar bort behörigheter från objekt finns i [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Portfolio behörigheter

I följande tabell visas vilka behörigheter du kan ge användare när de får visa eller hantera en Portfolio:

| **Åtgärder** | **Hantera** | **Visa** |
|---|---|---|
| Redigera information om Portfolio | ✓ |   |
| Visa en Portfolio | ✓ | ✓ |
| Ta bort en Portfolio | ✓ |   |
| Bifoga ett eget formulär | ✓ |   |
| Redigera ett anpassat fält | ✓ |   |
| Lägga till eller ta bort ett program&#42; | ✓ |   |
| Lägga till eller ta bort ett projekt&#42; | ✓ |   |
| Godkänn ett projekt | ✓ |   |
| Portfolio-optimering&#42; | ✓ |   |
| Lägga till en dokumentmapp&#42; | ✓ | ✓ |
| Lägga till ett dokument | ✓ | ✓ |
| Uppdateringar/kommentarer | ✓ | ✓ |
| Dela | ✓ | ✓ |
| Dela hela systemet |   | ✓ |

*Behörigheterna styrs av åtkomstnivån och behörigheterna för andra objekt, som projekt, program och dokument.
