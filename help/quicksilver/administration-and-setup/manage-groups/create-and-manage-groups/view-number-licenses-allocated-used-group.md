---
title: Visa antalet licenser som tilldelats och används i en grupp
description: Som Adobe Workfront-administratör kan du visa antalet av de enskilda licenstyper som för närvarande används i din grupp och dess undergrupper. Detta är användbart när du behöver utvärdera om du ska distribuera licenser.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Visa antalet licenser som allokerats och använts i en grupp

Som Adobe Workfront-administratör kan du visa antalet av de enskilda licenstyper som för närvarande används i din grupp och dess undergrupper. Detta är användbart när du behöver utvärdera om du ska distribuera licenser.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!IMPORTANT]
>
>En användarlicens räknas i en viss grupp endast om gruppen är användarens hemgrupp.

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
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa antalet licenser som används i en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på gruppens namn.
1. På den sida som visas i sidhuvudet i det övre högra hörnet kan du visa området **Licenser som används** för att se antalet **Planera** och **Arbeta** licenser som används.

   Om du visar en grupp på den översta nivån och Workfront-administratören har definierat ett maximalt antal licenser för gruppen, visas även dessa siffror. I gruppen nedan kan till exempel högst 10 användare ha en planlicens och 15 kan ha en arbetslicens:

   ![Allokerade licenser](assets/licenses-used-allocated.png)

   Mer information om hur en Workfront-administratör definierar ett maximalt antal tilldelade licenser för en grupp finns i avsnittet [Ange maximalt antal licenser för en hemgrupp](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) i artikeln [Hantera tillgängliga licenser i systemet](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Om gruppen du tittar på är en undergrupp kan du bara visa antalet licenser som används, inte det maximala antalet licenser som tilldelas för gruppen. Detta beror på att Workfront-administratörer inte har definierat ett högsta antal licenser för en undergrupp.
   >
   >![Använda licenser i undergrupp](assets/subgroup-used-licenses-only.png)
   >

1. Om du vill ha olika antal av varje typ av licens som används i gruppen (inklusive granskning och begäran) klickar du i textområdet direkt under **Licenser som används:**

   ![Klicka för mer information](assets/click-text-to-see-more.png)

   Den ruta som visas innehåller samma information för alla fyra Workfront-licenstyperna: Plan, Work, Review och Request. Längst ned i rutan visas det totala antalet licenser som används av medlemmar i den här gruppen eller en av dess undergrupper:

   ![Mer licensinformation](assets/more-license-info.png)

   För Granska och Begär licenser visas alltid kolumnen Max. obegränsat.
