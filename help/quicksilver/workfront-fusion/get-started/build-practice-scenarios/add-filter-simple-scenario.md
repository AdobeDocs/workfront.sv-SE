---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Lägga till ett filter i ett grundscenario
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: b43355ed-9329-4080-8e61-7177eb580994
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Lägg till ett filter i ett grundläggande scenario i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Lägg till ett filter i ett grundscenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-filter-basic-scenario.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Med filter kan du kontrollera att ditt scenario bara utvecklas om vissa villkor uppfylls.

I det här exemplet lägger du till ett filter i ditt scenario som tillåter att ett nytt projekt skapas från en begäran endast om begäran skickades till en viss begärandekö.

I det här exemplet ändras scenariot som skapades i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront utlösarmoduler innehåller filter som tillåter att ett scenario startar endast om vissa villkor uppfylls. Men eftersom filter mellan moduler används för alla icke-utlösande och icke-Workfront-användningsfall är det viktigt att du lär dig hur du använder filter mellan moduler. I det här exemplet används ett mellanmodulsfilter för funktioner som kan uppfyllas med ett in-modul-filter.

## Förutsättningar

Du måste skapa scenariot som beskrivs i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) innan du följer den här proceduren.

## Lägga till ett filter

### Förbered för att lägga till filtret

1. Öppna det första scenariot.
1. Välj `Project` i området **Utdata**.
Du bör nu ha `ID`, `Name` och `Project` markerat.
1. Klicka på OK för att spara modulinställningarna.
1. Öppna Workfront.
1. I Workfront letar du reda på det projekt som representerar begärandekön som Fusion-scenariot ska användas med.

   Det här projektet måste finnas på samma Workfront-konto som Fusion-anslutningen är konfigurerad för.

1. Anteckna projekt-ID:t i URL:en.

   Exempel: https://\&lt;MyDomain\>.my.workfront.com/project/\&lt;ProjectID\>/tasks

### Lägg till och konfigurera filtret

1. Öppna scenariot i scenarioredigeraren.
1. Klicka på skiftnyckelsikonen ![skiftningsikonen](assets/wrench-icon.png) mellan den första och den andra modulen och välj **Konfigurera ett filter**.
1. I fältet Etikett anger du en etikett för det här filtret, till exempel &quot;Filter för begärandekö&quot;.
1. Mappa `projectID` från den första modulen i det övre fältet i området **Villkor**.

   ![Mappa projekt-ID](assets/map-proj-id.png)
1. Låt operatorn **Villkor** vara lika med.
1. Klistra in det projekt-ID som du antecknade från projekt-URL:en i [Förbered för att lägga till filtret](#prepare-to-add-the-filter) i det nedre fältet i området **Villkor**.
1. Klicka på **OK** om du vill spara filterinställningarna.

### Testa och aktivera

1. Gå till den Workfront-miljö som Fusion ansluter till och lägg till ett fel i projektet som du angav i filtret. Lägg till ytterligare ett problem i ett annat projekt.
1. Klicka på **[!UICONTROL Run once]** i det nedre vänstra hörnet i scenarioredigeraren.
1. Granska utdata för att kontrollera att scenariot kördes som förväntat.

   Båda problemen bör förekomma i resultatet av det första scenariot, men endast problemet i det angivna projektet ska visas som indata i det andra scenariot.
1. När du är säker på att scenariot fungerar som förväntat klickar du på växeln **Schemaläggning** längst ned till vänster på skärmen till **På**.

   Detta aktiverar scenariot.
1. I [!DNL Workfront Fusion] klickar du på **[!UICONTROL Save]** i det nedre vänstra hörnet för att spara förloppet för scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

## Resurs

* Mer information om filter finns i [Lägga till ett filter i ett scenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
