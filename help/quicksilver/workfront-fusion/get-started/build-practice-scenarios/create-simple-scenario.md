---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Skapa ett grundläggande scenario i [!DNL Adobe Workfront Fusion]
description: Lär dig skapa ett enkelt automatiseringsscenario med Adobe Workfront Fusion. Automatiseringsscenarier automatiserar Workfront-processer, inklusive datamanipulering och -omvandling. Det här exemplet tar dig igenom processen att skapa ett scenario som söker efter en [!DNL Workfront] i Workfront och konverterar det till ett projekt.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Skapa ett grundläggande scenario i [!DNL Adobe Workfront Fusion]

Rollen för [!DNL Adobe Workfront Fusion] är att automatisera processerna så att ni kan koncentrera er på nya uppgifter i stället för att upprepa samma uppgifter om och om igen. Det fungerar genom att länka åtgärder inom och mellan program och tjänster för att skapa ett scenario som överför och omvandlar data automatiskt. Scenariot du skapar letar efter data i en app eller tjänst och bearbetar data för att ge det resultat du vill ha.

Det här exemplet tar dig igenom processen att skapa ett scenario som söker efter en [!DNL Workfront] i Workfront och konverterar det till ett projekt.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Skapa ett övningsscenario

### Börja skapa scenariot

1. I **Scenarier** område, klicka **Skapa ett nytt scenario**.

   <!--To locate the Scenarios area, see navigation article-->

   Scenarioredigeraren visas och innehåller en tom modul i mitten.

   <!--picture?-->

