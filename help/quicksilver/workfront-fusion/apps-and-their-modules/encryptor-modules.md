---
title: Krypterare
description: Med Adobe Workfront Fusion Encryptor-modulerna kan du kryptera alla textdata. De har för närvarande stöd för meddelandekryptering via AES256 och PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Krypterare

[!DNL Adobe Workfront Fusion] [!UICONTROL Encryptor] kan du kryptera alla textdata. De har för närvarande stöd för meddelandekryptering via AES256 och PGP ([!UICONTROL OpenPGP]).

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

## Meddelandekryptering och dekryptering med PGP

När du krypterar och dekrypterar via PGP måste du använda en nyckelring och skapa en privat eller offentlig nyckel (eller båda).

Mer information om publika och privata nycklar finns i [Grundläggande termer i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Mer information om nyckelkedjor finns i [Tangenter i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Encryptor] moduler och deras fält

När du konfigurerar [!UICONTROL Encryptor] visas följande fält. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

### Kryptera ett PGP-meddelande

Med den här modulen kan du kryptera ett meddelande med offentliga och privata nycklar.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Ange avsändarens privata nyckel. Detta kan autentisera avsändarens identitet.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Ange mottagarens offentliga nyckel.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Ange meddelandet som du vill kryptera.</td>
    </tr>

### Dekryptera ett PGP-meddelande

Med den här modulen kan du dekryptera ett meddelande med offentliga och privata nycklar.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Ange mottagarens privata nyckel.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Ange mottagarens offentliga nyckel. Detta kan autentisera avsändarens identitet.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Mappa meddelandet som du vill dekryptera.</td>
    </tr>
</table>
