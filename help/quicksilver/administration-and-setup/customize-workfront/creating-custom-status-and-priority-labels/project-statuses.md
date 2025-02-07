---
title: Få åtkomst till listan över systemprojektstatus
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Användarna kan ange status för ett projekt så att andra användare kan se projektets aktuella utvecklingsstadium vid en viss tidpunkt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Öppna listan över status för systemprojekt

Användarna kan ange status för ett projekt så att andra användare kan se projektets aktuella utvecklingsstadium vid en viss tidpunkt.

Workfront levereras med nio systemprojektstatusar. Du kan ändra namnet på dessa statusar, men du kan inte ta bort dem.

Du kan också lägga till anpassade projektstatusvärden som passar organisationens behov.

Som Workfront-administratör konfigurerar du standardstatusen för alla nya projekt i systemet. Instruktioner finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Åtkomst till projektstatus

Som Workfront-administratör kan du komma åt listan över projektstatus på systemnivå.

Mer information om hur du redigerar en systemstatus och skapar anpassade statusvärden finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Status**.

1. Klicka på fliken **Projekt**.

   Projektstatusvärdena i Workfront visas på den här fliken.

   ![Projektstatus](assets/project-status.png)

   Mer information om de inbyggda statusvärdena för systemprojekt finns i [Översikt över status för systemprojekt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Skapa anpassade projektstatusar och anpassa systemstatus

Som Workfront-administratör kan du lägga till systemprojektstatus i Workfront. Som gruppägare kan du lägga till en anpassad status som är specifik för en grupp. Mer information om hur du skapar anpassade statusar eller redigerar systemstatusar finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

När du skapar en anpassad projektstatus måste du alltid jämför den nya statusen med en befintlig systemstatus. Du måste förstå hur systemstatusarna fungerar för att veta vilken status som är lämplig för att motsvara din anpassade status. När du har valt samma status kan du inte ändra det här valet. Mer information om status för systemprojekt finns i [Översikt över status för systemprojekt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
