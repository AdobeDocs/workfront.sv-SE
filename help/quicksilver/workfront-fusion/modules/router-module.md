---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Routermodul i Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# [!UICONTROL Router]-modulen i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Lägg till en routermodul och konfigurera vägar](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/router-module.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Med modulen [!UICONTROL Router] kan du dela in ditt flöde i flera flöden och bearbeta data i varje flöde på olika sätt. När en [!UICONTROL Router]-modul tar emot ett paket vidarebefordrar den till varje ansluten väg i den ordning som rutterna kopplades till [!UICONTROL Router]-modulen.

>[!NOTE]
>
>* Om du vill verifiera ordningen på rutterna kan du klicka på ikonen [!UICONTROL Auto-align] som ordnar rutterna i enlighet med ordningen uppifrån och ned.
>
>  Om du vill ändra ordningen tar du bort modulen [!UICONTROL Router] och kopplar om flödena i önskad ordning.
>
>* Rutorna bearbetas sekventiellt, inte parallellt. Ett paket skickas inte till nästa väg förrän det har bearbetats fullständigt av föregående väg.
>



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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
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

## Lägger till en [!UICONTROL Router]-modul i ett scenario

[!UICONTROL Router] kan läggas till i ett scenario på något av följande sätt:

* Om du vill ansluta modulen [!UICONTROL Router] efter en modul klickar du på modulens högra handtag, börjar skriva **[!UICONTROL router]** för att söka efter den och väljer sedan **[!UICONTROL Flow Control]** > **[!UICONTROL Router]** i listan med moduler som visas.

  ![](assets/connect-the-router-350x108.png)

* Om du vill infoga modulen [!UICONTROL Router] mellan två moduler klickar du på skiftnyckelsikonen under vägen som förbinder de två modulerna (eller högerklickar på flödet) och väljer **[!UICONTROL Add a router]** på menyn.

  ![](assets/insert-router-350x191.png)

* Du kan infoga en [!UICONTROL Router]-modul automatiskt. Om du till exempel vill ansluta modulen i det nedre högra hörnet i bilden nedan till den i det övre vänstra hörnet (som redan är ansluten till den i det övre högra hörnet) drar du handtaget i den nedre högra modulen och släpper den i den övre vänstra modulen.

  ![](assets/insert-router-automatically-350x379.png)

## Filter

Du kan lägga ett filter på en väg efter modulen [!UICONTROL Router] för att filtrera paket som på andra vägar:

1. Klicka på en av punkterna i flödet.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. Lägg till villkor i rutan **[!UICONTROL Set up a filter]** som visas och klicka sedan på **[!UICONTROL OK]** för att spara filterinställningarna.

   ![](assets/set-up-a-filter-2-350x242.png)

Mer information finns i [Lägga till ett filter i ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Reservflöde

Filterinställningen på en väg efter en [!UICONTROL Router]-modul innehåller ett specialalternativ: Reservflödet:

![](assets/fallback-route-350x260.png)

När det här alternativet är aktiverat används den här vägen när ett paket inte kan fortsätta från modulen [!UICONTROL Router] via någon annan väg eftersom filtren på de andra vägarna filtrerade ut det.

Reservvägen urskiljs med ett annat piltecken i modulen [!UICONTROL Router]:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Ett typiskt användningsfall för reservflödet är att fortsätta flödet med ett flöde om villkoret är uppfyllt och med ett annat flöde om det inte är det, som i följande steg:

1. Infoga en [!UICONTROL Router]-modul i ditt scenario.
1. Anslut båda vägarna till modulen [!UICONTROL Router].
1. Klicka på den första vägen och ange ett villkor:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Klicka på den andra vägen och aktivera alternativet [!UICONTROL fallback route]:

   ![](assets/enable-fallback-route-option-350x238.png)
