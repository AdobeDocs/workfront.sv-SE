---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Konfigurera effekt på timmar när ett objekt tas bort och återställs
description: Du kan konfigurera vad som ska hända med timmar när någon tar bort ett projekt, en uppgift eller ett problem som timmarna är inloggade mot. Det alternativ du väljer avgör också vad som händer med timmarna om projektet, aktiviteten eller problemet återställs vid ett senare tillfälle. (Mer information om hur du återställer objekt i Workfront finns i Återställa borttagna objekt.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Konfigurera effekt på timmar när ett objekt tas bort och återställs

Du kan konfigurera vad som ska hända med timmar när någon tar bort ett projekt, en uppgift eller ett problem som timmarna är inloggade mot. Det alternativ du väljer avgör också vad som händer med timmarna om projektet, aktiviteten eller problemet återställs vid ett senare tillfälle. (Mer information om hur du återställer objekt i Workfront finns i [Återställa borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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

## Konfigurera hur timmar hanteras när ett objekt tas bort och återställs

{{step-1-to-setup}}

1. Expandera **Tidrapporter och timmar** och klicka sedan på **Inställningar**.

1. Leta reda på avsnittet **Inställningar för projekt, aktivitet eller problemborttagning**.
1. (Villkorligt) Om du vill konfigurera hur timmar hanteras när ett projekt tas bort väljer du något av följande alternativ i avsnittet **När projekt tas bort**:

   * Behåll loggade timmar som redan lagts till i tidrapporter som allmänna timmar (om projektet återställs senare finns timmarna kvar på tidrapporten)\
     Det här alternativet är markerat som standard.
   * Ta bort alla loggade timmar (om projektet återställs vid ett senare tillfälle återställs loggade timmar till projektet)

1. (Villkorligt) Om du vill konfigurera hur timmar hanteras när en uppgift eller ett problem tas bort, väljer du något av följande alternativ i avsnittet **Vid borttagning av aktiviteter eller problem**:

   * Flytta alla loggade timmar till det projekt där aktiviteten eller utgåvan finns (om aktiviteten eller utgåvan återställs vid ett senare tillfälle finns timmarna kvar i projektet)\
     Det här alternativet är markerat som standard.
   * Ta bort alla loggade timmar (om den här uppgiften eller problemet återställs vid ett senare tillfälle återställs loggade timmar till uppgiften eller problemet)

1. Klicka på **Spara**.
