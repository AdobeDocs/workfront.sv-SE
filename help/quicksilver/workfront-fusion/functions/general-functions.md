---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Allmänna funktioner i Adobe Workfront Fusion
description: Följande allmänna funktioner är tillgängliga på panelen för mappning av Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: a5130e551ad73717796bfac206d99799efc7987d
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Allmänna funktioner i [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get (object or array; path)]

Returnerar värdesökvägen för ett objekt eller en array. Använd punktnotation om du vill komma åt kapslade objekt. Det första objektet i en array är index 1.

>[!INFO]
>
>**Exempel:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (expression; value1; value2)]

Returnerar `value1` om uttrycket utvärderas till true, annars returneras `value2`.

>[!INFO]
>
>**Exempel:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Returnerar A
>
>* `if( = 2 ; A ; B )`
>
>   Returnerar B

## [!UICONTROL ifempty (value1; value2)]

Returnerar `value1` om det här värdet inte är tomt, annars returneras `value2`.

>[!INFO]
>
>**Exempel:**
>
>* `ifempty(` `A` `;` `B` )
>
>   Returnerar A
>
>* `ifempty(` `unknown` `;` `B` )
>
>   Returnerar B
>
>* `ifempty(` `""` `;` `B` )
>
>   Returnerar B

## [!UICONTROL switch (expression; value1; result1; [value2; result2; ...]; [else])]

Utvärderar ett värde (kallas uttryck) mot en lista med värden. Returnerar resultatet som motsvarar det första matchande värdet.

>[!INFO]
>
>**Exempel:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Returnerar 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Returnerar 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>  Returnerar 4

## [!UICONTROL omit(object; key1; [key2; ...])]

Utelämnar de angivna tangenterna för objektet och returnerar resten.

>[!INFO]
>
>**Exempel:**
>
>`omit(` Användare `;` lösenord `)`
>
>Returnerar en samling med användarens information, exklusive lösenordet.

## [!UICONTROL pick(object; key1; [key2; ...])]

Hämtar endast de angivna nycklarna från objektet.

>[!INFO]
>
>**Exempel:**
>
>`pick(` Användare `;` lösenord `;` e-postadress `)`
>
>Returnerar en samling med endast användarens lösenord och e-postadress.
