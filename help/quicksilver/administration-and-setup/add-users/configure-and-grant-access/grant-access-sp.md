---
title: Bevilja åtkomst till scenarioplan
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till scenarioplanen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# Bevilja åtkomst till scenarioplan

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till Scenarioplanering, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Förutom tillgång till Scenarioplanering måste en användare med en åtkomstnivå som inte är systemadministratör också ha tillgång till ekonomiska data för att kunna se all finansiell information i en plan, t.ex. budgetar, kostnader och jobbrollstariffer. Mer information finns i [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Företag eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre. Mer information finns i <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Översikt över äldre licenser</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för Adobe Workfront Scenario Planner för att få tillgång till de funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du skaffar Workfront Scenario Planner finns i <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Åtkomst krävs för att använda scenarioplaneraren</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa åtkomst eller senare till scenarioplanen</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektbehörigheter</p> </td> 
   <td> <p>Visa behörigheter eller högre för en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Begär åtkomst till en plan i scenarioplanen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konfigurera användaråtkomst till scenarioplanen med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på alternativet till höger om **Scenarioplan** som du vill använda för den här åtkomstnivån.

   >[!NOTE]
   >
   >Licenstypen Begäran eller Extern licens tillåter inte Visa eller Redigera åtkomst till Scenarioplanering.

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med någon av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

## Åtkomst till scenarioplan per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med scenarioplanen finns i avsnittet [Område för scenarioplanering](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Åtkomst till scenarioplan via inställning för åtkomstnivå

Följande information kan hjälpa dig att förstå hur du använder åtkomstnivåinställningarna för att styra användarnas åtkomst till information i Workfront Scenarioplan.

* [Ingen åtkomst](#no-access)
* [Visa åtkomst](#view-access)
* [Redigera åtkomst](#edit-access)

### Ingen åtkomst {#no-access}

En användare som inte har tillgång till Scenarioplanering kan varken se ikonen Scenarier på huvudmenyn när den läggs till i layoutmallen eller visa planer och initiativ som delas med dem. Om länken till en plan delas med en användare som inte har tillgång till Scenarioplanering kan användaren inte visa eller redigera planen.

### Visa åtkomst {#view-access}

Användare med åtkomst till Scenarioplanering kan göra följande:

* Se ikonen Scenarier på huvudmenyn ![](assets/esp-icon-in-main-menu.png)men området Planer är tomt såvida inte användaren klickar på en planlänk som delas av en annan användare.
* Visa en plan när en annan användare delar länken till den.

   Detta inkluderar all jobbrollinformation i planen.

   Det innehåller även jobbrollfrekvenser och kostnadsinformation om planen om mottagaranvändaren också har tillgång till ekonomiska data. Mer information finns i [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Redigera åtkomst {#edit-access}

Användare med Redigera-åtkomst till Scenarioplanering kan göra följande:

* Se ikonen Scenarier på huvudmenyn ![](assets/esp-icon-in-main-menu.png) och använda det för att få tillgång till plandata.
* Skapa planer.
* Visa, redigera och ta bort planer som de skapar.
* Visa, redigera och ta bort andra användares planer som de använder via en delad länk.

   Detta inkluderar all jobbrollsinformation i en plan.

   Det innehåller även jobbrollfrekvenser och kostnadsinformation om planen om mottagaranvändaren har tillgång till ekonomiska data. Mer information finns i [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
