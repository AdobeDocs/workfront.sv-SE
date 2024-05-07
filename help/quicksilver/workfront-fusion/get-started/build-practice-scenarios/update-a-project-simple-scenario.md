---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Lägga till en utlösarmodul i ett grundläggande scenario
description: Lär dig hur du lägger till en utlösarmodul så att scenariot regelbundet kan söka efter nya begäranden och konvertera dem till projekt.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Använda en funktion för att uppdatera ett projekt i ett enkelt scenario i [!DNL Adobe Workfront Fusion]

Att uppdatera en arbetsuppgift från Workfront är ett vanligt användningsområde för Workfront Fusion. I det här exemplet använder du en funktion för att ändra namnet på ett projekt till versaler.

Fusion innehåller många typer av funktioner som gör att du kan omvandla och utföra villkorsstyrd logik på dina data. Mer information om hur du använder funktioner finns i [Mappa information från en modul till en annan i Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

I det här exemplet ändras scenariot som skapas i [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Förutsättningar

Du måste skapa scenariot enligt [Skapa ett grundläggande scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) innan du följer den här proceduren.

## Uppdatera ett projekt med en funktion

### Lägg till modulen Uppdatera post i ditt scenario

1. Öppna scenariot i scenarioredigeraren.
1. Håll pekaren över den partiella cirkeln till höger om modulen och klicka sedan på **[!UICONTROL Add another module]**.
1. Välj [!DNL Adobe Workfront] i listan över program och välj sedan modulen **[!UICONTROL Update Record]**.
1. i fältet ID markerar du det ID-block som finns under objektmodulen Konvertera. Detta är ID:t för det projekt som skapades av den modulen.

   ![ID från Konvertera objekt](assets/id-convert-object.png)

1. Välj Projekt i fältet Posttyp eftersom objektet som ska uppdateras är ett projekt.
1. Välj Namn i området Välj fält att mappa.

   Ett namnfält öppnas.

### Mappa funktionen för namnuppdatering

När det här scenariot konverterar en begäran till ett projekt är projektets namn detsamma som begäran. Funktionen här har det namnet och alla bokstäver i det får en inledande versal.

1. Klicka på **Namn** fält.

   Mappningspanelen öppnas.
1. Klicka på knappen **Text- och binärfunktioner** -ikon. ![Ikon för textfunktioner](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Markera funktionen **uppåt**.

   Funktionen visas i fältet Namn, inklusive formateringen för de indata som förväntas.

   Indata för det här exemplet är namnet på det problem som projektet konverterades från.

1. Flytta markören mellan parenteserna eftersom det är här inmatningen ska placeras.
1. Klicka på knappen **modulutdata** -ikon. ![Ikon för modulutdata](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Markera namnblocket som utdata från din första modul.

   Namnblocket visas i funktionen.

   ![Namnblock i funktion](assets/map-name.png)

1. Klicka på OK för att spara modulinställningarna.

### Testa och aktivera

1. Testa scenariot genom att klicka **Kör en gång** i skärmens nedre vänstra hörn.
1. Granska utdata för att kontrollera att scenariot kördes som förväntat.
1. När du är säker på att scenariot fungerar som väntat klickar du på **Schemaläggning** växla i det nedre vänstra hörnet av skärmen till **På**.

   Detta aktiverar scenariot. Aktiva scenarier körs enligt det schema som angetts i utlösarmodulen.
1. I [!DNL Workfront Fusion], klicka **[!UICONTROL Save]** nära det nedre vänstra hörnet för att spara dina framsteg i scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

## Resurser:

* [Mappa objekt med funktioner i [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
