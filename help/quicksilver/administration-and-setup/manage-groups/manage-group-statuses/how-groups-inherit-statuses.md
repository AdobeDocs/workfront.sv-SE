---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Hur grupper ärver statusvärden
description: När du visar en lista med tillgängliga statusvärden för en grupp visas följande
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Hur grupper ärver statusvärden

När du visar en lista med tillgängliga statusvärden för en grupp visas följande

* Anpassade statusvärden som har skapats för gruppen, vilket förklaras i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Status ärvs från systemet och högre i grupphierarkin, vilket förklaras i den här artikeln.

## Ärver status

Gruppen ärver status när något av följande händer:

* Du skapar gruppen.
* En administratör låser en status i en grupp på högre nivå.
* En administratör tar bort en annan grupp och väljer att ersätta gruppen.

Tabellen nedan förklarar de olika omständigheterna.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">När du skapar en grupp</td> 
   <td> <p>När du skapar en ny grupp ärver den automatiskt:</p> 
    <ul> 
     <li>Olåsta statusvärden i gruppen en nivå upp om den nya gruppen är en undergrupp.</li> 
    </ul> 
    <ul> 
     <li>Låsta statusvärden på systemnivå.</li> 
    </ul> 
     <b>EXEMPEL:</b></span></span> 
     <p>Anta att en grupp som heter Marketing har två undergrupper som kallas Marketing Communications och Branding.</p> 
     <p>En gruppadministratör för marknadsföringsgruppen skapar en ny anpassad status som kallas Discovery.</p> 
     <p>Senare skapar du en ny undergrupp under marknadsföringsgruppen och kallar den Advertising.</p> 
     <p>Din undergrupp ärver Discovery-statusen eftersom du skapade gruppen efter att den andra administratören skapade den olåsta Discovery-statusen.</p> 
     <p>Eftersom undergrupperna Marketing Communications and Branding redan fanns under Marketing Group när detta inträffade, ärver de inte den olåsta Discovery-statusen.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">När en administratör låser en status på en högre nivå</td> 
   <td> <p>När en Workfront-administratör låser en status på systemnivå ärver din grupp den tillsammans med alla andra grupper i systemet.</p> <p>När en administratör låser en status för en grupp ovanför gruppen, ärver gruppen den med alla andra undergrupper under den högre gruppen.</p> <p><b>ANMÄRKNING</b>: Om en administratör senare låser upp en av dessa statusar på systemnivå eller i en grupp ovanför gruppen, behåller gruppen den status som den ärvde tidigare. Nu är det en separat version av statusen och du kan anpassa den för just din grupp.</p> 
    <p><b>EXEMPEL:</b></p>
    <p>Administratören för marknadsföringsgruppen låser den identifieringsstatus som nämns ovan för att se till att alla tre undergrupperna har den.</p> 
    <p>Tillsammans med er Advertising Group har grupperna Marketing Communications och Branding statusen Discovery nu. De ärvde det när det var låst i marknadsföringsgruppen ovanför dem.</p> 
    <p>Administratören för marknadsföringsgruppen låser sedan upp Discovery-statusen så att alla tre undergrupperna har sin egen version av Discovery-statusen. Nu kan du och administratörerna för de andra två grupperna anpassa Discovery-statusen efter gruppernas behov.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">När en administratör tar bort en grupp</td> 
   <td> <p>När en administratör tar bort en grupp och väljer din för att ersätta den i systemet, ärver gruppen den borttagna gruppens anpassade status om den inte redan finns i gruppen.</p> 
   <p><b>EXEMPEL: </b></p>
     <p>En grupp med namnet Meddelanden måste sammanfogas med din Advertising-grupp, så en Workfront-administratör tar bort gruppen Meddelanden och väljer att ersätta gruppen.</p> 
     <p>Meddelandegruppen hade en unik status som kallas Pågår. Din Advertising-grupp har nu denna status tillgänglig för användning.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Ärver statuskonfigurationer

När du skapar en grupp på den översta nivån ärver den följande konfigurationer från systemnivån. När du skapar en undergrupp ärver den följande konfigurationer från nästa högre grupp.

* Standardstatuskonfigurationer

   Mer information om dessa finns i [Använd anpassade statusvärden som standardstatusvärden](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Konfigurationer av visningsordning för status

   Mer information om dessa finns i [Ändra ordning på systemnivå och gruppstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Om någon ändrar dessa konfigurationer efter att gruppen har skapats påverkas inte gruppens status.
