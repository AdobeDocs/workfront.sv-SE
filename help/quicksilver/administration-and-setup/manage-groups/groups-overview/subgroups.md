---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Översikt över undergrupper
description: Du kan skapa upp till 14 nivåer med undergrupper under en grupp. På någon av dessa nivåer kan du skapa ett obegränsat antal parallella undergrupper.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Översikt över undergrupper

Du kan skapa upp till 14 nivåer med undergrupper under en grupp. På någon av dessa nivåer kan du skapa ett obegränsat antal parallella undergrupper. Instruktioner finns i [Skapa en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Mer information om grupper finns i [Översikt över grupper](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Vad ärver undergrupper?

Undergrupper ärver medlemskapet i sin överordnade grupp. Därför har användare och grupper i en undergrupp samma synlighet, behörigheter och åtkomst till alla objekt som användare och grupper som tillhör den överordnade grupp som de delar.

Dessutom ärver en undergrupp automatiskt gruppadministratörerna för sin grupp på den översta nivån, men du kan även tilldela medlemmar i en undergrupp att fungera som gruppadministratörer.

>[!TIP]
>
>Ibland kanske du vill använda undergrupper för att lägga till flera användare i en befintlig grupp för att ge dem åtkomst till ett objekt de behöver.
>
>Anta till exempel att du har en grupp helpdesk-tekniker och en separat grupp IT-chefer. Supportgruppen har behörighet till en viss frågekö. Du vill lägga till IT-cheferna i helpdesk-gruppen så att de också har behörighet till Request Queue. Utan undergruppsfunktionerna skulle du behöva lägga till IT-cheferna i helpdesk-gruppen manuellt, vilket kan vara ineffektivt och svårt att hantera. Om du lägger till IT-chefsgruppen i helpdesk-gruppen som en undergrupp kan du utföra den här uppgiften snabbare med bara en ändring.

>[!NOTE]
>
>Om en användare har lagts till i både en undergrupp och i den överordnade gruppen separat, tas inte användaren bort från den andra när användaren tas bort. Om du inte vill att användaren ska ha åtkomst till den överordnade gruppen måste du ta bort användaren både från undergruppen och från den överordnade gruppen.

## Offentliga och privata undergrupper

För en offentlig grupp kan alla användare (i eller utanför gruppen) som har behörighet att redigera användare lägga till gruppen i profilen för andra användare. De kan inte göra detta för en privat grupp.

Du kan bara redigera det här alternativet på den översta överordnade gruppen i en grupphierarki som har mer än en nivå. Alla undergrupper i den överordnade gruppen ärver inställningen.

Om du skapar en undergrupp under en grupp som är offentlig, är undergruppen också offentlig som standard. Mer information om hur du skapar en grupp och gör den offentlig finns i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Mer information om den åtkomst som krävs för att redigera användare finns i [Bevilja åtkomst till användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Alla grupper som du lägger till i en befintlig grupp blir automatiskt en undergrupp och är inte längre en huvudgrupp. Undergruppen behåller dock sina befintliga användare, liksom eventuella associationer med projekt, utgåvor och uppgifter, utöver alla projekt-, uppgifts- och utgivningsstatusar som tillhör den nya överordnade gruppen.

## Gruppadministratörer för undergrupper

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Du kan tilldela undergruppsmedlemmar som gruppadministratörer till undergruppen när du skapar eller redigerar den. Instruktioner finns i [&#128279;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) i artikeln [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Alternativt kan du lämna administreringen av undergruppen till de gruppadministratörer som är tilldelade till grupperna ovan. När du skapar en undergrupp får gruppadministratörer över grupperna ovan automatisk åtkomst för att hantera undergruppen.

>[!NOTE]
>
>Om du lägger till en användare i en undergrupp och den användaren är gruppadministratör för en grupp var som helst ovanför undergruppen, har den användaren administratörsbehörighet för att hantera undergruppen, även om användaren inte har tilldelats en gruppadministratör för den.

Mer information om vilka åtgärder som är tillgängliga för en Adobe Workfront-administratör som hanterar Workfront-systemet, en gruppadministratör som hanterar en högnivågrupp och en gruppadministratör som hanterar en undergrupp finns i [Åtgärder som är tillåtna för olika typer av administratörer](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
