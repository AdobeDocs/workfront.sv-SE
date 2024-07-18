---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Skapa ett enkelt scenario i  [!DNL Adobe Workfront Fusion]
description: Lär dig skapa ett enkelt automatiseringsscenario med Adobe Workfront Fusion. Automatiseringsscenarier automatiserar Workfront-processer, inklusive datamanipulering och -omvandling. Det här exemplet tar dig igenom processen att skapa ett scenario som söker efter ett problem och sedan konverterar det till ett projekt.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 0%

---

# Skapa ett grundläggande scenario i [!DNL Adobe Workfront Fusion]

Rollen för [!DNL Adobe Workfront Fusion] är att automatisera dina processer så att du kan koncentrera dig på nya uppgifter i stället för att upprepa samma uppgifter om och om igen. Det fungerar genom att länka åtgärder inom och mellan program och tjänster för att skapa ett scenario som överför och omvandlar data automatiskt. Scenariot du skapar letar efter data i en app eller tjänst och bearbetar data för att ge det resultat du vill ha.

I det här exemplet går du igenom processen att skapa ett scenario som söker efter ett problem i Workfront och konverterar det till ett projekt.

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

1. Klicka på **Skapa ett nytt scenario** i området **Scenarier**.

   <!--To locate the Scenarios area, see navigation article-->

   Scenarioredigeraren visas och innehåller en tom modul i mitten.

   <!--picture?-->

