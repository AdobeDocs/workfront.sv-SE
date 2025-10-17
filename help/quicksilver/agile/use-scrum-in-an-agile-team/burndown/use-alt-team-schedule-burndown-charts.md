---
product-area: agile-and-teams
navigation-topic: burndown
title: Använd ett alternativt teamschema för nedladdningsscheman
description: Scheman som definieras i  [!DNL Adobe Workfront] påverkar nedladdningsschemat genom att utesluta dagar (helger och helger) från nedladdningen.
author: Jenny
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Använd ett alternativt teamschema för nedladdningsscheman

Scheman som definieras i [!DNL Adobe Workfront] påverkar nedladdningsschemat genom att utesluta dagar (helger och helger) från nedladdningen.

Som standard används standardschemat för nedladdningsschemat. Förutom standardschemat kan team även välja att använda ett alternativt schema för att inkludera teamspecifika, icke-arbetsrelaterade dagar. Det alternativa schemat visas sedan i nedladdningsschemat för alla upprepningar som har tilldelats teamet. Det alternativa schemat påverkar bara nedladdningsschemat. (Mer information om standardschemat och hur administratören av [!DNL Workfront] kan skapa ett teamspecifikt schema finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Nedladdningsschemat tar inte hänsyn till vissa dagar. Om ditt team till exempel arbetar fyra timmar varje fredag visas det som en heldag i nedladdningsschemat.

Mer information om hur du använder nedladdningsschemat finns i översikten över [Agile-nedladdningsschemat](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Arbeta eller högre</p> </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Använd ett alternativt teamschema för nedladdningsscheman

1. Kontrollera att administratören för [!DNL Workfront] redan har skapat det alternativa schemat, vilket beskrivs i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på menyn **[!UICONTROL More]** och välj sedan **[!UICONTROL Edit]**.

1. I avsnittet **[!UICONTROL Agile]** i området **[!UICONTROL Schedule]** väljer du det nya schemat i listrutan.

1. Klicka på **[!UICONTROL Save Changes]**.
