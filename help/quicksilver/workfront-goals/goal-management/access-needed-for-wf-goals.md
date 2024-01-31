---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Krav för att använda Workfront-mål
description: Adobe Workfront-administratören måste se till att vissa villkor uppfylls innan du kan komma åt Adobe Workfront mål.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Krav för att använda Workfront-mål

Adobe Workfront-administratören måste se till att alla följande villkor uppfylls innan du kan komma åt Adobe Workfront mål:

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* Din organisation måste köpa rätt licens för Workfront Goals. Mer information finns i avsnittet [Få åtkomst till Workfront Goals Organization](#obtain-workfront-goals-organization-access)i den här artikeln.

* Tilldela dig rätt typ av Workfront-licens. Mer information om tilldelning av licenstyper och åtkomstnivåer finns i avsnittet [Uppdatera licenstyper och inställningar för åtkomstnivå](#update-license-types-and-access-level-settings) i den här artikeln.

>[!NOTE]
>
>Användare med en extern licenstyp har inte åtkomst till Workfront-mål.

* Ge åtkomst till mål på din åtkomstnivå. Mer information finns i [Ge åtkomst till Adobe Workfront mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* Tilldela dig en layoutmall som innehåller området Mål på huvudmenyn.

  >[!NOTE]
  >
  >Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn.

  Mer information finns i avsnittet [Lägg till Workfront-mål i en layoutmall](#add-workfront-goals-to-a-layout-template) i den här artikeln.

* Om du måste ändra mål som du inte skapat själv måste målskaparen dela målen med dig och ge dig behörigheten Hantera.

  Mer information finns i avsnittet [Dela individuella mål med andra användare](#share-individual-goals-with-other-users) i den här artikeln.

## Få åtkomst till Workfront Goals Organization {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

Din organisation måste köpa ytterligare en licens, utöver Workfront-licensen, för att dina användare ska kunna komma åt Workfront mål. När organisationen har köpt den extra licensen aktiverar Workfront Workfront Goals för ditt konto. Kontakta din kontoansvarige på Workfront om du vill ha information om hur du köper en licens för Workfront Goals.

## Uppdatera licenstyper och inställningar för åtkomstnivå  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

Din Workfront-administratör måste ge dig en av följande Workfront-licenstyper för att få tillgång till Workfront mål:

* Plan
* Arbete
* Granska
* Begäran

När din Workfront-administratör har gett dig en av dessa licenstyper måste du även få åtkomst till mål på din åtkomstnivå. Mer information om åtkomst till mål finns i [Ge åtkomst till Adobe Workfront mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Som Workfront-administratör kan du granska antalet licenser för Workfront Goals i ditt system och se hur många som är aktiverade för tillfället. Mer information finns i [Hantera tillgängliga licenser i ditt system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Med Workfront kan du tilldela fler licenser för Workfront Goals som du har köpt. Om du tilldelar fler licenser än vad som tillåts enligt Workfront Goals-avtalet kontaktar en Workfront-kontoansvarig dig för att tala om att du har överskridit ditt avtalsnummer.

## Lägg till Workfront-mål i en layoutmall {#add-workfront-goals-to-a-layout-template}

Din Workfront- eller gruppadministratör måste tilldela dig en layoutmall som innehåller området Mål på huvudmenyn så att du kan komma åt Workfront mål.

![](assets/layout-template-align-highlighted-350x220.png)

Din Workfront-administratör eller gruppadministratör kan även lägga till följande i din layoutmall så att du enkelt kan komma åt Workfront-mål:

* En fäst flik
* Gör målområdet till din landningssida

Mer information om hur du uppdaterar layoutmallen finns i följande artiklar:

* [Skapa och hantera layoutmallar](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Anpassa huvudmenyn med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Anpassa fästa sidor med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Anpassa landningssidan med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Tilldela användare till en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Dela individuella mål med andra användare {#share-individual-goals-with-other-users}

Som standard kan alla användare som har minst Visa åtkomst till mål på åtkomstnivå visa alla mål i Workfront.

Alla användare som har Redigera-åtkomst till mål kan skapa mål och får automatiskt Manage-åtkomst till de mål de skapar. Om de måste redigera andra användares mål måste någon med behörigheten Hantera för dessa mål dela de mål som de inte skapade med dem.

Mer information om att dela mål med användare och ge dem behörigheten Hantera finns i [Dela ett mål i Workfront-mål](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
