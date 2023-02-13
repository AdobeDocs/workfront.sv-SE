---
product-area: reporting
navigation-topic: text-mode-reporting
title: Skapa OR-satser i textlägesfilter
description: Du kan inkludera flera satser när du skapar ett filter i listor och rapporter.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Skapa OR-satser i textlägesfilter

Du kan inkludera flera satser när du skapar ett filter i listor och rapporter.

Mer information om hur du skapar filter finns i följande artiklar:

* [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Redigera ett filter i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Filteroperatorer för textläge

Mer information om Adobe Workfront filteroperatorer i standardfiltergränssnittet finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront har två filteroperatorer som kopplar ihop varje filterprogramsats:

* **OCH**: När du kopplar en filterprogramsats med operatorn AND anger du att du vill att båda filterprogramsatserna ska uppfyllas samtidigt.

   Programsatserna i ett filter kopplas som standard av operatorn AND.

   När du skapar ett AND-filter i textlägesgränssnittet behöver du inte använda operatorn AND. Det antas.

   **Exempel:** Om du vill filtrera efter uppgifter som har ett planerat slutförandedatum som är idag och ett Procent färdigt som är lägre än 100 % använder du följande textlägeskod:

   <pre>planeradSlutförandedatum=$$TODAY</pre><pre>planningCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **ELLER**: När du kopplar ihop två filtersatser av operatorn OR anger du att du vill att någon av programsatserna ska uppfyllas.

   >[!TIP]
   >
   >När du ändrar dina AND-satser till OR-satser bör antalet objekt i rapporten öka.

   När du skapar ett OR-filter med hjälp av textlägesgränssnittet måste du använda operatorn OR.

   **Exempel:** Om du vill filtrera efter uppgifter som har ett planerat slutförandedatum i dag eller ett Procent färdigt som är lägre än 100 % använder du följande textlägeskod:

   <pre>planeradSlutförandedatum=$$TODAY</pre><pre>planningCompletionDate_Mod=eq</pre><pre>ELLER:1:percentComplete=100</pre><pre>ELLER:1:percentComplete_Mod=lt</pre>

## Textlägessyntax för OR-filter

Textlägessyntaxen för ett OR-filter måste innehålla följande:

* Operatorn OR följt av ett kolon, ett tal och ett annat kolon i början av varje filterrad som refererar till objektet i programsatsen OR. Detta inkluderar raden som refererar till filterfältet eller -attributet och raden som refererar till filtermodifieraren.

   Följ det här mönstret när du skapar ett OR-filter:

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>ELLER:1:<field name in camel case>=<value></pre><pre>ELLER:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >Operatorn OR är skiftlägeskänslig och alltid versaler.

   Du kan ha flera OR-satser i ett filter. I det här fallet får varje OR-programsats ett tal, i den ordning som du vill att programsatserna ska tillämpas.

   **Exempel:**  Om du vill filtrera efter uppgifter som har ett planerat slutförandedatum idag ELLER ett Procent färdigt som är lägre än 100 % ELLER statusvärdet Nytt använder du följande textlägeskod:

   <pre>planeradSlutförandedatum=$$TODAY</pre><pre>planningCompletionDate_Mod=eq</pre><pre>ELLER:1:status=NEW</pre><pre>ELLER:1:status_Mod=in</pre><pre>ELLER:2:percentComplete=100</pre><pre>ELLER:2:percentComplete_Mod=lt</pre>

* Namnet på fälten eller attributen som du refererar till i ett filter måste skrivas med kamelstil. Mer information om kamelcase finns i [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* När du refererar till anpassade fält i ett OR-filter måste du infoga DE: mellan ELLER-modifierarsyntaxen och namnet på det anpassade fältet. Du måste stava namnet på det anpassade fältet så som det visas i Workfront-gränssnittet.

   **Exempel:** Om du vill filtrera efter uppgifter som har statusvärdet Nytt ELLER Procent färdigt lägre än 100 % ELLER ett anpassat fält med namnet Kontotyp med värdet Lika, använder du följande textlägeskod:

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>ELLER:1:percentComplete=100</pre><pre>ELLER:1:percentComplete_Mod=lt</pre><pre>ELLER:2:DE:Kontotyp=Versalt</pre><pre>ELLER:2:DE:Account Type_Mod=in</pre>
