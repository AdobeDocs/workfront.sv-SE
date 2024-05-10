---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: SOAP-modul
description: Du kan använda SOAP-modulen för att ansluta till SOAP API:er i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: b820fb8d597205da9f2d0e5e6f5aec1056ec9a45
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# [!UICONTROL SOAP] modul

Du kan använda [!UICONTROL SOAP] modul att ansluta till [!UICONTROL SOAP] API:er [!UICONTROL Adobe Workfront Fusion].

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] eller högre</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
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
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Begränsningar i [!UICONTROL SOAP] modul

>[!NOTE]
>
>Omdirigeringar inaktiveras under WDSL-inläsning. Det här är en säkerhetsfunktion, men det kan betyda att overifierade omdirigeringar blockeras när modulen körs.

The [!UICONTROL SOAP] Modulen är för närvarande i betaversion och stöder inte:

* Omdefiniera element
* Begränsningar för bråktal
* Begränsningar för totalt antal siffror
* Begränsningar för tomt utrymme
* Flera delar i in- och utdatameddelanden. Endast meddelanden med en del stöds
* Anpassade XML-schemaelement definierade med hjälp av [[!UICONTROL SOAP] Kodning](https://schemas.xmlsoap.org) scheman och element.

>[!INFO]
>
>**Exempel:**
>  
>Följande känns inte igen korrekt av [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>     <complexContent>
>           <restriction base="soapenc:Array">
>                 <attribute ref="soapenc:arrayType"
>                       wsdl:arrayType="xsd:integer[]"/>
>           </restriction>
>     </complexContent>
></complexType>
>```
>
>Det här exemplet innehåller `soapenc:Array`, `soapenc:arrayType` och `wsdl:arrayType` referenser, som ännu inte stöds i [!UICONTROL Workfront Fusion].

## Tillfällig lösning

Om [!UICONTROL SOAP] modulen vägrar att bearbeta WSDL-filen eller genererar olika fel i modulens konfiguration, du kan försöka med att använda den universella **[!UICONTROL HTTP]>[!UICONTROL Make a request]** i stället:

1. I [!DNL Workfront Fusion]skapar du ett nytt scenario.
1. Infoga **[!UICONTROL HTTP]>[!UICONTROL Make a request]** i scenariot.
1. Öppna modulens konfiguration och fyll i följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL Enabled]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Öppna ett nytt webbläsarfönster eller en ny flik.
1. Klistra in WSDL-URL:en i webbläsarens adressfält och hämta XML-filen.

   WSDL-URL:en avslutas vanligtvis med `?wsdl`, men inte nödvändigtvis, till exempel `http://voip.ms/api/v1/server.wsdl`.

1. Om WSDL-filen inte visas direkt i webbläsaren öppnar du den hämtade filen i en textredigerare.
1. Sök efter `<service>` eller `<wsdl:service>` tagg:

   ![](assets/service-350x65.png)

1. Kopiera URL:en från `location` -attribut.
1. I [!DNL Workfront Fusion], klistra in URL-adressen i HTTP-modulens URL-fält.
1. Öppna [Online [!UICONTROL SOAP] Klient](https://wsdlbrowser.com/) i ett nytt webbläsarfönster/en ny flik.
1. Klistra in WSDL-URL:en i WSDL-URL-fältet.
1. Klicka på **[!UICONTROL Browse]**.
1. Välj från listan med funktioner till vänster, till exempel `getLanguages`.
1. Kopiera innehållet i [!UICONTROL Request XML] textområde.
1. I [!UICONTROL Workfront Fusion], klistra in det kopierade innehållet i modulens URL-fält.
1. Ange värden för valda parametrar genom att ersätta frågetecknen med faktiska värden:

   ![](assets/request-xml-350x172.png)

1. Stäng modulens konfiguration genom att klicka på **[!UICONTROL OK]**.
1. Kör scenariot eller modulen.
