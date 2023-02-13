---
title: Bevilja administrativ åtkomst för en layoutmall
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör kan du ge administratörsbehörighet för en layoutmall till gruppadministratörerna för en viss grupp så att de kan redigera mallen. Mallen tilldelas inte användarna i gruppen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Bevilja administrativ åtkomst för en layoutmall

Som Adobe Workfront-administratör kan du ge administratörsbehörighet för en layoutmall till gruppadministratörerna för en viss grupp så att de kan redigera mallen. Mallen tilldelas inte användarna i gruppen.

Mer information om hur du tilldelar användare till en layoutmall finns i [Tilldela användare till en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td><p>Åtkomstnivå för systemadministratören</p><p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Bevilja administrativ åtkomst för en layoutmall

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka **Bevilja åtkomst till** i det övre avsnittet på sidan.
1. Klicka på **Lägg till en grupp**, börja skriva namnet på gruppen, klicka på namnet när det visas och klicka sedan på **Klar**.

   Alla användare som är utsedda som gruppadministratörer för den grupp du anger kan administrera layoutmallen. Mallen är dock inte tilldelad gruppmedlemmen för användning. Mer information om hur du tilldelar en layoutmall till en grupp finns i [Tilldela en layoutmall till användare](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) i den här artikeln.

   >[!NOTE]
   >
   >* När en gruppadministratör skapar en layoutmall är det obligatoriskt att tilldela administratörsåtkomst. Layoutmallen är avsedd för och synlig endast för den angivna gruppen. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Mer information om gruppadministratörer finns i [Gruppadministratörer](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Om du inte ger administratörsbehörighet till gruppadministratörerna i en viss grupp får alla användare som kan redigera användarkonton administratörsbehörighet för layoutmallen. Vissa Workfront-administratörer väljer att inte bevilja administrativ åtkomst för en layoutmall för att göra den till en layoutmall på systemnivå.


1. Du kan klicka på Spara när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.
