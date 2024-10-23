---
title: Förbättringar av administratören för fjärde kvartalet 2023
description: Förbättringar av administratören för fjärde kvartalet 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Förbättringar av administratören för fjärde kvartalet 2023

Den här sidan beskriver alla administratörsförbättringar som gjorts i den fjärde utgåvan av kvartal 2023 i förhandsvisningsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön med version 23.10.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den fjärde utgåvan av kvartal 2023 finns i [Översikt över utgåvan fjärde kvartalet 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Bevis- och dokumentbeslut som är tillgängliga för kunder med äldre licensmodell

Gamla kunder som ännu inte gått över till den nya licensmodellen för Adobe Workfront kan nu se data med antalet beslut om bevis/dokument per användare och månad i en enda rapport. Dessa data är tillgängliga när du kör en rapport om användarbeslut.

Mer information finns i [Förstå objekt i Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) och [Visa antalet korrektur- och dokumentbeslut för alla användare](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Beräknade fält i anpassade formulär kan nu använda jokertecknet $$USER

Jokertecknet `$$USER` är nu tillgängligt i beräknade anpassade fält och externa sökfält på den nya formulärdesignern. Om `$$USER` refereras i en beräkning läggs den aktuella användarens ID till. Du kan också använda jokertecknet med ett annat fält. `$$USER.{name}` skulle till exempel lägga till den aktuella användarens namn.

Mer information om beräkningsfält finns i [Lägga till beräknade fält med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Lägg till värdealternativ från ett externt API till ett anpassat formulär

En ny fälttyp, **Extern sökning**, är nu tillgänglig för den anpassade formulärdesignern. När du har data lagrade på ett externt system kan du med den här fälttypen läsa in alternativ från ett externt API och filtrera baserat på andra fältvärden i det anpassade formuläret.

När formuläret läggs till i ett objekt visas de värden som returneras från API:t i ett listrutefält och användaren kan välja ett.

>[!NOTE]
>
>Den nya fälttypen **Extern sökning** är inte tillgänglig i den äldre formulärbyggaren.

Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
