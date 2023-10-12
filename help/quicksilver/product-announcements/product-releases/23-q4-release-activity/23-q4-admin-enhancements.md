---
title: Förbättringar av administratören för fjärde kvartalet 2023
description: Förbättringar av administratören för fjärde kvartalet 2023
author: Lisa
feature: Product Announcements
source-git-commit: 8488cb46b3dd9b377c59121597db5b6fe784fdab
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Förbättringar av administratören för fjärde kvartalet 2023

Den här sidan beskriver alla administratörsförbättringar som gjorts i den fjärde utgåvan av kvartal 2023 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön med version 23.10.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den fjärde utgåvan av kvartal 2023 finns på [Versionsöversikt för fjärde kvartalet 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Beräknade fält i anpassade formulär kan nu använda jokertecknet $$USER

The `$$USER` jokertecken är nu tillgängliga i beräknade anpassade fält och externa sökfält i den nya formulärdesignern. Referens `$$USER` i en beräkning läggs den aktuella användarens ID till. Du kan också använda jokertecknet med ett annat fält. Till exempel: `$$USER.{name}` lägger till den aktuella användarens namn.

Mer information om beräkningsfält finns i [Lägg till beräknade fält med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Lägg till värdealternativ från ett externt API till ett anpassat formulär

En ny fälttyp, **Extern sökning** finns nu på den anpassade formulärdesignern. När du har data lagrade på ett externt system kan du med den här fälttypen läsa in alternativ från ett externt API och filtrera baserat på andra fältvärden i det anpassade formuläret.

När formuläret läggs till i ett objekt visas de värden som returneras från API:t i ett listrutefält och användaren kan välja ett.

>[!NOTE]
>
>Den nya **Extern sökning** fälttypen är inte tillgänglig i det äldre formulärverktyget.

Mer information finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
