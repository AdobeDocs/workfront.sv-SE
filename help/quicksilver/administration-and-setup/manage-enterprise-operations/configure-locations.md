---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Konfigurera platser
description: Du kan konfigurera de standardplatser som är tillgängliga att tilldela som attribut till jobbroller i tariffkort.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Konfigurera platser

Du kan konfigurera de standardplatser som är tillgängliga att tilldela som attribut till jobbroller i tariffkort. Detta garanterar att priskorten korrekt återspeglar marknadsräntorna på varje plats.

Graderingskort gör att din organisation enkelt kan hantera faktureringstaxor för projekt. Mer information finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till en plats

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Platser**] i den vänstra panelen.
1. Klicka på [!UICONTROL **Lägg till fler platser**] längst ned i listan.
1. Ange platsnamn och beskrivning.
1. Klicka utanför inmatningsområdet för att spara platsen.
1. Om du vill ta bort en plats markerar du den i listan och klickar på ikonen **Ta bort** ![Ta bort](assets/delete.png) .

>[!NOTE]
>
>Platser som är associerade med jobbroller på ett tariffkort kan inte tas bort.

## Lägg till en underplats

Du kan lägga till en underplats till en befintlig plats. Om du till exempel redan har en plats i Storbritannien kan London vara en underplats.

Tre nivåer av underplatser är tillåtna. Land, delstat och stad är vanliga användningsområden för underplatser.

Varje underplats kan läggas till som ett attribut på ett tariffkort på samma sätt som en plats på den översta nivån, för att definiera hastigheten för en specifik jobbroll på den platsen.

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Platser**] i den vänstra panelen.
1. Välj en befintlig plats i listan och klicka på **Lägg till underplats**.
1. Ange platsnamn och beskrivning.
1. Klicka utanför inmatningsområdet för att spara platsen.

   Underplatsen är indragen under den översta platsen.

   ![Platser och underplatser](assets/locations-sublocations.png)