1. Välj **[!UICONTROL New scenario]** platshållarnamn i det övre vänstra hörnet och ange sedan ett namn.
1. Fortsätt med [Lägg till och konfigurera den första modulen](#add-and-configure-the-first-module) nedan.

### Lägg till och konfigurera den första modulen

1. Klicka på den tomma modulen för att välja det program du vill välja en modul från.

   En lista över program visas till höger om modulen.

1. Välj **[!DNL Adobe Workfront]**. Om sökfältet inte visas klickar du på sökfältet längst ned i listan, skriver&quot;Workfront&quot; och markerar det när det visas i listan.

   Listan ändras och visar alla [!DNL Workfront] moduler som du kan använda.

1. Klicka på **[!UICONTROL Search]** -modul.

   Modulkonfigurationsfönstret öppnas.

1. I [!UICONTROL Connection] väljer du din Workfront-anslutning.

   Om du inte har någon Workfront-anslutning kan du läsa [Skapa en anslutning till [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. I [!UICONTROL Record Type] ruta, markera **[!UICONTROL Task]**. Detta anger att modulen endast ska söka efter uppgifter.

   Du kan hitta **[!UICONTROL Task]** i listan om du börjar skriva ordet[!UICONTROL task].&quot;

1. I **[!UICONTROL Result Set]** ruta, markera **[!UICONTROL First Matching Record]**.

   Detta ställer in modulen så att endast den första posten som uppfyller villkoren returneras.
1. I **[!UICONTROL Search criteria]** konfigurerar du villkoret att returnera den specifika uppgiften.

   1. I den första rutan under [!UICONTROL Search Criteria]markerar du det fält som du vill ta med i sökningen. I detta exempel väljer du **[!UICONTROL Name]**.

      Du kan hitta **[!UICONTROL Name]** i listan om du börjar skriva ordet[!UICONTROL name].&quot;
   1. För operatorn klickar du på listrutepilen bredvid **Finns** och ändra det till [!UICONTROL **Innehåller (skiftlägesokänslig)**].

      Detta gör att modulen kan hitta projekt med de valda orden i namnet, även om du inte anger hela namnet eller anger namnet med fel skiftläge (till exempel versaler).
   1. I det sista fältet under [!UICONTROL Search Criteria], anger du ett ord eller en fras som du vet finns i namnet på den uppgift du söker efter.

1. I **[!UICONTROL Outputs]** markerar du de fält som du vill att modulen ska visa. I det här exemplet väljer du **[!UICONTROL ID]** och **[!UICONTROL Name]** fält.

   >[!TIP]
   >
   >Du kan använda **Cmd+F** ([!DNL Mac] OS) eller **Ctrl-F** ([!DNL Windows] OS) för att snabbt hitta ett fält.

1. Klicka **[!UICONTROL OK]** för att spara modulkonfigurationen.

1. Högerklicka på modulen och klicka på **[!UICONTROL Rename]** skriver du ett namn som beskriver vad du vill att modulen ska göra (till exempel&quot;Sök efter uppgift&quot;) och klickar sedan på **[!UICONTROL OK]**.

   Namnet visas precis nedanför modulen. Under den, [!DNL Workfront Fusion] innehåller en kort beskrivning av den typ av åtgärd som modulen utför.

   ![](assets/module-renamed-wf.png)

1. Fortsätt med [Lägg till och konfigurera den andra modulen](#add-and-configure-the-second-module).

## Lägg till och konfigurera den andra modulen

1. Håll pekaren över den partiella cirkeln till höger om modulen och klicka sedan på **[!UICONTROL Add another module]**.
1. Välj [!DNL Adobe Workfront] i listan över program och välj sedan modulen **[!UICONTROL Convert object]**.
1. I [!UICONTROL Connection] väljer du samma Workfront-anslutning som du använde i den tidigare modulen.
1. I **[!UICONTROL Record type]** fält, markera **[!UICONTROL Task]**, eftersom modulen konverterar en uppgift.
1. I **[!UICONTROL Convert to]** fält, markera **Projekt**.
1. Klicka på mappningsväxeln bredvid fältet Aktivitets-ID för att aktivera det.

   Växeln blir blå när den är aktiverad. Detta gör att du kan mappa uppgifts-ID:t från föregående modul.

   ![Växla karta](assets/map-toggle.png)
1. Klicka på **[!UICONTROL Task ID]** fält.

   En panel öppnas där du kan välja vad som ska användas som ID för uppgiften som du vill konvertera till ett projekt. Eftersom du har aktiverat mappning innehåller panelen utdata från tidigare moduler. Du har valt ID som utdata från föregående modul, så det är nu tillgängligt på panelen.

   Panelen kallas för mappningspanelen. Mer information om mappningspanelen finns i [Mappa information från en modul till en annan](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Välj **ID** på mappningspanelen.

   Ett ID-block visas i ID-fältet. Här visas numret på den modul som modulen mappas från och fältet som mappas.

   ![Karta-ID](assets/map-id.png)

1. Klicka på **Mall-ID** börjar du skriva namnet på den Workfront-mall som du vill använda för det här projektet och markerar den när den visas i listan.
1. Klicka **[!UICONTROL OK]** för att spara modulkonfigurationen.

1. Högerklicka på modulen och klicka på **[!UICONTROL Rename]** skriver du ett namn som beskriver vad du vill att modulen ska göra (till exempel&quot;Konvertera till projekt&quot;) och klickar sedan på **[!UICONTROL OK]**.

1. Fortsätt till [Testa scenariot](#test-the-scenario).

## Testa scenariot

Innan du aktiverar ditt scenario är det viktigt att du testar det genom att köra det minst en gång och visa resultatet. Detta hjälper er att förstå hur data flödar genom scenariot och hitta eventuella fel.

I det här scenariot skulle ett lyckat test resultera i att den nya uppgiften hittas och konverteras till ett projekt.

1. Klicka **[!UICONTROL Run once]** i det nedre vänstra hörnet av scenarioredigeraren.
1. När scenariot är klart klickar du på bubblan ovanför den första modulen för att visa information om det datapaket som modulen har bearbetat, inklusive data som hämtats från aktiviteten som modulen returnerade.

1. Klicka på exekveringspanelen ovanför den andra modulen för att visa indata (uppgiften) och utdata (det konverterade projektet).

   Mer information om data i inspektionsbubblorna finns i:

   * Allmän information finns i [Scenariokörningsflöde i [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Mer information om bearbetade paket finns i [Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. I [!DNL Workfront Fusion], klicka **[!UICONTROL Save]** nära det nedre vänstra hörnet för att spara dina framsteg i scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

>[!TIP]
>
>Vi rekommenderar den valfria men användbara metoden att lägga till anteckningar om varje modul.
>
>1. Högerklicka på en [!DNL Workfront] och sedan klicka på **[!UICONTROL Add a note]**.
>1. Skriv en översikt för modulen i anteckningen som visas.
>
>    Du kan lägga till flera anteckningar för en modul.
>
>1. Stäng **[!UICONTROL Notes]** område.
>
>     När du har lagt till en anteckning i ett scenario visas en orange punkt på **[!UICONTROL Notes]** icon ![](assets/notes-icon-w-dot.png) längst ned i scenarioredigeraren.
>
>1. Klicka på **[!UICONTROL Notes]** icon ![](assets/notes-icon-w-dot.png) för att visa dina anteckningar.
>

## Aktivera scenariot

Det sista steget i att skapa ett scenario är att aktivera det.

Eftersom det här scenariot söker efter en viss uppgift behöver du inte aktivera den. När du aktiverar ett scenario körs det enligt ett schema eller när en viss åtgärd inträffar i ett program. När du har aktiverat ett scenario körs det som standard var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta du vill att det ska köras.

Mer information om hur du aktiverar scenarier finns i [Aktivera eller inaktivera ett scenario i [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Mer information om scheman finns i [Schemalägg ett scenario i [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Nästa steg

* [Lägga till en utlösarmodul](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) så att scenariot regelbundet kan söka efter nya begäranden och konvertera dem till projekt.
* Lägg till en webkrok så att scenariot kan köras varje gång en begäran anges.
* Lägg till ett filter för att säkerställa att endast vissa begäranden konverteras till projekt.
* Lägg till en funktion som anpassar namnet på det nya projektet.
* Lägg till felhantering för att säkerställa att scenariot är motståndskraftigt mot fel.

