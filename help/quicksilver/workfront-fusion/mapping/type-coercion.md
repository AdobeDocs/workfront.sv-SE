---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Typtvång i Adobe Workfront Fusion
description: I det här dokumentet beskrivs hur  [!DNL Adobe Workfront Fusion] fungerar i situationer när värden tas emot i förväntade och oväntade dataformat.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: d09174b874ff59676a28881de02ae4e7196d0f80
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Typtvång i [!DNL Adobe Workfront Fusion]

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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

+++

### Typtvång

Det här dokumentet beskriver hur [!DNL Adobe Workfront Fusion] beter sig i situationer när det tar emot värden i förväntade och oväntade dataformat.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Förväntat</th> 
   <th>Mottaget</th> 
   <th> <p>Beskrivning</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>array </td> 
   <td>array </td> 
   <td> <p>Värdet överförs oförändrat.</p> </td> 
  </tr> 
  <tr> 
   <td>array </td> 
   <td>övriga </td> 
   <td> <p>Om det mottagna värdet inte är av arraytyp skapar [!DNL Workfront Fusion] en array och det första (och enda) elementet blir det mottagna värdet.</p> </td> 
  </tr> 
  <tr> 
   <td>boolesk </td> 
   <td>boolesk </td> 
   <td> <p>Värdet överförs oförändrat.</p> </td> 
  </tr> 
  <tr> 
   <td>boolesk </td> 
   <td>tal </td> 
   <td> <p>Värdet konverteras till logiskt Ja, även om värdet är 0.</p> </td> 
  </tr> 
  <tr> 
   <td>boolesk </td> 
   <td>text </td> 
   <td> <p>Om värdet är lika med false eller om värdet är tomt konverteras det till logiskt Nej. Annars konverteras den till logiskt Ja.</p> </td> 
  </tr> 
  <tr> 
   <td>boolesk </td> 
   <td>övriga </td> 
   <td> <p>Värdet konverteras till logiskt Ja när det mottagna värdet finns (är inte null).</p> </td> 
  </tr> 
  <tr> 
   <td>buffert </td> 
   <td>buffert </td> 
   <td> <p>Värdet ändras bara om teckentabellen är som förväntat. Om teckentabellen skiljer sig försöker [!DNL Workfront Fusion] konvertera det mottagna värdet till den begärda teckentabellen. Om konverteringen inte stöds returnerar [!DNL Workfront Fusion] ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>buffert </td> 
   <td>boolesk </td> 
   <td> <p>Värdet konverteras till text (true/false) och sedan till binära data enligt stegen ovan för konvertering till text.</p> </td> 
  </tr> 
  <tr> 
   <td>buffert </td> 
   <td>datum </td> 
   <td> <p>Värdet konverteras till ISO 8601-text och sedan till binära data enligt de steg som anges för konvertering till text.</p> </td> 
  </tr> 
  <tr> 
   <td>buffert </td> 
   <td>tal </td> 
   <td> <p>Värdet konverteras till text och sedan till binära data enligt stegen ovan för konvertering till text.</p> </td> 
  </tr> 
  <tr> 
   <td>buffert </td> 
   <td>text </td> 
   <td> <p>Värdet konverteras till binära data och kodas som förväntat. Om den förväntade kodningen inte anges kommer utf8-kodning att användas.</p> </td> 
  </tr> 
  <tr> 
   <td>buffert </td> 
   <td>övriga </td> 
   <td> <p>[!DNL Workfront Fusion] returnerar ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>samling </td> 
   <td>samling </td> 
   <td> <p>Värdet överförs oförändrat.</p> </td> 
  </tr> 
  <tr> 
   <td>samling </td> 
   <td>övriga </td> 
   <td> <p>[!DNL Workfront Fusion] returnerar ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>datum </td> 
   <td>datum </td> 
   <td> <p>Värdet överförs oförändrat.</p> </td> 
  </tr> 
  <tr> 
   <td>datum </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] försöker konvertera texten till ett datum. Om konverteringen misslyckas returneras ett valideringsfel. Datum måste innehålla dag, månad och år. Datum kan innehålla tid- och tidszon. Standardtidszonen baseras på dina inställningar. Exempel:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>datum </td> 
   <td>övriga </td> 
   <td> <p>[!DNL Workfront Fusion] returnerar ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>tal </td> 
   <td>tal </td> 
   <td> <p>Värdet överförs oförändrat.</p> </td> 
  </tr> 
  <tr> 
   <td>tal </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] försöker konvertera texten till ett tal. Om konverteringen misslyckas returneras ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>tal </td> 
   <td>övriga </td> 
   <td> <p>[!DNL Workfront Fusion] returnerar ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>Värdet överförs oförändrat.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>array </td> 
   <td> <p>Om den angivna arrayen stöder konvertering till text, konverteras värdet. Annars returnerar [!DNL Workfront Fusion] ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>boolesk </td> 
   <td> <p>Värdet konverteras till text (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffert </td> 
   <td> <p>Om textkodning anges för binära data konverteras värdet till text. Annars returnerar [!DNL Workfront Fusion] ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>datum </td> 
   <td> <p>Värdet konverteras till ISO 8601-text.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>tal </td> 
   <td> <p>Värdet konverteras till text.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>övriga </td> 
   <td> <p>[!DNL Workfront Fusion] returnerar ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>tid </td> 
   <td>tid </td> 
   <td> <p>Värdet överförs oförändrat.</p> </td> 
  </tr> 
  <tr> 
   <td>tid </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] kommer att försöka konvertera tiden till formatet :minutes: sekunder. Om konverteringen misslyckas returneras ett valideringsfel.</p> </td> 
  </tr> 
  <tr> 
   <td>tid </td> 
   <td>övriga </td> 
   <td> <p>[!DNL Workfront Fusion] returnerar ett valideringsfel.</p> </td> 
  </tr> 
 </tbody> 
</table>
