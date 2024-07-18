---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Lägga till en utlösarmodul i ett grundläggande scenario
description: Lär dig hur du lägger till en utlösarmodul så att scenariot regelbundet kan söka efter nya begäranden och konvertera dem till projekt.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Använd en funktion för att uppdatera ett projekt i ett enkelt scenario i [!DNL Adobe Workfront Fusion]

Att uppdatera en arbetsuppgift från Workfront är ett vanligt användningsområde för Workfront Fusion. I det här exemplet använder du en funktion för att ändra namnet på ett projekt till versaler.

Fusion innehåller många typer av funktioner som gör att du kan omvandla och utföra villkorsstyrd logik på dina data. Mer information om hur du använder funktioner finns i [Mappa information från en modul till en annan i Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

I det här exemplet ändras scenariot som skapades i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Förutsättningar

Du måste skapa scenariot som beskrivs i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) innan du följer den här proceduren.

## Uppdatera ett projekt med en funktion

### Lägg till modulen Uppdatera post i ditt scenario

1. Öppna scenariot i scenarioredigeraren.
1. Håll pekaren över den partiella cirkeln till höger om modulen och klicka sedan på **[!UICONTROL Add another module]**.
1. Välj [!DNL Adobe Workfront] i listan med program och välj sedan modulen **[!UICONTROL Update Record]**.
1. i fältet ID markerar du det ID-block som finns under objektmodulen Konvertera. Detta är ID:t för det projekt som skapades av den modulen.

   ![ID från Konvertera objekt](assets/id-convert-object.png)

1. Välj Projekt i fältet Posttyp eftersom objektet som ska uppdateras är ett projekt.
1. Välj Namn i området Välj fält att mappa.

   Ett namnfält öppnas.

### Mappa funktionen för namnuppdatering

När det här scenariot konverterar en begäran till ett projekt är projektets namn detsamma som begäran. Funktionen här har det namnet och alla bokstäver i det får en inledande versal.

1. Klicka på fältet **Namn**.

   Mappningspanelen öppnas.
1. Klicka på ikonen **Text och binära funktioner** på mappningspanelen. ![Ikon för textfunktioner](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Markera funktionen **upper**.

   Funktionen visas i fältet Namn, inklusive formateringen för de indata som förväntas.

   Indata för det här exemplet är namnet på det problem som projektet konverterades från.

1. Flytta markören mellan parenteserna eftersom det är här inmatningen ska placeras.
1. Klicka på ikonen **modulutdata** på mappningspanelen. ![Ikon för modulutdata](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Markera namnblocket som utdata från din första modul.

   Namnblocket visas i funktionen.

   ![Namnblock i funktion](assets/map-name.png)

1. Klicka på OK för att spara modulinställningarna.

### Testa och aktivera

1. Testa scenariot genom att klicka på **Kör en gång** i skärmens nedre vänstra hörn.
1. Granska utdata för att kontrollera att scenariot kördes som förväntat.
1. När du är säker på att scenariot fungerar som förväntat klickar du på växeln **Schemaläggning** längst ned till vänster på skärmen till **På**.

   Detta aktiverar scenariot. Aktiva scenarier körs enligt det schema som angetts i utlösarmodulen.
1. I [!DNL Workfront Fusion] klickar du på **[!UICONTROL Save]** i det nedre vänstra hörnet för att spara förloppet för scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

## Resurser:

* [Mappa objekt med funktioner i  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
