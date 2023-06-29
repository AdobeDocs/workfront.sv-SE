---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Routermodul i Adobe Workfront Fusion
description: Med routermodulen kan du dela in ditt flöde i flera flöden och bearbeta data i varje flöde på olika sätt. När en routermodul tar emot ett paket vidarebefordrar den till varje ansluten rutt i den ordning som rutterna kopplades till routermodulen.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# [!UICONTROL Router] modulen i [!DNL Adobe Workfront Fusion]

The [!UICONTROL Router] kan du dela in ditt flöde i flera olika flöden och bearbeta data i varje flöde på olika sätt. En gång en [!UICONTROL Router] modulen tar emot ett paket som vidarebefordrar det till varje ansluten rutt i den ordning som rutterna kopplades till [!UICONTROL Router] -modul.

>[!NOTE]
>
>* Om du vill verifiera ordningen på rutterna kan du klicka på [!UICONTROL Auto-align] -ikonen som ordnar rutterna enligt ordningen uppifrån och ned.
>
>  Om du vill ändra ordningen tar du bort [!UICONTROL Router] och återanslut vägarna i önskad ordning.
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
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Lägga till en [!UICONTROL Router] modulen till ett scenario

A [!UICONTROL Router] kan läggas till i ett scenario på något av följande sätt:

* Om du vill ansluta [!UICONTROL Router] efter en modul, klicka på modulens högra handtag och börja skriva **[!UICONTROL router]** för att söka efter den och sedan välja **[!UICONTROL Flow Control]** > **[!UICONTROL Router]** i listan med moduler som visas.

  ![](assets/connect-the-router-350x108.png)

* Om du vill infoga [!UICONTROL Router] mellan två moduler, klicka på skiftnyckelsikonen under vägen som förbinder de två modulerna (eller högerklicka på flödet) och välj **[!UICONTROL Add a router]** på menyn.

  ![](assets/insert-router-350x191.png)

* Du kan infoga en [!UICONTROL Router] automatiskt. Om du till exempel vill ansluta modulen i det nedre högra hörnet i bilden nedan till den i det övre vänstra hörnet (som redan är ansluten till den i det övre högra hörnet) drar du handtaget i den nedre högra modulen och släpper den i den övre vänstra modulen.

  ![](assets/insert-router-automatically-350x379.png)

## Filter

Du kan lägga ett filter på en väg efter [!UICONTROL Router] för att filtrera paket som på andra vägar:

1. Klicka på en av punkterna i flödet.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. I **[!UICONTROL Set up a filter]** ruta som visas, lägg till villkor och klicka sedan **[!UICONTROL OK]** för att spara filterinställningarna.

   ![](assets/set-up-a-filter-2-350x242.png)

Mer information finns i [Lägga till ett filter i ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Reservrutten

Filterinställningen på en väg efter en [!UICONTROL Router] modulen innehåller ett specialalternativ: Återgångsvägen:

![](assets/fallback-route-350x260.png)

När det här alternativet är aktiverat används den här vägen när ett paket inte kan fortsätta från [!UICONTROL Router] modulen via någon annan väg eftersom filtren på de andra vägarna filtrerade ut den.

Fallback-vägen urskiljs med en annan pilsymbol inuti [!UICONTROL Router] modul:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Ett typiskt användningsfall för reservflödet är att fortsätta flödet med ett flöde om villkoret är uppfyllt och med ett annat flöde om det inte är det, som i följande steg:

1. Infoga en [!UICONTROL Router] i ditt scenario.
1. Koppla båda vägarna till [!UICONTROL Router] modul .
1. Klicka på den första vägen och ange ett villkor:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Klicka på den andra vägen och aktivera [!UICONTROL fallback route] alternativ:

   ![](assets/enable-fallback-route-option-350x238.png)
