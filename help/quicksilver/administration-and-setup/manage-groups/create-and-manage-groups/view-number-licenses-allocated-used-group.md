---
title: Visa antalet licenser som allokerats och använts i en grupp
description: Som Adobe Workfront-administratör kan du visa antalet av de enskilda licenstyper som för närvarande används i din grupp och dess undergrupper. Detta är användbart när du behöver utvärdera om du ska distribuera licenser.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Visa antalet licenser som allokerats och använts i en grupp

Som Adobe Workfront-administratör kan du visa antalet av de enskilda licenstyper som för närvarande används i din grupp och dess undergrupper. Detta är användbart när du behöver utvärdera om du ska distribuera licenser.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!IMPORTANT]
>
>En användarlicens räknas i en viss grupp endast om gruppen är användarens hemgrupp.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront</a>*</td> 
   <td> <p>Team eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront-licens</a>*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Visa antalet licenser som används i en grupp

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** ![](assets/groups-icon.png).

1. Klicka på gruppens namn.
1. På den sida som visas i sidhuvudsområdet i det övre högra hörnet visas **Licenser som används** område för att se antalet **Plan** och **Arbete** licenser som används för närvarande.

   Om du visar en grupp på den översta nivån och Workfront-administratören har definierat ett maximalt antal licenser för gruppen, visas även dessa siffror. I gruppen nedan kan till exempel högst 10 användare ha en planlicens och 15 kan ha en arbetslicens:

   ![](assets/licenses-used-allocated.png)

   Mer information om hur en Workfront-administratör definierar ett maximalt antal tilldelade licenser för en grupp finns i avsnittet [Ange högsta antal licenser för en hemgrupp](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) i artikeln [Hantera tillgängliga licenser i ditt system](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Om gruppen du tittar på är en undergrupp kan du bara visa antalet licenser som används, inte det maximala antalet licenser som tilldelas för gruppen. Detta beror på att Workfront-administratörer inte har definierat ett högsta antal licenser för en undergrupp.
   >
   >![](assets/subgroup-used-licenses-only.png)

1. Om du vill ha olika antal av varje licenstyp som används i gruppen (inklusive Granska och Begär) klickar du i textområdet direkt nedan **Licenser som används:**

   ![](assets/click-text-to-see-more.png)

   Den ruta som visas innehåller samma information för alla fyra licenstyperna i Workfront: Planera, arbeta, granska och begär. Längst ned i rutan visas det totala antalet licenser som används av medlemmar i den här gruppen eller en av dess undergrupper:

   ![](assets/more-license-info.png)

   För Granska och Begär licenser visas alltid kolumnen Max. obegränsat.
