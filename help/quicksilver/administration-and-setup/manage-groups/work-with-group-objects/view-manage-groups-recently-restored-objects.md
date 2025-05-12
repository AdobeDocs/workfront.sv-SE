---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visa och hantera nyligen återställda objekt i en grupp
description: När du visar en grupp som du hanterar i området Grupper kan du visa, dela, gruppera och återställa dess nyligen återställda arbetsobjekt, dokument och mallar.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8ec06363-080e-4f1d-8a50-fc14f06ad323
source-git-commit: 96b9939131beebd9c1968cb5c287d75295c68c5b
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Visa och hantera nyligen återställda objekt i en grupp

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med nyligen återställda projekt, uppgifter, utgåvor, dokument och mallar på följande sätt:

* Visa, filtrera och gruppera en lista över nyligen återställda objekt
* Exportera en lista över nyligen återställda objekt

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Mer information om återställda objekt finns i [Återställa borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

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
   <td role="rowheader">Adobe Workfront-licens</td>
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr>
  <tr> 
   <td role="rowheader">Objektbehörigheter</td>
   <td>De återställda objekten måste vara kopplade till gruppen eller någon av dess undergrupper.</td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa och hantera nyligen återställda objekt i en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på gruppens namn.
1. Klicka på **Senast återställd** i den vänstra panelen.
1. Öppna någon av följande flikar där du vill visa och hantera gruppens nyligen återställda objekt:

   * Projekt
   * Uppgifter
   * Problem
   * Dokument
   * Mallar

   På varje flik visas objekt av motsvarande objekttyp som tillhör den aktuella gruppen eller dess undergrupper och som har återställts under de senaste 30 dagarna.

1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Exportera hela listan med objekt på fliken</p> </td> 
      <td> <p>Klicka på <strong>Exportera</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Ändra visningen av information i listan</p> </td> 
      <td> <p>Använd <strong>Filter</strong> i det övre högra hörnet ovanför listan för att definiera vad som ska visas baserat på villkor som du anger. Använd <strong>Visa</strong> för att definiera vilka fält som ska visas som kolumner. Använd <strong>Gruppering</strong> för att gruppera objekten i kategorier.</p> </td> 
     </tr> 
    </tbody> 
   </table>
