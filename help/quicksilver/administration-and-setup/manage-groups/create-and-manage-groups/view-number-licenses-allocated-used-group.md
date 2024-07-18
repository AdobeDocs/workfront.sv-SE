---
title: Visa antalet licenser som allokerats och använts i en grupp
description: Som Adobe Workfront-administratör kan du visa antalet av de enskilda licenstyper som för närvarande används i din grupp och dess undergrupper. Detta är användbart när du behöver utvärdera om du ska distribuera licenser.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: 0e8f8973ad4c1310b973bae4e6fe3578c05db204
workflow-type: tm+mt
source-wordcount: '486'
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
   <td role="rowheader">Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Visa antalet licenser som används i en grupp

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på gruppens namn.
1. På den sida som visas i sidhuvudet i det övre högra hörnet kan du visa området **Licenser som används** för att se antalet **Planera** och **Arbeta** licenser som används.

   Om du visar en grupp på den översta nivån och Workfront-administratören har definierat ett maximalt antal licenser för gruppen, visas även dessa siffror. I gruppen nedan kan till exempel högst 10 användare ha en planlicens och 15 kan ha en arbetslicens:

   ![](assets/licenses-used-allocated.png)

   Mer information om hur en Workfront-administratör definierar ett maximalt antal tilldelade licenser för en grupp finns i avsnittet [Ange maximalt antal licenser för en hemgrupp](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) i artikeln [Hantera tillgängliga licenser i systemet](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Om gruppen du tittar på är en undergrupp kan du bara visa antalet licenser som används, inte det maximala antalet licenser som tilldelas för gruppen. Detta beror på att Workfront-administratörer inte har definierat ett högsta antal licenser för en undergrupp.
   >
   >![](assets/subgroup-used-licenses-only.png)
   >

1. Om du vill ha olika antal av varje typ av licens som används i gruppen (inklusive granskning och begäran) klickar du i textområdet direkt under **Licenser som används:**

   ![](assets/click-text-to-see-more.png)

   Den ruta som visas innehåller samma information för alla fyra Workfront-licenstyperna: Plan, Work, Review och Request. Längst ned i rutan visas det totala antalet licenser som används av medlemmar i den här gruppen eller en av dess undergrupper:

   ![](assets/more-license-info.png)

   För Granska och Begär licenser visas alltid kolumnen Max. obegränsat.
