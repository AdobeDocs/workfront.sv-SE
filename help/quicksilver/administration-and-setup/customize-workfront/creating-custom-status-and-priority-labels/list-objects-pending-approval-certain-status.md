---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Lista objekt med en väntande godkännandeprocess med en viss status
description: Om du försöker ta bort en status kan ett felmeddelande tala om för dig att den inte kan tas bort eftersom den används i väntande godkännandeprocesser för objekt i systemet. Om du vill hitta och granska objekten för att bestämma vad du behöver göra kan du köra en rapport som listar dem.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Lista objekt med en väntande godkännandeprocess som använder en viss status

Om du försöker ta bort en status kan ett felmeddelande tala om för dig att den inte kan tas bort eftersom den befinner sig i minst en väntande godkännandeprocess i systemet. Du kan köra en rapport för att lista objekten där den befinner sig i en väntande godkännandeprocess och sedan bestämma vad du behöver göra för varje.

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
   <td>
     <p>Nytt: Standard</p>
     <p>eller</p>
     <p>Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p><p>Redigera åtkomst till filter, vyer, grupperingar</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Du får behörigheten Hantera för de rapporter du skapar.</td>
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## I standardläge

{{step1-to-reports}}

1. Klicka på **Ny rapport** och välj sedan **Projektrapport**, **Aktivitetsrapport** eller **Problemrapport**.
1. Öppna fliken **Filter**.
1. Klicka på **Lägg till en filterregel** och gör sedan följande för att konfigurera regeln:
   1. Börja skriva `status` och välj sedan **Status** när den visas.
   1. Låt **vara** i det andra fältet.
   1. Välj statusens namn i det tredje fältet.
1. Klicka på **Lägg till en filterregel** igen och gör sedan följande för att konfigurera regeln
   1. Börja skriva `pending status` och markera sedan objektet när det visas under den objekttyp som du letar efter (**Projekt**, **Aktivitet** eller **Problem**).
   1. Låt **vara** i det andra fältet.
   1. Skriv `in` i det tredje fältet.
1. Klicka på **Lägg till en filterregel** igen och gör sedan följande för att konfigurera regeln
   1. Börja skriva in godkännandeprocessen och välj sedan **Grupp-ID** när det visas under **Godkännandeprocess**.
   1. Välj **Är tom** i det andra fältet.
1. Klicka på **Spara + stäng** om du vill köra rapporten och visa alla objekt av den typ som du har angett med godkännandeprocesser i väntande läge baserat på den status som du har angett (**Projekt**, **Aktivitet** eller **Problem**).
1. Upprepa de här stegen för att hitta samma information för de två andra objekttyperna.


## I textläge

{{step1-to-reports}}

1. Klicka på **Ny rapport** och välj sedan **Projektrapport**, **Aktivitetsrapport** eller **Problemrapport**.
1. Öppna fliken **Filter**.
1. Välj **Växla till textläge**.
1. Kopiera och klistra in följande i redigeringsfönstret och ersätt XXX med 3-bokstavskangenten för statusen:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Du kan visa nyckeln i statuslistan, som visas i följande artiklar:
   * [Öppna listan över status för systemprojekt](project-statuses.md)
   * [Åtkomst till listan över status för systemaktivitet](task-statuses.md)
   * [Åtkomst till listan över status för systemproblem](issue-statuses.md)

1. Klicka på **Spara + stäng** om du vill köra rapporten och visa alla objekt av den typ som du har angett med godkännandeprocesser i väntande läge baserat på den status som du har angett (**Projekt**, **Aktivitet** eller **Problem**).
1. Upprepa de här stegen för att hitta samma information för de två andra objekttyperna.
