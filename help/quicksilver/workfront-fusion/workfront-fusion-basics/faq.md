---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Vanliga frågor om Adobe Workfront Fusion
description: I den här artikeln behandlas vanliga frågor om [!DNL Adobe Workfront Fusion], inklusive information om objekt som ofta används i Fusion-arbetsflöden
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f2d67401782abc7e7714d9e14c495a4a6ba2fcc7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Vanliga frågor om Adobe Workfront Fusion

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Vad är ett scenario?

### Svar

Ett scenario definierar en sekvens av steg som ska köras av [!DNL Adobe Workfront Fusion]. För varje scenario anger du datakällan, hur data ska behandlas och vilka data som ska användas och vad som ska ignoreras. [!DNL Workfront Fusion] gör att du kan skapa så komplexa scenarier som du behöver, även de mest avancerade scenarierna är möjliga.

Mer information finns i [Skapa ett scenario för praktikintegrering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Kan jag använda mer än en modul i ett scenario? Eller bara en utlösare och en handling?

### Svar

Du kan använda så många moduler du vill i ett scenario. Du kan skapa oberoende flöden och ange vilka data som ska flöda genom dem. Du kan också använda resultat som returneras av enskilda åtgärder och sedan skicka dem vidare till nästa åtgärd.

## Kan [!DNL Workfront Fusion] arbeta med filer?

### Svar

Ja. Använda [!DNL Workfront Fusion], kan filer tas emot, sparas, omformas, konverteras, krypteras och så vidare. Dessutom [!DNL Workfront Fusion] innehåller ett stort antal inbyggda funktioner som gör att användarna kan arbeta effektivt och kreativt med de data som finns i filerna.

Mer information finns i [Om att mappa filer i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Vad händer om jag släpper [!DNL Workfront Fusion] Vill du bearbeta ett e-postmeddelande som innehåller mer än en bifogad fil?

### Svar

Om du använder [!UICONTROL Email] modul [!UICONTROL Retrieve attachments], skickas varje bifogad fil separat genom resten av modulerna i scenariot. Liknande moduler är också tillgängliga i andra program som tar emot flera filer samtidigt.

Mer information finns i [[!UICONTROL Email] moduler](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Vissa utlösare gör att scenarier kan köras direkt. Vad betyder&quot;direkt&quot;?

### Svar

Vanliga scenarier körs med intervall enligt det schema du anger (t.ex. varje timme, var femte minut, en gång i månaden och så vidare). Det finns särskilda utlösare, så kallade direktutlösare (webhooks), som kan starta ditt scenario omedelbart efter att de har tagit emot data från en viss tjänst. Direktutlösare kan vara mycket användbara. Vi rekommenderar att du använder dem när det är möjligt. De hjälper till att minska antalet åtgärder. Mottagna data bearbetas omedelbart utan att vänta på nästa schemalagda körning. Till exempel [!DNL Google Sheets] modul [!UICONTROL Watch Changes] startar ett scenario omedelbart efter att en cell har uppdaterats.

## Vad är aggregatorer?

### Svar

An [!UICONTROL Aggregator] sammanfogar data i en enda samling. Ett exempel på detta är filer som komprimeras till ett ZIP-arkiv och skickas som en e-postbilaga.

Mer information finns i [[!UICONTROL Aggregator] modulen i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Vad är en operation?

### Svar

En åtgärd är en åtgärd som utförs av en modul. En åtgärd utförs till exempel varje gång en utlösare körs och varje gång en åtgärd utför en åtgärd.

## Vad är dataöverföring?

### Svar

Dataöverföring avser mängden data som överförs genom ditt scenario. Anta till exempel att du har ett scenario som hämtar en 100 kB-bild från FTP och minskar dess storlek till 50 kB och sparar båda bilderna som [!DNL Dropbox]. Mängden data som används i detta scenario är 250 kB.

## Vad är en anslutning?

### Svar

En anslutning är länken mellan [!DNL Workfront Fusion] konto och den tredjepartstjänst som du vill använda. Anslutningen kan enkelt skapas när du redigerar ett scenario. Om du vill lägga till en anslutning klickar du på **[!UICONTROL Add]** i modulinställningarna och följ instruktionerna steg för steg.

Mer information finns i [Om att ansluta [!DNL Adobe Workfront Fusion] till en app eller tjänst](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
