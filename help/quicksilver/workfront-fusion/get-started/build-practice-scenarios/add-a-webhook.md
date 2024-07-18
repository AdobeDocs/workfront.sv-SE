---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Lägga till en webkrok i ett grundläggande scenario
description: Webhooks, som också kallas direktutlösare, är en specifik typ av utlösarmodul som kan starta ett scenario när en ändring görs, i stället för enligt ett visst schema.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Lägg till en webkrok i ett grundläggande scenario i [!DNL Adobe Workfront Fusion]

Webhooks, som också kallas direktutlösare, är en specifik typ av utlösarmodul som kan starta ett scenario när en ändring görs, i stället för enligt ett visst schema.

I det här exemplet lägger du till en webkrok för att starta ett scenario så snart en begäran har skickats till en viss kö. Scenariot konverterar sedan dessa begäranden till ett projekt.

I det här exemplet ändras scenariot som skapades i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Förutsättningar

Du måste skapa scenariot som beskrivs i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) innan du följer den här proceduren.

## Lägg till och konfigurera webkroken

1. Öppna objektmodulen Konvertera.
1. Ta bort det svarta ID-blocket i fältet Problem ID. Blocket är svart eftersom modulen som det mappades från inte längre är tillgänglig.
1. Markera ID-blocket under den första modulen (bevakade händelser) för att mappa det till den andra modulen.
1. Klicka på **OK**.

### Lägg till webbkrokmodulen

1. Öppna scenariot i scenarioredigeraren.
1. Högerklicka på den första modulen och välj **Ta bort modul**.

   Modulen tas bort och en tom platshållare lämnas kvar.

1. Klicka på den tomma modulen och välj **Adobe Workfront** i listan med program.
1. Välj **Bevakade händelser**.
1. Klicka på **Lägg till** bredvid Webkrok-fältet.
1. i fältet Posttyp väljer du **Utgåva** så att modulen utlöser ändringar i utgåvor.
1. Välj **Nytt läge** i fältet Läge. Det här är ett obligatoriskt fält som används för filtret, som det här exemplet inte omfattar.
1. Välj **Endast ny post** i fältet Postens ursprung. Detta gör att scenariot kan utlösas när en utgåva läggs till, inte när någon uppdateras eller tas bort.
1. Klicka på **Spara** för att spara modulkonfigurationen.
