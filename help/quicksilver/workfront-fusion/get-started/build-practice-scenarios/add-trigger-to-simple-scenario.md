---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Lägga till en utlösarmodul i ett grundläggande scenario
description: Lär dig hur du lägger till en utlösarmodul så att scenariot regelbundet kan söka efter nya begäranden och konvertera dem till projekt.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Lägga till en utlösarmodul i ett grundläggande scenario

Utlösarmoduler placeras i början av ett scenario. Dessa moduler startar en scenariokörning när specifika villkor har ändrats i en viss tjänst. Ändringen kan vara att skapa nya poster, ta bort poster, uppdatera poster och så vidare.

Avsökningsmoduler kontrollerar tjänsten vid ett angivet tidsintervall och returnerar information om ändringar som gjorts under det tidsintervallet. Om inga ändringar har gjorts körs inte scenariot av utlösaren.

I det här exemplet lägger du till en utlösarmodul som körs var 15:e minut och startar ett scenario om någon begäran har skickats till en viss kö. Scenariot konverterar sedan dessa begäranden till ett projekt.

I det här exemplet ändras scenariot som skapas i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Förutsättningar

Du måste skapa scenariot enligt [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) innan du följer den här proceduren.

## Lägga till och konfigurera utlösarmodulen

### Lägg till utlösarmodulen

1. Öppna scenariot i scenarioredigeraren.
1. Högerklicka på den första (sökmodulen) och välj **Ta bort modul**.

   Modulen tas bort och en tom platshållare lämnas kvar.

1. Klicka på den tomma modulen och välj **Adobe Workfront** i listan över program.
1. Välj **Bevakningspost**.
1. Se till att modulen använder samma anslutning som resten av modulerna i scenariot.
1. Välj **Endast nya poster**.
1. Välj i rutan Utdata `ID`, `Name`och `Project ID`.
1. Klicka **OK** för att spara modulinställningarna.

   Ett fönster med namnet Välj var du vill starta visas.

1. Välj **Från och med**.

### Schemalägg utlösarmodulen

1. Klicka på klockan i modulen Bevakade poster.

   Fönstret Schemainställningar öppnas.

1. I fältet Kör scenario väljer du **Med regelbundna intervall**.

1. Klicka **OK**.

### Uppdatera den andra modulen

Eftersom den första modulen har ersatts måste den andra modulen mappas till den nya första modulen.

1. Öppna objektmodulen Konvertera.
1. Ta bort det svarta ID-blocket i fältet Problem ID. Blocket är svart eftersom modulen som det mappades från inte längre är tillgänglig.
1. Markera ID-blocket under den första modulen (bevakade poster) för att mappa det till den andra modulen.
1. Klicka **OK**.

### Testa och aktivera

1. Gå till den Workfront-miljö som Fusion ansluter till och lägg till ett problem.
1. Klicka **[!UICONTROL Run once]** i det nedre vänstra hörnet av scenarioredigeraren.
1. Granska utdata för att kontrollera att scenariot kördes som förväntat.
1. När du är säker på att scenariot fungerar som väntat klickar du på **Schemaläggning** växla i det nedre vänstra hörnet av skärmen till **På**.

   Detta aktiverar scenariot.
1. I [!DNL Workfront Fusion], klicka **[!UICONTROL Save]** nära det nedre vänstra hörnet för att spara dina framsteg i scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

## Resurs

* Mer information om webbhooks finns i [Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
