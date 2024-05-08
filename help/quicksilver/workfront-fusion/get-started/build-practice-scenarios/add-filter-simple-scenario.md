---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Lägga till ett filter i ett grundscenario
description: Med filter kan du kontrollera att ditt scenario bara utvecklas om vissa villkor uppfylls.
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Lägg till ett filter i ett grundscenario i [!DNL Adobe Workfront Fusion]

Med filter kan du kontrollera att ditt scenario bara utvecklas om vissa villkor uppfylls.

I det här exemplet lägger du till ett filter i ditt scenario som tillåter att ett nytt projekt skapas från en begäran endast om begäran skickades till en viss begärandekö.

I det här exemplet ändras scenariot som skapas i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront utlösarmoduler innehåller filter som tillåter att ett scenario startar endast om vissa villkor uppfylls. Men eftersom filter mellan moduler används för alla icke-utlösande och icke-Workfront-användningsfall är det viktigt att du lär dig hur du använder filter mellan moduler. I det här exemplet används ett mellanmodulsfilter för funktioner som kan uppfyllas med ett in-modul-filter.

## Förutsättningar

Du måste skapa scenariot enligt [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) innan du följer den här proceduren.

## Lägga till ett filter

### Förbered för att lägga till filtret

1. Öppna det första scenariot.
1. I **Utdata** område, markera `Project`.
Du borde ha `ID`, `Name`och `Project` markerat.
1. Klicka på OK för att spara modulinställningarna.
1. Öppna Workfront.
1. I Workfront letar du reda på det projekt som representerar begärandekön som Fusion-scenariot ska användas med.

   Det här projektet måste finnas på samma Workfront-konto som Fusion-anslutningen är konfigurerad för.

1. Anteckna projekt-ID:t i URL:en.

   Exempel: https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### Lägg till och konfigurera filtret

1. Öppna scenariot i scenarioredigeraren.
1. Klicka på skiftnyckelsikonen ![Ikon för skiftnyckel](assets/wrench-icon.png) mellan den första och den andra modulen och välj **Konfigurera ett filter**.
1. I fältet Etikett anger du en etikett för det här filtret, till exempel &quot;Filter för begärandekö&quot;.
1. I **Villkor** i det övre fältet, mappa `projectID` från den första modulen.

   ![Mappa projekt-ID](assets/map-proj-id.png)
1. Lämna **Villkor** -operatorn lika med.
1. I det nedre fältet på **Villkor** -området, klistra in det projekt-ID som du antecknade från projektets URL i [Förbered för att lägga till filtret](#prepare-to-add-the-filter).
1. Klicka **OK** för att spara filterinställningarna.

### Testa och aktivera

1. Gå till den Workfront-miljö som Fusion ansluter till och lägg till ett fel i projektet som du angav i filtret. Lägg till ytterligare ett problem i ett annat projekt.
1. Klicka **[!UICONTROL Run once]** i det nedre vänstra hörnet av scenarioredigeraren.
1. Granska utdata för att kontrollera att scenariot kördes som förväntat.

   Båda problemen bör förekomma i resultatet av det första scenariot, men endast problemet i det angivna projektet ska visas som indata i det andra scenariot.
1. När du är säker på att scenariot fungerar som väntat klickar du på **Schemaläggning** växla i det nedre vänstra hörnet av skärmen till **På**.

   Detta aktiverar scenariot.
1. I [!DNL Workfront Fusion], klicka **[!UICONTROL Save]** nära det nedre vänstra hörnet för att spara dina framsteg i scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

## Resurs

* Mer information om filter finns i [Lägga till ett filter i ett scenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

