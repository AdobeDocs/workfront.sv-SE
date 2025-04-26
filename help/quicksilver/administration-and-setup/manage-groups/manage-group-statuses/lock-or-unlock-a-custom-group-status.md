---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Låsta och olåsta gruppstatusar
description: Att låsa en grupps anpassade status är ett sätt att se till att personer i gruppen och dess undergrupper använder samma processer i arbetsflödet. När en gruppstatus är låst är den tillgänglig för alla användare i gruppen och i de nedre grupperna.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Låsta och olåsta gruppstatusar

Att låsa en grupps anpassade status är ett sätt att se till att personer i gruppen och dess undergrupper använder samma processer i arbetsflödet. När en gruppstatus är låst är den tillgänglig för alla användare i gruppen och i de nedre grupperna. Även om du (eller en Workfront-administratör) kan redigera eller ta bort en status som du låser, kan inte administratörer av undergrupper nedan göra det för dessa grupper. De kan bara ändra visningsordningen i statuslistan.

Omvänt kan administratörer av undergrupper som är mindre flexiblare hantera de unika arbetsflöden som används i deras grupper genom att låsa upp en grupps anpassade status. När en gruppstatus är olåst kan administratörer av undergrupper ändra sina attribut eller ta bort den för dessa undergrupper.

>[!IMPORTANT]
>
>Om du låser en anpassad status efter att den har låsts upp under en tidsperiod, ersätter dina statusinställningar dem som gjorts av gruppadministratörer i de nedre undergrupperna. När statusen är låst kan dessa administratörer inte ändra eller ta bort statusen för sina grupper.

Instruktioner om hur du låser eller låser upp en gruppstatus finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Du kan använda både låsta och olåsta lägen i en gruppgodkännandeprocess. Om du skapar en process för gruppgodkännande med olåst gruppstatus kan användarna bifoga godkännandeprocessen till alla projekt, aktiviteter eller utgåvor som är kopplade till gruppen.

