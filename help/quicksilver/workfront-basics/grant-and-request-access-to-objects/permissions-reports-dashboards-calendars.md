---
title: Dela rapporter, kontrollpaneler och kalendrar
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör ger användarna åtkomst att visa eller redigera rapporter, instrumentpaneler och kalendrar när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till rapporter, instrumentpaneler och kalendrar finns i Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar.
author: Alina
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Dela rapporter, kontrollpaneler och kalendrar

Din Adobe Workfront-administratör ger användarna åtkomst att visa eller redigera rapporter, instrumentpaneler och kalendrar när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till rapporter, instrumentpaneler och kalendrar finns i [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller hantera specifika rapporter, instrumentpaneler eller kalendrar som du har åtkomst till Dela. Mer information om hur du tilldelar behörigheter till användare för delning av objekt finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.

Mer information om vad användare på varje åtkomstnivå kan göra med problem finns i avsnittet [Rapporter](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) i artikeln [Tillgängliga funktioner för varje objekttyp](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Att tänka på när du delar en rapport, kontrollpanel eller kalender

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

* Den som har skapat en rapport, kontrollpanel eller kalender har som standard behörigheten Hantera.
* Att dela rapporter, kontrollpaneler och kalendrar påminner om att dela andra objekt i Workfront.

  Mer information om hur du delar objekt i Workfront finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

  Läs även följande artiklar om du vill veta mer om hur du delar rapporter, kontrollpaneler och kalendrar:

   * [Dela en rapport i Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Dela en instrumentpanel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Dela en kalenderrapport](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* Du kan dela rapporter och kontrollpaneler individuellt eller dela dem flera gånger.

  Du kan bara dela kalendrar individuellt. Du kan inte dela dem i grupp.

* Du kan inte dela inbyggda systemrapporter. Du kan bara dela anpassade rapporter.

  Mer information om hur du sparar en systemrapport som en ny anpassad rapport finns i [Skapa en kopia av en rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

* Du kan ge följande behörigheter till rapporter, instrumentpaneler och kalendrar:

   * Visa
   * Hantera

* När du delar en kontrollpanel har användarna behörigheten Visa som standard för alla rapporter, kalendrar och externa sidor på kontrollpanelen.
* Användare med en begärandelicens kan inte visa en systemomfattande rapport. En rapport måste delas med de begärande individuellt om de behöver visa den.
* Om en rapport har en fråga och du delar den offentligt, måste de användare som har åtkomst till rapporten vara inloggade på Workfront för att kunna köra rapporten med hjälp av uppmaningen. Om de inte kan logga in på Workfront ser de rapporten utan uppmaningen.\
  Mer information om begränsningar för delning av rapporter med uppmaningar finns i avsnittet [Begränsningar för delning av promptrapporter](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) i artikeln [Lägga till en uppmaning i en rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Du kan ta bort ärvda behörigheter från en rapport eller kalender.

  Mer information om hur du tar bort ärvda behörigheter från objekt finns i [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

* Du kan även dela en rapport eller en kalender offentligt eller i hela systemet.

  Du kan inte dela en instrumentpanel offentligt, men du kan dela den i hela systemet.

  >[!CAUTION]
  >
  >Vi rekommenderar att du använder försiktighet när du delar objekt som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.
