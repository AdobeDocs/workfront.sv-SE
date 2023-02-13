---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Lista objekt med väntande godkännandeprocesser som använder en viss status
description: Om du försöker ta bort en status kan ett felmeddelande tala om för dig att den inte kan tas bort eftersom den används i väntande godkännandeprocesser för objekt i systemet. Om du vill hitta och granska objekten för att bestämma vad du behöver göra kan du köra en rapport som listar dem.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Lista objekt med väntande godkännandeprocesser som använder en viss status

Om du försöker ta bort en status kan ett felmeddelande tala om för dig att den inte kan tas bort eftersom den finns i minst en väntande godkännandeprocess i systemet. Du kan köra en rapport för att lista objekten där den befinner sig i en väntande godkännandeprocess och sedan bestämma vad du behöver göra för varje.

## I standardläge

1. Gå till **Rapportering** i det globala navigeringsfältet väljer du **Rapporter** -fliken.
1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Rapporter**.
1. Klicka **Ny rapport** väljer **Projektrapport**, **Uppgiftsrapport**, eller **Problemrapport**.
1. Öppna **Filter** -fliken.
1. Klicka **Lägg till en filterregel** gör du följande för att konfigurera regeln:
   1. Börja skriva `status`väljer **Status** när den visas.
   1. Lämna **Jämn** i det andra fältet.
   1. Välj statusens namn i det tredje fältet.
1. Klicka **Lägg till en filterregel** gör sedan följande för att konfigurera regeln
   1. Börja skriva `pending status`markerar du objektet när det visas under den objekttyp som du tittar på (**Projekt**, **Uppgift**, eller **Problem**).
   1. Lämna **Jämn** i det andra fältet.
   1. Typ `in` i det tredje fältet.
1. Klicka **Lägg till en filterregel** gör sedan följande för att konfigurera regeln
   1. Börja skriva under godkännandeprocessen och välj **Grupp-ID** när den visas under **Godkännandeprocess**.
   1. Välj **Är tom** i det andra fältet.
1. Klicka **Spara + Stäng** för att köra rapporten och lista alla objekt av den typ som du har angett med godkännandeprocesser i väntande tillstånd baserat på den status som du har angett (**Projekt**, **Uppgift**, eller **Problem**).
1. Upprepa de här stegen för att hitta samma information för de två andra objekttyperna.


## I textläge

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Rapporter**.
1. Klicka **Ny rapport** väljer **Projektrapport**, **Uppgiftsrapport**, eller **Problemrapport**.
1. Öppna **Filter** -fliken.
1. Välj **Växla till textläge**.
1. Kopiera och klistra in följande i redigeringsfönstret och ersätt XXX med 3-bokstavskangenten för statusen:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Du kan visa nyckeln i statuslistan, som visas i följande artiklar:
   * [Öppna listan över status för systemprojekt](project-statuses.md)
   * [Åtkomst till listan över status för systemaktivitet](task-statuses.md)
   * [Åtkomst till listan över status för systemproblem](issue-statuses.md)

1. Klicka **Spara + Stäng** för att köra rapporten och lista alla objekt av den typ som du har angett med godkännandeprocesser i väntande tillstånd baserat på den status som du har angett (**Projekt**, **Uppgift**, eller **Problem**).
1. Upprepa de här stegen för att hitta samma information för de två andra objekttyperna.
