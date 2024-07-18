---
title: Ändra beräknade fältformler med AI Assistant
content-type: reference
description: Du kan använda AI Assistant för att lösa fel i ogiltiga anpassade uttryck i beräkningsfält.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Ändra beräknade fältformler med AI Assistant

Du kan använda AI Assistant för att lösa fel i ogiltiga anpassade uttryck i beräkningsfält.

När du skapar beräkningsfältet i det anpassade formulärbyggaren visas ett felmeddelande under fältet om formeln är ogiltig.

![Ogiltigt uttrycksfel](assets/invalid-expression.png)

AI Assistant kan hjälpa dig att ändra formeln till ett giltigt beräknat fältuttryck.

## Ändra ett beräknat fältuttryck

Så här ändrar du ett ogiltigt beräknat fältuttryck:

1. Klicka på ikonen **AI-assistenten** ![AI-assistenten](assets/ai-assistant-icon.png) i skärmens övre högra hörn.
1. Ange ett meddelande i promptområdet längst ned på AI Assistant-panelen, till exempel:
   `Rewrite this formula to remove the invalid expression error`
1. Kopiera det ogiltiga uttrycket från det anpassade formulärverktyget och klistra in det i promptområdet.
1. Tryck på **Retur**.

   AI Assistant kan ta en stund att generera den reviderade formeln, beroende på hur stor eller komplex formeln är.
1. Visa den reviderade formeln på AI-assistentpanelen.
1. (Valfritt) Kopiera den reviderade formeln från AI-assistentpanelen och klistra in den i beräkningsfältet i det anpassade formulärbyggaren.

>[!NOTE]
>
>Vi rekommenderar att du testar beräkningsfältet för att se till att det hämtar det förväntade resultatet.

Mer information om beräkningsfält i Workfront finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
