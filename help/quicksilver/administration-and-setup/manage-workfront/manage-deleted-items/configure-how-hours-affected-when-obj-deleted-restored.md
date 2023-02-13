---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Konfigurera påverkan på timmar när ett objekt tas bort och återställs
description: Du kan konfigurera vad som ska hända med timmar när någon tar bort ett projekt, en uppgift eller ett problem som timmarna är inloggade mot. Det alternativ du väljer avgör också vad som händer med timmarna om projektet, aktiviteten eller problemet återställs vid ett senare tillfälle. (Mer information om hur du återställer objekt i Workfront finns i Återställa borttagna objekt.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Konfigurera påverkan på timmar när ett objekt tas bort och återställs

Du kan konfigurera vad som ska hända med timmar när någon tar bort ett projekt, en uppgift eller ett problem som timmarna är inloggade mot. Det alternativ du väljer avgör också vad som händer med timmarna om projektet, aktiviteten eller problemet återställs vid ett senare tillfälle. (Mer information om hur du återställer objekt i Workfront finns i [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera hur timmar hanteras när ett objekt tas bort och återställs

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Expandera **Tidrapporter och timmar** och sedan klicka **Inställningar**.

1. Leta reda på **Inställningar för projekt-, aktivitets- eller problemborttagning** -avsnitt.
1. (Villkorligt) Om du vill konfigurera hur timmar hanteras när ett projekt tas bort väljer du något av följande alternativ i dialogrutan **När projekt tas bort** avsnitt:

   * Behåll loggade timmar som redan lagts till i tidrapporter som allmänna timmar (om projektet återställs senare finns timmarna kvar på tidrapporten)\
      Det här alternativet är markerat som standard.
   * Ta bort alla loggade timmar (om projektet återställs vid ett senare tillfälle återställs loggade timmar till projektet)

1. (Villkorligt) Om du vill konfigurera hur timmar hanteras när en uppgift eller ett problem tas bort väljer du något av följande alternativ i dialogrutan **När uppgifter eller problem tas bort** avsnitt:

   * Flytta alla loggade timmar till det projekt där aktiviteten eller utgåvan finns (om aktiviteten eller utgåvan återställs vid ett senare tillfälle finns timmarna kvar i projektet)\
      Det här alternativet är markerat som standard.
   * Ta bort alla loggade timmar (om aktiviteten eller problemet återställs vid ett senare tillfälle återställs loggade timmar till uppgiften eller problemet)

1. Klicka **Spara**.
