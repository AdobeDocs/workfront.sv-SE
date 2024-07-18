---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenariokörning, cykler och faser i  [!DNL Adobe Workfront Fusion]
description: I den här artikeln beskrivs händelser som inträffar när ett  [!DNL Adobe Workfront Fusion] scenario körs, till exempel initiering, åtgärder, implementeringar och återställningar.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Scenariokörning, cykler och faser i [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] är ett transaktionssystem som liknar relationsdatabaser. Varje scenariokörning börjar med initieringsfasen, fortsätter med minst en cykel bestående av operations- och implementerings-/återställningsfaserna och avslutas med slutförandefasen:

>[!INFO]
>
>**Exempel**
>
>Initiering
>
>Cykel 1
>
>Åtgärd (läsa eller skriva)
>
>Verkställ eller återställ
>
>Cykel 2
>
>Åtgärd (läsa eller skriva)
>
>Verkställ eller återställ
>
>...
>
>Cykel #N
>
>Åtgärd (läsa eller skriva)
>
>Verkställ eller återställ
>
>Slutför

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
  <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Initiering

Under initieringsfasen skapas alla nödvändiga anslutningar (anslutning till en databas, e-posttjänst och så vidare). De kontrolleras också om varje modul kan utföra de avsedda åtgärderna.

## Cyklar

Varje cykel representerar en odelbar arbetsenhet som består av en serie operationer. Det går att ange maximalt antal cykler på panelen [!UICONTROL scenario settings]. Standardvärdet är 1.

Mer information finns i [Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Åtgärd

Under operationsfasen utförs läsning och/eller skrivning:

* Läsåtgärden består av att hämta data från en tjänst som sedan bearbetas av andra moduler enligt ett fördefinierat scenario. Modulen [!UICONTROL Dropbox] >[!UICONTROL Watch files] returnerar till exempel nya paket (filer) som skapats sedan den senaste scenariokörningen.
* Skrivåtgärden består av att skicka data till en viss tjänst för vidare bearbetning. Modulen [!DNL Dropbox] >[!UICONTROL Upload a file] överför till exempel en fil till en [!DNL Dropbox]-mapp.

## Verkställ

Om operationsfasen lyckas för alla moduler börjar den implementeringsfas under vilken alla åtgärder som utförs av modulerna verkställs. Det innebär att [!DNL Workfront Fusion] skickar information till alla tjänster som är inblandade i operationsfasen om att åtgärden lyckades.

## Återställning

Om ett fel inträffar under operations- eller implementeringsfasen i en modul avbryts fasen och återställningsfasen startas, vilket gör alla åtgärder under den angivna cykeln void. Vissa moduler stöder inte återställning och åtgärder som utförs av dessa moduler kan inte återtas. Mer information finns i avsnittet [ACID-moduler](#acid-modules).

## Slutför

Under slutförandefasen stängs öppna anslutningar (till exempel FTP-anslutningar, databasanslutningar och så vidare) och scenariot slutförs.

## ACID-moduler

Alla [!DNL Workfront Fusion]-moduler som stöder återställning (kallas även för transaktioner) markeras med ACID-taggen.

![](assets/acid-modules-350x189.png)

Moduler som inte är markerade med den här taggen kan inte återställas till det ursprungliga läget när fel inträffar i andra moduler. Ett typiskt exempel på en modul som inte är en ACID-modul är åtgärden [!UICONTROL Email] >[!UICONTROL Send an Email]. När e-postmeddelandet har skickats kan du inte ångra det.
