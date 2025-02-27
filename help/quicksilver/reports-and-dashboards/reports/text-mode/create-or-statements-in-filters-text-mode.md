---
product-area: reporting
navigation-topic: text-mode-reporting
title: Skapa OR-satser i textlägesfilter
description: Du kan inkludera flera satser när du skapar ett filter i listor och rapporter.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Skapa OR-satser i textlägesfilter

Du kan inkludera flera satser när du skapar ett filter i listor och rapporter.

Mer information om hur du skapar filter finns i följande artiklar:

* [Översikt över filter](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Redigera ett filter i textläge](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Filteroperatorer för textläge

Mer information om Adobe Workfront filteroperatorer i standardfiltergränssnittet finns i [Filteröversikt](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront har två filteroperatorer som kopplar ihop varje filterprogramsats:

* **AND**: När du kopplar en filterprogramsats med operatorn AND till två anger du att du vill att båda filterprogramsatserna ska uppfyllas samtidigt.

  Programsatserna i ett filter förenas som standard med operatorn AND.

  När du skapar ett AND-filter i textlägesgränssnittet behöver du inte använda operatorn AND. Det antas.

  **Exempel:** Använd följande textlägeskod om du vill filtrera efter aktiviteter som har dagens planerade slutförandedatum och ett procenttal som är lägre än 100 %:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OR**: När du ansluter 2 filtersatser av operatorn OR anger du att du vill att någon av programsatserna ska uppfyllas.

  >[!TIP]
  >
  >När du ändrar dina AND-programsatser till OR-programsatser bör antalet objekt i rapporten öka.

  När du skapar ett OR-filter med hjälp av textlägesgränssnittet måste du använda operatorn OR.

  **Exempel:** Använd följande textlägeskod om du vill filtrera efter aktiviteter som har ett Planerat slutförandedatum i dag eller ett Procent färdigt som är lägre än 100 %:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## Textlägessyntax för OR-filter

Textlägessyntaxen för ett OR-filter måste innehålla följande:

* Operatorn OR följt av ett kolon, ett tal och ett annat kolon i början av varje filterrad som refererar till objektet i programsatsen OR. Detta inkluderar raden som refererar till filterfältet eller -attributet och raden som refererar till filtermodifieraren.

  Följ det här mönstret när du skapar ett OR-filter:

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >Operatorn OR är skiftlägeskänslig och alltid versaler.

  Du kan ha flera OR-satser i ett filter. I det här fallet får varje OR-programsats ett tal, i den ordning som du vill att programsatserna ska tillämpas.

  **Exempel:** Om du vill filtrera efter aktiviteter som har ett Planerat slutförandedatum som är i dag ELLER ett Procent färdigt som är lägre än 100 % ELLER Status som nytt använder du följande textlägeskod:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* Namnet på fälten eller attributen som du refererar till i ett filter måste skrivas med kamelstil. Mer information om kamelfall finns i [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* När du refererar till anpassade fält i ett OR-filter måste du infoga DE: mellan OR-modifierarsyntaxen och namnet på det anpassade fältet. Du måste stava namnet på det anpassade fältet så som det visas i Workfront-gränssnittet.

  **Exempel:** Om du vill filtrera efter aktiviteter som har statusen Nytt ELLER Procent färdigt lägre än 100 % ELLER ett anpassat fält med namnet Kontotyp och värdet Lika, använder du följande textlägeskod:

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
