---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operationer i Adobe Workfront Fusion
description: En åtgärd i Adobe Workfront Fusion är en uppgift som utförs av en modul. För spårningsändamål är en lyckad åtgärd som utförs av en modul en åtgärd.
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Åtgärder i [!DNL Adobe Workfront Fusion]

En åtgärd i [!DNL Adobe Workfront Fusion] är en uppgift som utförs av en modul. För spårningsändamål är en lyckad åtgärd som utförs av en modul en åtgärd.

## Att tänka på vid inventering av antalet operationer

* I allmänhet betraktas varje lyckad åtgärd som en åtgärd.

* Den första modulen i ett scenario körs bara en gång och räknas alltid som en åtgärd, även om den inte returnerar ett paket.

* Hur många gånger resten av modulerna körs beror på hur många paket de måste behandla.  En serie av en modul för ett paket är en åtgärd. Ett undantag är aggregeringsmodulen, som räknas som en åtgärd per uppsättning paket som bearbetas.

* Operationer räknas på [!UICONTROL Finalization] scen för en scenariokörning.

* Följande är **not** räknas som operationer:

   * Alla filtersteg.

   * Alla åtgärder som innehåller fel eller stopp.

   * Alla vägar som inte körs eftersom ruttens regler inte uppfylls, till exempel återgångsvägar eller inaktiverade rutter.

   * Alla åtgärder som inte körs, antingen på grund av att ett filter inte tillåter data genom eller på grund av att scenariot stoppades på grund av ett fel.

## Operationsbegränsningar

Din organisation kan ha en månatlig driftgräns. Detta baseras på [!DNL Workfront] en plan som din organisation har köpt. The [!UICONTROL Ultimate] [!DNL Workfront] plan erbjuder obegränsat antal operationer.

Om din organisation har en månadsgräns meddelas du när du nått gränsen. Om du går över gränsen, [!DNL Workfront] kommer att kontakta din organisation för att säkerställa att din plan uppfyller dina behov.

## Visa antalet åtgärder som har utförts under de senaste 30 dagarna

Du kan se ett diagram som visar hur många åtgärder som har utförts. Dessa diagram är tillgängliga på följande platser:

* **Kontrollpanel för organisation**: Åtgärder som används av hela organisationen
* **Teamkontrollpanel**: Åtgärder som används av scenarier som ägs av det här teamet ([!DNL Adobe Experience Cloud] endast)
* **Sida för scenarioinformation**: Åtgärder som används i detta scenario ([!DNL Adobe Experience Cloud] endast)

