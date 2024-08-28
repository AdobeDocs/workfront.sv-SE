---
title: Ändra beräknade fältformler med AI Assistant
content-type: reference
description: Du kan använda AI Assistant för att lösa fel i ogiltiga anpassade uttryck i beräkningsfält.
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 09c05db7c6a5db7db74dd95ca323415f4318489d
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Generera eller ändra beräknade fältformler med AI Assistant

Du kan använda AI Assistant för att generera formler baserat på en uppmaning som du anger. Du kan också lösa fel i ogiltiga anpassade uttryck i beräkningsfält.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Prime eller Ultimate</p>
       <p>eller</p>
       <p>Aktuell: Inte tillgänglig</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Inte tillgänglig</p></td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Generera ett beräknat fältuttryck

## Ändra ett beräknat fältuttryck

När du skapar beräkningsfältet i det anpassade formulärbyggaren visas ett felmeddelande under fältet om formeln är ogiltig.

![Ogiltigt uttrycksfel](assets/invalid-expression.png)

AI Assistant kan hjälpa dig att ändra formeln till ett giltigt beräknat fältuttryck.

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

