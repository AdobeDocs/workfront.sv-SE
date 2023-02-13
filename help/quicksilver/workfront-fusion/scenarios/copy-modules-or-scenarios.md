---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Kopiera moduler eller scenarier i [!DNL Adobe Workfront Fusion]
description: Kopiera moduler eller scenarier i [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Kopiera moduler eller scenarier i [!DNL Adobe Workfront Fusion]

Du kan kopiera moduler, grupper av moduler eller hela scenarier i [!DNL Adobe Workfront Fusion]. Med den här funktionen kan du återanvända scenarier eller delar av scenarier utan att behöva skapa dem igen

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr>
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Du måste lägga till moduler i ett scenario innan du kan kopiera dem.

## Kopiera en modul eller en grupp moduler

När du kopierar en modul behåller kopian alla fältvärden och inställningar i den ursprungliga modulen.

Du kan klistra in modulen eller modulerna i ett annat område i samma scenario, eller i ett annat scenario.

Tänk på följande när du klistrar in moduler i ett annat scenario.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Fältvärden som hämtar information från en annan modul som du inte kopierat kan inte längre komma åt den informationen. Du måste ange dessa fält för att hämta information från det nya scenariot.
* Om du klistrar in modulerna i ett scenario som ägs av ett annat team eller en annan organisation måste alla anslutningar uppdateras till anslutningar som ägs av den grupp eller organisation som äger det nya scenariot.

### Kopiera moduler

Att kopiera en grupp moduler liknar att kopiera en enda modul.

1. Högerklicka på den modul som du vill kopiera.

   >[!NOTE]
   >
   >Du kan markera mer än en modul genom att hålla ned [!UICONTROL shift] och klicka på de moduler du vill kopiera. Om du kopierar en grupp moduler kopieras även alla kopplingslinjer, filter eller routningslogik mellan dem.

1. Välj **[!UICONTROL Copy module]**.
1. Flytta markören till det område i scenariot där du vill ha en kopia av scenariot.
1. Högerklicka och välj **[!UICONTROL Paste]**.
1. Koppla de inklistrade modulerna till scenariot genom att dra dem till rätt plats i scenariot.

   Du kan också använda kortkommandon för att kopiera och klistra in.

## Kopiera ett scenario genom att klona

När du klonar ett scenario skapas en kopia av scenariot, som du sedan kan redigera.

1. Öppna sidan med scenarioinformation:

   1. Klicka på **[!UICONTROL Scenario]** i den vänstra panelen klickar du på ett scenario som du vill ha information om.

      eller

      Om du arbetar med scenariot i [Scenarioredigeraren i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)klickar du på vänsterpilen ![](assets/exit-editing-arrow.png) nära fönstrets övre vänstra hörn.

1. Högerklicka **[!UICONTROL Options]** längst upp till höger på sidan.
1. Välj **[!UICONTROL Clone]**.
1. (Valfritt) Ange ett namn för det nya scenariot.
1. (Valfritt) Aktivera **[!UICONTROL Keep the states of any new modules the same as those being duplicated]** för att säkerställa att det kopierade scenariot även innehåller information om de senaste posterna som bearbetats av det ursprungliga scenariot.
1. Klicka **[!UICONTROL Save]** för att skapa scenariot.

## Kopiera ett scenario med hjälp av utkast

Scenarioteman representerar arrangemanget, mappningen och fältvärdena för ett givet scenario vid en viss tidpunkt. Du kan exportera en scenarioplan till en JSON-fil på datorn och sedan importera den när du skapar ett nytt scenario. Scenarier som importeras från en scenarioplan kan redigeras.

En scenarioplan representerar hela scenariot. Om du bara vill kopiera vissa moduler från ett scenario, se [Kopiera en modul eller en grupp moduler](#copy-a-module-or-a-group-of-modules) i den här artikeln.

>[!NOTE]
>
>För information om ritningar i samband med [!DNL Adobe Workfront], se [Översikt över utkast](../../administration-and-setup/blueprints/blueprints-overview.md).

### Exportera en scenarioplan

1. I scenariot klickar du på **[!UICONTROL More]** i området för scenarioinställningar.
1. Klicka på **[!UICONTROL Export Blueprint]**.

   En JSON-fil skapas och hämtas till datorn. Du kan hitta den här filen i [!DNL Downloads] mapp.

### Importera en plan

>[!IMPORTANT]
>
>Om du importerar en plan till ett befintligt scenario ersätter scenarioplanen det befintliga scenariot. Du kan inte lägga till en plan i ett befintligt scenario.

1. Börja skapa ett nytt scenario.
1. I scenariot klickar du på **[!UICONTROL More]** i området för scenarioinställningar.
1. Klicka på **[!UICONTROL Import Blueprint]**.
1. Klicka på **[!UICONTROL Browse]**
1. Navigera till den plan som du vill importera och klicka på **[!UICONTROL Open]**.
1. Klicka på **[!UICONTROL Save]**.

   En JSON-fil skapas och hämtas till datorn. Du kan hitta den här filen i [!UICONTROL Downloads] mapp.

## Kopiera och återanvända scenarier med hjälp av mallar

Du kan skapa mallar som utgångspunkt för [!DNL Workfront Fusion] scenarier. När du skapar ett scenario från en mall kan du ändra scenariot utan att ändra mallen. Fältvärden sparas inte i mallar.

Mer information om hur du skapar och använder mallar finns i [Scenariomallar](../../workfront-fusion/scenarios/templates/fusion-templates.md).
