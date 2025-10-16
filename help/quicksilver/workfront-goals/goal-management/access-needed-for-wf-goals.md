---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Krav för att använda Workfront-mål
description: Adobe Workfront-administratören måste se till att vissa villkor uppfylls innan du kan komma åt Adobe Workfront mål. Läs den här artikeln om åtkomstkraven, behörigheterna och layoutkraven för att få tillgång till Workfront-målen.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: dacfd8ef7475b197ac6ce5dd598c99df97037479
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Krav för att använda Workfront-mål

<!--Audited P&P only: 04/2025-->

Adobe Workfront-administratören måste se till att alla följande villkor uppfylls innan du kan komma åt Adobe Workfront mål:

* Din organisation har tidigare köpt ett Adobe Workfront Goals-paket. Adobe Workfront-mål går inte längre att köpa.

  Mer information finns i avsnittet [Få åtkomst till Workfront-målorganisation](#obtain-workfront-goals-organization-access) i den här artikeln.

* Tilldela dig rätt typ av Workfront-licens. Mer information om tilldelning av licenstyper och åtkomstnivåer finns i avsnittet [Uppdatera licenstyper och inställningar för åtkomstnivå](#update-license-types-and-access-level-settings) i den här artikeln.

  >[!NOTE]
  >
  >Användare med en extern licenstyp har inte åtkomst till Workfront-mål.

* Ge åtkomst till mål på din åtkomstnivå. Mer information finns i [Bevilja åtkomst till Adobe Workfront-mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

  >[!NOTE]
  >
  >Som standard får användarna ingen åtkomst till mål på åtkomstnivån.


* Tilldela dig en layoutmall som innehåller området Mål på huvudmenyn.

  >[!NOTE]
  >
  >Alla användare, inklusive systemadministratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn.

  Mer information finns i avsnittet [Lägg till Workfront-mål i en layoutmall](#add-workfront-goals-to-a-layout-template) i den här artikeln.

* Om du måste ändra mål som du inte skapat själv måste målskaparen dela målen med dig och ge dig behörigheten Hantera.

  Mer information finns i avsnittet [Dela enskilda mål med andra användare](#share-individual-goals-with-other-users) i den här artikeln.

## Få åtkomst till Workfront Goals Organization {#obtain-workfront-goals-organization-access}

Det senaste Adobe Workfront-paketet som innehöll Workfront Goals var Adobe Workfront Ultimate.
Workfront-mål kan inte längre köpas för nyare paket.
Tala med din kontorepresentant om du vill veta mer om Workfront mål.

<!--Old: >
Depending on which Workfront plan your company is currently on, the following scenarios exist: 

* **A new Workfront plan**: You must have an Ultimate Workfront plan. Workfront Goals are included only in this plan. 

* **A current Workfront plan**: Your organization must purchase an additional license, in addition to the Workfront license.

  After your organization purchases the additional license, Workfront enables Workfront Goals for your account. For information about purchasing a license for Workfront Goals contact your Workfront account manager.

For information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Uppdatera licenstyper och inställningar för åtkomstnivå  {#update-license-types-and-access-level-settings}

Om ditt företag har åtkomst till Workfront-mål från ett tidigare köp måste din Workfront-administratör ge dig följande behörighet för Workfront-mål:

1. En av följande licenser:

   * Medarbetare eller högre
   * Begäran eller senare

<!--Old: 
* **The new access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

  * Contributor
  * Light
  * Standard

* **The current access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals:

  * Plan
  * Work 
  * Review
  * Request
-->

1. Följande åtkomstnivå:

   * Visa eller öka åtkomsten till mål på din åtkomstnivå.

   Mer information om åtkomst till mål finns i [Bevilja åtkomst till Adobe Workfront-mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Som Workfront-administratör kan du granska antalet licenser för Workfront Goals i ditt system och se hur många som är aktiverade för tillfället. Mer information finns i [Hantera tillgängliga licenser i systemet](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Med Workfront kan du tilldela fler licenser för Workfront Goals som du har köpt. Om du tilldelar fler licenser än vad som tillåts enligt Workfront Goals-avtalet kontaktar en Workfront-kontoansvarig dig för att tala om att du har överskridit ditt avtalsnummer.

## Lägg till Workfront-mål i en layoutmall {#add-workfront-goals-to-a-layout-template}

Din Workfront- eller gruppadministratör måste tilldela dig en layoutmall som innehåller området Mål på huvudmenyn så att du kan komma åt Workfront mål.

![Layoutmall](assets/layout-template-align-highlighted-350x220.png)

Din Workfront-administratör eller gruppadministratör kan även lägga till följande i din layoutmall så att du enkelt kan komma åt Workfront-mål:

* En fäst flik
* Gör målområdet till din landningssida

Mer information om hur du uppdaterar layoutmallen finns i följande artiklar:

* [Skapa och hantera layoutmallar](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Anpassa huvudmenyn med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Anpassa fästa sidor med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Anpassa landningssidan med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Tilldela användare till en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Dela individuella mål med andra användare {#share-individual-goals-with-other-users}

Som standard kan alla användare som har minst Visa åtkomst till mål på åtkomstnivå visa alla mål i Workfront.

Alla användare som har Redigera-åtkomst till mål kan skapa mål och får automatiskt Manage-åtkomst till de mål de skapar. Om de måste redigera andra användares mål måste någon med behörigheten Hantera för dessa mål dela de mål som de inte skapade med dem.

Mer information om att dela mål med användare och ge dem behörigheterna Hantera finns i [Dela ett mål i Workfront-mål](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
