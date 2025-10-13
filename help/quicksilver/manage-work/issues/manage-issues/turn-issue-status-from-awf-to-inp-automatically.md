---
product-area: projects
navigation-topic: manage-issues
title: Uppdatera automatiskt utskicksstatus från Väntar på feedback till Pågår
description: När den primära kontakten för ett problem gör en uppdatering av problemet genom att antingen uppdatera ett fält (inklusive ett anpassat fält) eller lägga till en kommentar, uppdateras ärendets status automatiskt.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Uppdatera automatiskt utskicksstatus från Väntar på feedback till Pågår

<!--Audited: 109/2025-->

När den primära kontakten för ett problem gör en uppdatering av problemet genom att antingen uppdatera ett fält (inklusive ett anpassat fält) eller lägga till en kommentar, uppdateras ärendets status automatiskt.

Följande krävs för att denna automatiska statusändring ska kunna utföras:

* Problemet måste läggas till med en begärandekö.

  Mer information om hur du skapar begärandeköer finns i avsnittet [Skapa och hantera begärandeköer](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md).

  Mer information om hur du skickar begäranden till en frågekö finns i [Skapa och skicka Adobe Workfront-begäranden](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Köinformationen i begärandekön måste ha följande inställningar:
   * **När någon gör en begäran tilldelas** automatiskt **Contribute Access**
   * **Ändra status** har valts

  ![Köinformation ger Contribute åtkomst och Ändra status är valt.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  När du konfigurerar en begärandekö kan du definiera den primära kontaktpersonens åtkomst till de utgåvor de skickar.
  >
  >När du avmarkerar inställningen Ändra status när du ställer in begärandekön måste du komma ihåg att systemadministratörer alltid har tillgång till att ändra status för problem, även om alternativet Ändra status är avmarkerat i inställningarna för begärandekön.

  Mer information om köinformation finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Problemet måste ha statusen Väntar på feedback.
* Det måste finnas en AWF-status (Väntar på feedback) för problem på systemnivå.

  Mer information om statusvärden på systemnivå finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
