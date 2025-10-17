---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Översikt över gruppförfrågningar
description: Teamförfrågningar finns i Teams-området på huvudmenyn.
author: Jenny
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Översikt över gruppförfrågningar

## Förstå teamförfrågningar

Teamförfrågningar finns i området [!UICONTROL Teams] i [!UICONTROL Main Menu]. Klicka på ikonen [!UICONTROL Team Requests] ![Request ](assets/request-icon.png) i den vänstra panelen för att visa teamförfrågningar.

>[!NOTE]
>
>Agile-team har inga teamförfrågningar.

Fliken [!UICONTROL Team Requests] visar begäranden som väntar på tilldelning för det team som är markerat i listrutan. Siffran inom parentes anger hur många objekt som ska bearbetas.

En teambegäran representerar en väntande arbetsuppgift som inte är tilldelad en viss användare. Istället tilldelas den till ett team, och alla medlemmar i det teamet kan frivilligt ta ansvar för objektet. Om en användare frivilligt vill arbeta med en teamförfrågan godkänner användaren arbetsuppdraget som sin egen. Uppgiften tilldelas den enskilda användaren utöver teamet.

>[!NOTE]
>
>En teamförfrågan ska inte användas för samverkansbaserade aktivitetstilldelningar. Om du behöver tilldela flera användare för att arbeta tillsammans med en uppgift gör du detta via [!UICONTROL Advanced Assignments] och inte via Team-förfrågningar. Mer information finns i [Skapa avancerade uppdrag](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Förstå alternativen [!UICONTROL Ready to Start] och [!UICONTROL All]

Det finns två alternativ högst upp i gruppförfrågningsavsnittet: [!UICONTROL Ready to Start] och [!UICONTROL All].

Alternativet [!UICONTROL Ready to Start] visar bara aktiviteter och utgåvor som uppfyller alla följande villkor:

* Alla föregångare har uppfyllt villkoren för sina underordnade beroendetyper.\
  Om till exempel typen av föregående relation är [!UICONTROL Finish-Start] (föregående aktivitet måste avslutas innan den beroende aktiviteten kan starta) måste föregående aktivitet markeras som [!UICONTROL Complete]. (Mer information om beroendetyper för föregångare finns i [Översikt över typer av uppgiftsberoenden](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* Den inloggade användaren är den person som är tilldelad dessa uppgifter och utgåvor (för arbetsförfrågningar), eller den valda gruppen är tilldelad dessa uppgifter och utgåvor (för teamförfrågningar).
* Projektstatusen är [!UICONTROL Current].
* [!UICONTROL Projected Start Date] eller [!UICONTROL Planned Start Date] har passerat eller schemalagts att börja inom två veckor från dagens datum (eller så har [!UICONTROL Projected Start Date] eller [!UICONTROL Planned Start Date] inte definierats).
* [!UICONTROL Handoff Date] har redan inträffat eller kommer att inträffa inom två veckor från dagens datum.

>[!NOTE]
>
>Om aktiviteten uppfyller de första tre villkoren och har ett leveransdatum inom två veckor från dagens datum, visas den som [!UICONTROL Ready to Start] även om de planerade/planerade datumen är längre än två veckor. Om aktiviteten inte har något leveransdatum måste planerade/planerade datum ligga inom två veckor från dagens datum.

Alternativet [!UICONTROL All] visar alla uppgifter och ärenden i aktuella projekt som har tilldelats den inloggade användaren eller alla uppgifter eller ärenden som har tilldelats teamet.