1. Markera platshållarnamnet **[!UICONTROL New scenario]** i det övre vänstra hörnet och ange sedan ett namn.
1. Fortsätt med [Lägg till och konfigurera den första modulen](#add-and-configure-the-first-module) nedan.

### Lägg till och konfigurera den första modulen

1. Klicka på den tomma modulen för att välja det program du vill välja en modul från.

   En lista över program visas till höger om modulen.

1. Välj **[!DNL Adobe Workfront]**. Om sökfältet inte visas klickar du på sökfältet längst ned i listan, skriver&quot;Workfront&quot; och markerar det när det visas i listan.

   Listan ändras till att visa alla [!DNL Workfront] moduler som du kan använda.

1. Klicka på modulen **[!UICONTROL Search]**.

   Modulkonfigurationsfönstret öppnas.

1. I rutan [!UICONTROL Connection] väljer du din Workfront-anslutning.

   Om du inte har någon Workfront-anslutning kan du läsa [Skapa en anslutning till [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Välj **[!UICONTROL Issue]** i rutan [!UICONTROL Record Type]. Detta anger att modulen endast ska söka efter problem.

   Du kan hitta **[!UICONTROL Issue]** i listan om du börjar skriva ordet [!UICONTROL issue].

1. Välj **[!UICONTROL First Matching Record]** i rutan **[!UICONTROL Result Set]**.

   Detta ställer in modulen så att endast den första posten som uppfyller villkoren returneras.
1. Konfigurera villkoren i området **[!UICONTROL Search criteria]** för att returnera det specifika problemet.

   1. I den första rutan under [!UICONTROL Search Criteria] markerar du det fält som du vill ta med i sökningen. I det här exemplet väljer du **[!UICONTROL Name]**.

      Du kan hitta **[!UICONTROL Name]** i listan om du börjar skriva ordet [!UICONTROL name].
   1. För operatorn klickar du på listrutepilen bredvid **Exist** och ändrar den till [!UICONTROL **Innehåller (skiftlägesokänslig)**].

      Detta gör att modulen kan hitta projekt med de valda orden i namnet, även om du inte anger hela namnet eller anger namnet med fel skiftläge (till exempel versaler).
   1. I det sista fältet under [!UICONTROL Search Criteria] anger du ett ord eller en fras som du vet finns i namnet på det problem du söker efter.

1. I listan **[!UICONTROL Outputs]** markerar du de fält som du vill att modulen ska visa. I det här exemplet väljer du fälten **[!UICONTROL ID]** och **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Du kan använda **Cmd+F** ([!DNL Mac] OS) eller **Ctrl-F** ([!DNL Windows] OS) för att snabbt hitta ett fält.

1. Klicka på **[!UICONTROL OK]** för att spara modulkonfigurationen.

1. Högerklicka på modulen, klicka på **[!UICONTROL Rename]**, skriv ett namn som beskriver vad du vill att modulen ska göra (till exempel&quot;Sök efter utgåva&quot;) och klicka sedan på **[!UICONTROL OK]**.

   Namnet visas precis nedanför modulen. Under det finns en kort beskrivning av den typ av åtgärd som har utförts av modulen i [!DNL Workfront Fusion].

   ![](assets/)

1. Fortsätt med [Lägg till och konfigurera den andra modulen](#add-and-configure-the-second-module).

## Lägg till och konfigurera den andra modulen

1. Håll pekaren över den partiella cirkeln till höger om modulen och klicka sedan på **[!UICONTROL Add another module]**.
1. Välj [!DNL Adobe Workfront] i listan med program och välj sedan modulen **[!UICONTROL Misc Action]**.

   I modulen Diverse åtgärder kan du utföra åtgärder i Workfront som inte har någon dedikerad modul. I det här exemplet används den här modulen för att konvertera utgåvan till ett projekt.
1. I fältet [!UICONTROL Connection] väljer du samma Workfront-anslutning som du använde i den tidigare modulen.
1. I fältet **[!UICONTROL Record type]**väljer du **[!UICONTROL Issue]** eftersom åtgärden som ska utföras är relaterad till ett problem.
1. Välj **convertToProject** i fältet **[!UICONTROL Action]**. Detta är den åtgärd som kommer att konvertera den valda utgåvan till ett projekt.
1. Klicka på fältet **[!UICONTROL ID]**.

   En panel öppnas där du kan välja vad som ska användas som ID för det problem som du vill konvertera till ett projekt. Panelen innehåller utdata från tidigare moduler. Eftersom du valde ID som utdata från den tidigare modulen är det nu tillgängligt på panelen.

   Panelen kallas för mappningspanelen. Mer information om mappningspanelen finns i [Mappa information från en modul till en annan](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Välj **ID** på mappningspanelen.

   Ett ID-block visas i ID-fältet. Här visas numret på den modul som modulen mappas från och fältet som mappas.

   ![Mappnings-ID](assets/map-id.png)

1. (Valfritt) I projektavsnittet letar du reda på fältet Ägar-ID och börjar skriva ditt namn i fältet. Markera det sedan när det visas. Då blir du projektägare och det blir enklare att hitta i Workfront.

   >[!TIP]
   >
   >Du kan använda **Cmd+F** ([!DNL Mac] OS) eller **Ctrl-F** ([!DNL Windows] OS) för att snabbt hitta ett fält.

1. Klicka på **[!UICONTROL OK]** för att spara modulkonfigurationen.

1. Högerklicka på modulen, klicka på **[!UICONTROL Rename]**, skriv ett namn som beskriver vad du vill att modulen ska göra (till exempel&quot;Konvertera till projekt&quot;) och klicka sedan på **[!UICONTROL OK]**.

1. Fortsätt till [Testa scenariot](#test-the-scenario).

## Testa scenariot

Innan du aktiverar ditt scenario är det viktigt att du testar det genom att köra det minst en gång och visa resultatet. Detta hjälper er att förstå hur data flödar genom scenariot och hitta eventuella fel.

I det här scenariot skulle ett lyckat test resultera i att problemet hittas och konverteras till ett projekt.

1. Klicka på **[!UICONTROL Run once]** i det nedre vänstra hörnet i scenarioredigeraren.
1. När scenariot är klart klickar du på bubblan ovanför den första modulen för att visa information om det datapaket som modulen har bearbetat, inklusive data som hämtats från det problem som modulen returnerade.

1. Klicka på exekveringspanelen ovanför den andra modulen för att visa indata (problemet) och utdata (det konverterade projektet).

   Mer information om data i inspektionsbubblorna finns i:

   * Allmän information finns i [Körningsflöde för scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Mer information om bearbetade paket finns i [Scenariokörning, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. I [!DNL Workfront Fusion] klickar du på **[!UICONTROL Save]** i det nedre vänstra hörnet för att spara förloppet för scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

>[!TIP]
>
>Vi rekommenderar den valfria men användbara metoden att lägga till anteckningar om varje modul.
>
>1. Högerklicka på en [!DNL Workfront]-modul och klicka sedan på **[!UICONTROL Add a note]**.
>1. Skriv en översikt för modulen i anteckningen som visas.
>
>    Du kan lägga till flera anteckningar för en modul.
>
>1. Stäng området **[!UICONTROL Notes]**.
>
>     När du har lagt till en anteckning i ett scenario visas en orange punkt på ikonen **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) längst ned i scenarioredigeraren.
>
>1. Klicka på ikonen **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) för att visa dina anteckningar.
>

## Aktivera scenariot

Det sista steget i att skapa ett scenario är att aktivera det.

Eftersom det här scenariot söker efter ett specifikt problem behöver det inte aktiveras. När du aktiverar ett scenario körs det enligt ett schema eller när en viss åtgärd inträffar i ett program. När du har aktiverat ett scenario körs det som standard var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta du vill att det ska köras.

Mer information om att aktivera scenarier finns i [Aktivera eller inaktivera ett scenario i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Mer information om scheman finns i [Schemalägg ett scenario i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
