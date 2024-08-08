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
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '261'
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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om användaren <b>Admin (gruppanvändare)</b> är aktiverad måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p>Mer information om inställningen <b>Användare</b> på en åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Skapa direktrapporter

1. Börja redigera en användare enligt beskrivningen i [Redigera en användarprofil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
1. Kontrollera att ett företag har valts i fältet **Företag** i avsnittet **Organisation**.

   Det här fältet får inte vara tomt.

1. I fältet **Direktrapporter** anger du eventuella användare som rapporterar till den användare som du redigerar.
1. (Valfritt) I fältet **Rapporter till** anger du namnet på den användare som den här användaren rapporterar till.
1. Klicka på **Spara ändringar**.
