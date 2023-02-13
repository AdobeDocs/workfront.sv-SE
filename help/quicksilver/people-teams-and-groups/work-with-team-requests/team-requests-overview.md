---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Översikt över gruppförfrågningar
description: Teamförfrågningar finns i Teams-området på huvudmenyn.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Översikt över gruppförfrågningar

## Förstå teamförfrågningar

Teamförfrågningar finns i [!UICONTROL Teams] området i [!UICONTROL Main Menu]. Klicka på [!UICONTROL Team Requests] icon ![Ikon för begäran](assets/request-icon.png) i den vänstra panelen för att visa teamförfrågningar.

>[!NOTE]
>
>Agile-team har inga teamförfrågningar.

The [!UICONTROL Team Requests] På -fliken visas de begäranden som väntar på tilldelning för det team som är markerat i listrutan. Siffran inom parentes anger hur många objekt som ska bearbetas.

En teambegäran representerar en väntande arbetsuppgift som inte är tilldelad en viss användare. Istället tilldelas den till ett team, och alla medlemmar i det teamet kan frivilligt ta ansvar för objektet. Om en användare frivilligt vill arbeta med en teamförfrågan godkänner användaren arbetsuppdraget som sin egen. Uppgiften tilldelas den enskilda användaren utöver teamet.

>[!NOTE]
>
>En teamförfrågan ska inte användas för samverkansbaserade aktivitetstilldelningar. Om du behöver tilldela flera användare för att arbeta tillsammans med en uppgift gör du det här [!UICONTROL Advanced Assignments] och inte via Team-förfrågningar. Mer information finns i [Skapa avancerade uppdrag](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Förstå [!UICONTROL Ready to Start] och [!UICONTROL All] alternativ

Det finns två alternativ högst upp i gruppförfrågningar: [!UICONTROL Ready to Start] och [!UICONTROL All].

The [!UICONTROL Ready to Start] visas endast uppgifter och ärenden som uppfyller följande villkor:

* Alla föregångare har uppfyllt villkoren för sina underordnade beroendetyper.\
   Om till exempel typen av föregående relation är [!UICONTROL Finish-Start] (föregående aktivitet måste slutföras innan den beroende aktiviteten kan startas), måste föregående aktivitet markeras som [!UICONTROL Complete]. (Mer information om beroendetyper för föregångare finns i [Översikt över typer av uppgiftsberoenden](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* Den inloggade användaren är den person som är tilldelad dessa uppgifter och utgåvor (för arbetsförfrågningar), eller så är det valda teamet tilldelat dessa uppgifter och utgåvor (för teamförfrågningar).
* Projektstatusen är [!UICONTROL Current].
* The [!UICONTROL Projected Start Date] eller [!UICONTROL Planned Start Date] har passerat eller är schemalagd att börja inom två veckor från dagens datum (eller inte [!UICONTROL Projected Start Date] eller [!UICONTROL Planned Start Date] har definierats).
* The [!UICONTROL Handoff Date] har redan inträffat eller kommer att inträffa inom två veckor från dagens datum.

>[!NOTE]
>
>Om aktiviteten uppfyller de tre första villkoren och har ett leveransdatum inom två veckor från dagens datum, visas den som [!UICONTROL Ready to Start] även om de planerade/planerade datumen är längre än två veckor. Om aktiviteten inte har något leveransdatum måste planerade/planerade datum ligga inom två veckor från dagens datum.

The [!UICONTROL All] visar alla uppgifter och ärenden i aktuella projekt som tilldelats den inloggade användaren eller alla uppgifter eller ärenden som tilldelats teamet.
