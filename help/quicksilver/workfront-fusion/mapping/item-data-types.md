---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Objektdatatyper i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Objektdatatyper i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Objektdatatyper](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/data-types/item-data-types.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

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

## Artikeldatatyper

Du kan innehålla de typer av objekt som listas nedan i ett paket.

Mer information om vilka typer av objekt [!DNL Workfront Fusion] tillåter konvertering mellan varandra finns i [Typtvång in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Text</p> </td> 
   <td> <p>Den vanligaste artikeltypen. För vissa textobjekt kontrollerar [!DNL Adobe Workfront Fusion] om den högsta eller lägsta tillåtna längden uppfylls eller om objektet utför formatvalidering (e-post, URL eller filnamn).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Nummer</p> </td> 
   <td> <p>För vissa numeriska objekt kan [!DNL Workfront Fusion] validera indata för ett angivet intervall (det lägsta eller högsta tillåtna värdet).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Boolean (Ja/Nej)</p> </td> 
   <td> <p>Den här typen används för objekt med endast två möjliga värden: true eller false. </p> <p>När du anger moduler kan den booleska typen visas i två olika former:</p> 
    <ul> 
     <li> <p>Den obligatoriska kryssrutan visas om fältet är obligatoriskt och måste fyllas i.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Valfria fält som kan lämnas tomma visas som en valruta, vilket gör att du kan välja mellan tre värden: <code>Yes</code>, <code>No</code> och <code>Not defined</code> (standard).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Du kan klicka på <strong>[!UICONTROL Map]</strong> om du behöver mappa värdet till ett objekt från en annan modul.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datum</p> </td> 
   <td> <p>Datum anges i ISO 8601-datumformat, till exempel <code>2015-09-18T11:58Z</code>. Du kan ändra tidszonen i dina profilinställningar enligt beskrivningen i <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Ändra profilinställningar i [!DNL Adobe Workfront Fusion]</a>. </p> <p>Om du klickar på ett fält som kräver ett datum visas en popup-kalender i modulinställningarna. Tiden krävs inte för vissa objekt.</p> <p>Värden för Date-objekt formateras med den lokala tidszonen och webbtidszonen som är vald i din profil. Du kan visa ISO 8601-versionen av ett datumobjekts värde genom att hålla markören över objektet.</p> <p>Obs! Om ISO-värdet inte visas är objektet förmodligen text, inte ett datum.</p> <p>Tiden anges i formatet <code>hours:minutes:seconds</code>, till exempel <code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffert (binära data)</p> </td> 
   <td> <p>Filinnehåll skickas vanligtvis som bufferttypsinnehåll (bildinnehåll, videofil med flera). I vissa fall inkluderas textdata i den här typen (till exempel en textfil). [!DNL Workfront Fusion] kan automatiskt konvertera textdata i binär kod till text och text till textdata i binär kod. Mer information finns i <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Om att mappa filer i [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Samling</p> </td> 
   <td> <p>En samling är ett objekt som består av flera underposter. Avsändarobjektet i ett e-postmeddelande är ett exempel på en samling: det innehåller avsändarens namn (texttyp) och avsändarens e-postadress (texttyp).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Markera (meny)</p> </td> 
   <td> <p>När du konfigurerar modulinställningarna enligt beskrivningen i <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Konfigurera en moduls inställningar i [!DNL Adobe Workfront Fusion]</a> kan du välja bland flera objekt av samma typ. Ett exempel är mappvalsmenyn i inställningarna för modulerna [!DNL Dropbox]. </p> <p>När du ställer in moduler kan urvalsmenyn visas i två former:</p> <p> <p>Om det går att markera flera objekt visas flera objekt med kryssrutor.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Om bara ett alternativ är möjligt visas en listruta.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Om du behöver mappa ett objekt från en annan modul använder du knappen <strong>Karta</strong> . Med den här knappen öppnas ett textfält i stället för en markeringsmeny. Mer information finns i <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>Du kan använda arraytypen för att arbeta med flera värden av samma typ, inklusive samlingar. Ett exempel är modulerna [!UICONTROL Email]: de returnerar en matris med bilagor och varje bifogad fil innehåller namn, innehåll, storlek och så vidare. Mer information finns i <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Mappa en array i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validering</p> </td> 
   <td> <p>[!DNL Workfront Fusion] kan utföra validering för varje typ av objekt. Om ett objekt inte godkänns i valideringen avbryts bearbetningen av modulen på grund av ett datafel. Mer information finns i <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Felbearbetning i [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
