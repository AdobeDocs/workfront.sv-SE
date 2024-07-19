---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operationer i Adobe Workfront Fusion
description: En åtgärd i Adobe Workfront Fusion är en uppgift som utförs av en modul. För spårningsändamål är en lyckad åtgärd som utförs av en modul en åtgärd.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Åtgärder i [!DNL Adobe Workfront Fusion]

En åtgärd i [!DNL Adobe Workfront Fusion] är en aktivitet som utförs av en modul. För spårningsändamål är en lyckad åtgärd som utförs av en modul en åtgärd.

## Att tänka på vid inventering av antalet operationer

* I allmänhet betraktas varje lyckad åtgärd som en åtgärd.

* Den första modulen i ett scenario körs bara en gång och räknas alltid som en åtgärd, även om den inte returnerar ett paket.

* Hur många gånger resten av modulerna körs beror på hur många paket de måste behandla.  En serie av en modul för ett paket är en åtgärd. Ett undantag är aggregeringsmodulen, som räknas som en åtgärd per uppsättning paket som bearbetas.

* Åtgärder räknas vid [!UICONTROL Finalization]-steget i en scenariokörning.

* Följande räknas **inte** som åtgärder:

   * Alla filtersteg.

   * Alla åtgärder som innehåller fel eller stopp.

   * Alla vägar som inte körs eftersom ruttens regler inte uppfylls, till exempel återgångsvägar eller inaktiverade rutter.

   * Alla åtgärder som inte körs, antingen på grund av att ett filter inte tillåter data genom eller på grund av att scenariot stoppades på grund av ett fel.

## Operationsbegränsningar

Din organisation kan ha en månatlig driftgräns. Detta baseras på den [!DNL Workfront]-plan som din organisation har köpt. Planen [!UICONTROL Ultimate] [!DNL Workfront] erbjuder ett obegränsat antal åtgärder.

Om din organisation har en månadsgräns meddelas du när du nått gränsen. Om du överskrider gränsen kommer [!DNL Workfront] att kontakta din organisation för att säkerställa att din plan uppfyller dina behov.

## Visa antalet åtgärder som har utförts under de senaste 30 dagarna

Du kan se ett diagram som visar hur många åtgärder som har utförts. Dessa diagram är tillgängliga på följande platser:

* **Organisationens kontrollpanel**: Åtgärder som används av hela organisationen
* **Teaminstrumentpanel**: Åtgärder som används av scenarier som ägs av det här teamet (endast [!DNL Adobe Experience Cloud])
* **Sidan med scenarioinformation**: Åtgärder som används i det här scenariot (endast [!DNL Adobe Experience Cloud])
