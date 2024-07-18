---
title: Öppna listan över status för systemprojekt
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Användarna kan ange status för ett projekt så att andra användare kan se projektets aktuella utvecklingsstadium vid en viss tidpunkt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Öppna listan över status för systemprojekt

Användarna kan ange status för ett projekt så att andra användare kan se projektets aktuella utvecklingsstadium vid en viss tidpunkt.

Workfront levereras med nio systemprojektstatusar. Du kan ändra namnet på dessa statusar, men du kan inte ta bort dem.

Du kan också lägga till anpassade projektstatusvärden som passar organisationens behov.

Som Workfront-administratör konfigurerar du standardstatusen för alla nya projekt i systemet. Instruktioner finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Åtkomst till projektstatus

Som Workfront-administratör kan du komma åt listan över projektstatus på systemnivå.

Mer information om hur du redigerar en systemstatus och skapar anpassade statusvärden finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Projektinställningar** > **Status**.

1. Klicka på fliken **Projekt**.

   Projektstatusvärdena i Workfront visas på den här fliken.

   ![](assets/project-status.png)

   Mer information om de inbyggda statusvärdena för systemprojekt finns i [Översikt över status för systemprojekt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Skapa anpassade projektstatusar och anpassa systemstatus

Som Workfront-administratör kan du lägga till systemprojektstatus i Workfront. Som gruppägare kan du lägga till en anpassad status som är specifik för en grupp. Mer information om hur du skapar anpassade statusar eller redigerar systemstatusar finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

När du skapar en anpassad projektstatus måste du alltid jämför den nya statusen med en befintlig systemstatus. Du måste förstå hur systemstatusarna fungerar för att veta vilken status som är lämplig för att motsvara din anpassade status. När du har valt samma status kan du inte ändra det här valet. Mer information om status för systemprojekt finns i [Översikt över status för systemprojekt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
