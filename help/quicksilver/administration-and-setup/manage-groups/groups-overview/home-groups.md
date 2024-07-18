---
title: Översikt över hemgrupper
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: En hemgrupp tilldelas i användarens profil. Alla användare måste ha en hemgrupp. En användare kan tillhöra mer än en grupp, men kan bara ha en hemgrupp. Även om alla befintliga grupper i systemet kan tilldelas som en användares hemgrupp rekommenderar vi att du skapar och tilldelar nya grupper som representerar större organisationsenheter. När du skapar hemgrupper bör du tänka på hur din organisation delar upp dina Adobe Workfront-användare.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Översikt över hemgrupper

En hemgrupp tilldelas i användarens profil. Alla användare måste ha en hemgrupp. En användare kan tillhöra mer än en grupp, men kan bara ha en hemgrupp. Mer information om grupper finns i [Gruppöversikt](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Även om alla befintliga grupper i systemet kan tilldelas som en användares hemgrupp rekommenderar vi att du skapar och tilldelar nya grupper som representerar större organisationsenheter.

När du skapar hemgrupper bör du tänka på hur din organisation delar upp dina Adobe Workfront-användare. Här följer några förslag som avgör vilken typ av grupper som ska användas som hemgrupp:

* Grupper som representerar avdelningar som IT eller marknadsföring
* Grupper som styrs av olika budgetar
* Grupper som finns i olika områden eller regioner
* Grupper som består av flera team som tillhör samma kostnadsställe

>[!NOTE]
>
>Om du behöver ordna om dina hemgrupper i organisationsenheter måste du >
>1. Skapa den nya gruppen enligt beskrivningen i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Tilldela om den nya gruppen som användarens hemgrupp enligt beskrivningen i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>

## Hantering av layoutmallar

När du tilldelar en layoutmall till en grupp kan alla användare som har gruppen tilldelad som sin hemgrupp se de inställningar som anges i layoutmallen.

Om en layoutmall har tilldelats en hemgrupp är den bara synlig för användare som har tilldelats den hemgruppen.

Mer information finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Licenshantering

Varje användare kan bara tilldelas till en hemgrupp, vilket gör det enklare att hantera antalet licenser.

Workfront-administratörer kan ange högsta antal licenser för hemgrupperna.

Genom att ange ett högsta antal licenser kan Workfront-administratörer förhindra att en affärsenhet använder Workfront-licenser som köpts för andra affärsenheter.

Mer information finns i [Hantera tillgängliga licenser i systemet](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
