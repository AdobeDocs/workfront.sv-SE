---
title: Skapa direktrapporter
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Du kan ange användare som direkta rapporter till en annan användare. På så sätt kan du skapa ett organisationsschema som visar organisationens hanteringsstruktur.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dea77522-d89f-4baa-a701-aea124d2b3a5
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Skapa direktrapporter

Du kan ange användare som direkta rapporter till en annan användare. På så sätt kan du skapa ett organisationsschema som visar organisationens hanteringsstruktur. Mer information finns i [Visa organisationsschemat](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: Standard</p><p>eller</p><p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa direktrapporter

1. Börja redigera en användare enligt beskrivningen i [Redigera en användarprofil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
1. Kontrollera att ett företag har valts i fältet **Företag** i avsnittet **Organisation**.

   Det här fältet får inte vara tomt.

1. I fältet **Direktrapporter** anger du eventuella användare som rapporterar till den användare som du redigerar.
1. (Valfritt) I fältet **Rapporter till** anger du namnet på den användare som den här användaren rapporterar till.
1. Klicka på **Spara ändringar**.
