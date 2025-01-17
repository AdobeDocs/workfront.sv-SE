---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Vanliga frågor om Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Vanliga frågor om Adobe Workfront Fusion

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Vanliga frågor om scenarioplanering](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/faq.html)
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

## Vad är ett scenario?

### Svar

Ett scenario definierar en serie steg som ska köras av [!DNL Adobe Workfront Fusion]. För varje scenario anger du datakällan, hur data ska behandlas och vilka data som ska användas och vad som ska ignoreras. Med [!DNL Workfront Fusion] kan du skapa så komplexa scenarier som du behöver. Även de mest avancerade scenarierna är möjliga.

Mer information finns i [Skapa ett scenario för praktikintegrering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Kan jag använda mer än en modul i ett scenario? Eller bara en utlösare och en handling?

### Svar

Du kan använda så många moduler du vill i ett scenario. Du kan skapa oberoende flöden och ange vilka data som ska flöda genom dem. Du kan också använda resultat som returneras av enskilda åtgärder och sedan skicka dem vidare till nästa åtgärd.

## Kan [!DNL Workfront Fusion] arbeta med filer?

### Svar

Ja. Med [!DNL Workfront Fusion] kan filer tas emot, sparas, omformas, konverteras, krypteras och så vidare. Dessutom innehåller [!DNL Workfront Fusion] ett stort antal inbyggda funktioner som är utformade för att användarna ska kunna arbeta effektivt och kreativt med data i filerna.

Mer information finns i [Om att mappa filer i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Vad händer om jag låter [!DNL Workfront Fusion] bearbeta ett e-postmeddelande som innehåller mer än en bifogad fil?

### Svar

Om du använder [!UICONTROL Email]-modulen [!UICONTROL Retrieve attachments] skickas varje bifogad fil individuellt genom resten av modulerna i scenariot. Liknande moduler är också tillgängliga i andra program som tar emot flera filer samtidigt.

Mer information finns i [[!UICONTROL Email] moduler](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Vissa utlösare gör att scenarier kan köras direkt. Vad betyder&quot;direkt&quot;?

### Svar

Vanliga scenarier körs med intervall enligt det schema du anger (t.ex. varje timme, var femte minut, en gång i månaden och så vidare). Det finns särskilda utlösare, så kallade direktutlösare (webhooks), som kan starta ditt scenario omedelbart efter att de har tagit emot data från en viss tjänst. Direktutlösare kan vara mycket användbara. Vi rekommenderar att du använder dem när det är möjligt. De hjälper till att minska antalet åtgärder. Mottagna data bearbetas omedelbart utan att vänta på nästa schemalagda körning. [!DNL Google Sheets]-modulen [!UICONTROL Watch Changes] startar till exempel ett scenario omedelbart efter att en cell har uppdaterats.

## Vad är aggregatorer?

### Svar

En [!UICONTROL Aggregator] sammanfogar data i en enda samling. Ett exempel på detta är filer som komprimeras till ett ZIP-arkiv och skickas som en e-postbilaga.

Mer information finns i modulen [[!UICONTROL Aggregator] i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Vad är en operation?

### Svar

En åtgärd är en åtgärd som utförs av en modul. En åtgärd inträffar t.ex. varje gång en utlösare körs och varje gång en åtgärd utför en åtgärd.

## Vad är dataöverföring?

### Svar

Dataöverföring avser mängden data som överförs genom ditt scenario. Anta till exempel att du har ett scenario som hämtar en 100 kB-bild från FTP och minskar dess storlek till 50 kB och sparar båda bilderna i [!DNL Dropbox]. Mängden data som används i detta scenario är 250 kB.

## Vad är en anslutning?

### Svar

En anslutning är länken mellan ditt [!DNL Workfront Fusion]-konto och den tredjepartstjänst som du vill använda. Anslutningen kan enkelt skapas när du redigerar ett scenario. Om du vill lägga till en anslutning klickar du på knappen **[!UICONTROL Add]** i modulinställningen och följer instruktionerna.

Mer information finns i [Anslutningsöversikt](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
