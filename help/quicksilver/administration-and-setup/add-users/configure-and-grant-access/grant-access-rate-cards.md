---
title: Bevilja åtkomst till finansiella data
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du definiera en användares åtkomst till ekonomiska data i Workfront via åtkomstnivån.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---


# Bevilja åtkomst till tariffkort

{{highlighted-preview-article-level}}

Som Adobe Workfront-administratör kan du definiera en användares åtkomst till tariffkort via användarens åtkomstnivå, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Mer information om tariffkort finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när det gäller att bevilja åtkomst till tariffkort

Tänk på följande när du beviljar användare åtkomst till betalkort i Workfront:

* Användarna måste ha Redigera-åtkomst till Rate Cards, Projects och Financial Data för att kunna koppla ett kurskort till ett projekt.
* Användare som saknar åtkomst till tariffkort och redigeringsåtkomst till ekonomiska data kan inte bifoga ett tariffkort till ett projekt, men de kan redigera andra faktureringstariffer för det projekt som kommer från andra källor.

## Konfigurera användaråtkomst för att klassificera kort med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på knappen **Visa** eller **Redigera** till höger om Klassificeringskort och välj sedan de funktioner som du vill ge under **Finjustera dina inställningar**.

   ![Finjustera åtkomst till betalkort](assets/rate-card-access-fine-tune.png)

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Åtkomst till kort med delad hastighet

Du kan dela ett tariffkort med andra användare genom att ge dem behörighet enligt beskrivningen i [Dela ett tariffkort](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md).

När du delar ett objekt med en annan användare bestäms mottagarens rättigheter till det av en kombination av två saker:

* De behörigheter som du ger mottagaren för objektet
* Mottagarens åtkomstnivåinställningar för objektets typ
