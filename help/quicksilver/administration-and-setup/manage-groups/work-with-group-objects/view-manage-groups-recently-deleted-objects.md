---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visa och hantera nyligen borttagna objekt i en grupp
description: När du visar en grupp som du hanterar i området Grupper kan du visa, filtrera, återställa och exportera de nyligen borttagna arbetsobjekten, dokumenten och mallarna.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Visa och hantera nyligen borttagna objekt i en grupp

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med nyligen borttagna projekt, uppgifter, utgåvor, dokument och mallar på följande sätt:

* Visa, filtrera och gruppera en lista över nyligen borttagna objekt
* Återställ nyligen borttagna objekt som du väljer
* Exportera en lista med nyligen borttagna objekt

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Mer information om borttagna objekt finns i [Hantera borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>De borttagna objekten måste vara kopplade till gruppen eller någon av dess undergrupper. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

+++

## Visa och hantera nyligen borttagna objekt i en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på gruppens namn.
1. Klicka på **Nyligen borttagen** i den vänstra panelen.
1. Öppna någon av följande flikar där du vill visa och hantera gruppens nyligen borttagna objekt:

   * Projekt
   * Uppgifter
   * Problem
   * Dokument
   * Mallar

   På varje flik visas objekt av motsvarande objekttyp som tillhör den aktuella gruppen eller dess undergrupper och som har tagits bort under de senaste 30 dagarna.

   >[!NOTE]
   >
   >Om någon tog bort ett projekt togs alla dess enskilda uppgifter, utgåvor och dokument bort tillsammans med projektet. De visas inte individuellt på flikarna Åtgärder, Problem, Dokument eller Mallar. Om du återställer projektet återställs även alla dessa underordnade objekt till projektet.
   >
   >
   >Om någon har tagit bort en uppgift, ett ärende, ett dokument eller en mall individuellt kan du visa och hantera den på lämplig flik.

1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Återställ objekt</p> </td> 
      <td> <p>Markera upp till 10 objekt och klicka sedan på <strong>Återställ</strong>.</p> </td> 
     </tr> 
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
