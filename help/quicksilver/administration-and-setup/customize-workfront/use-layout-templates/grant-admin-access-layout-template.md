---
title: Bevilja administratörsåtkomst för en layoutmall
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör kan du ge administratörsbehörighet för en layoutmall till gruppadministratörerna för en viss grupp så att de kan redigera mallen. Mallen tilldelas inte användarna i gruppen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Bevilja administrativ åtkomst för en layoutmall

Som Adobe Workfront-administratör kan du ge administratörsbehörighet för en layoutmall till gruppadministratörerna för en viss grupp så att de kan redigera mallen. Mallen tilldelas inte användarna i gruppen.

Mer information om hur du tilldelar användare till en layoutmall finns i [Tilldela användare till en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.</p>
        <p>Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bevilja administrativ åtkomst för en layoutmall

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på **Bevilja åtkomst till** i det övre avsnittet på sidan.
1. I rutan som visas klickar du på **Lägg till en grupp**, börjar skriva namnet på gruppen, klickar på namnet när det visas och klickar sedan på **Klar**.

   Alla användare som är utsedda som gruppadministratörer för den grupp du anger kan administrera layoutmallen. Mallen är dock inte tilldelad gruppmedlemmen för användning. Mer information om hur du tilldelar en layoutmall till en grupp finns i [Tilldela en layoutmall till användare](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) i den här artikeln.

   >[!NOTE]
   >
   >* När en gruppadministratör skapar en layoutmall är det obligatoriskt att tilldela administratörsåtkomst. Layoutmallen är avsedd för och synlig endast för den angivna gruppen. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Mer information om gruppadministratörer finns i [Gruppadministratörer](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Om du inte ger administratörsbehörighet till gruppadministratörerna i en viss grupp får alla användare som kan redigera användarkonton administratörsbehörighet för layoutmallen. Vissa Workfront-administratörer väljer att inte bevilja administrativ åtkomst för en layoutmall för att göra den till en layoutmall på systemnivå.

1. Du kan klicka på **Spara** när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.
