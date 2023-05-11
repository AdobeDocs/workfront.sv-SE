---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: http-modules
title: Använd ömsesidig TLS i HTTP-moduler i Adobe Workfront Fusion
description: Du kan använda Mutual TLS i dina Adobe Workfront Fusion HTTP-moduler, vilket gör att båda sidor av informationstransaktionen kan verifiera den andres identitet.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: e67e6b6d3baf9f17a0a451fa4e1dbc365340f76e
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Använd ömsesidig TLS i HTTP-moduler i [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion kräver [!DNL Adobe Workfront Fusion] utöver en Adobe Workfront-licens.

## Översikt över Ömsesidig TLS

När du skickar data via Internet är det viktigt att se till att de kommer till eller kommer från rätt plats och att bara den avsedda mottagaren kan läsa dem. När TLS är aktiverat använder klienten (dator som begär information) certifikat för att verifiera serverns identitet (dator som tillhandahåller information). Detta gör säkra HTTP-anslutningar.

Med ömsesidig TLS kan den här identitetsbekräftelsen användas på båda sätt. När servern skickar sitt certifikat för att verifiera sin identitet till klienten, begär den även klientens certifikat. Detta garanterar att servern inte skickar information till en plats eller användare som skulle missbruka den.

>[!INFO]
>
>**Exempel:**
>
>* **TLS**: När en person skriver&quot;MyGreatBank.com&quot; i en webbläsare vill de vara säkra på att de går till My Great Bank, inte en webbplats som kan missbrukas eller sälja sin bankinformation. De vill också vara säkra på att deras bankkontoinformation är krypterad.
   >
   >   När webbläsaren (klienten) ansluter till MyGreatBank.com (servern) kräver TLS ett certifikat från MyGreatBank.com för att verifiera dess identitet. Certifikatet tillhandahålls av en certifikatutfärdare som [!DNL DigiCert] eller [!DNL Thawte]. Eftersom webbläsaren litar på certifikatutfärdaren tillåts anslutningen.
>
>* **Ömsesidig TLS**: MySoftware.com är en programvaruklient som behöver information från API:t MyGreatBank.com. MyGreatBank tillåter bara betrodda klienter att ansluta till sina servrar. Förutom den vanliga TLS-verifieringen av identiteten på MyGreatBank.com verifierar TLS/certificate Authority-processen även begäran från MySoftware.com.


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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

&#42;&#42;För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Tillhandahåller [!DNL Workfront Fusion] offentligt certifikat


När du ansluter till en webbtjänst med en HTTP-begäran kräver webbtjänsten vanligtvis en [!DNL Workfront Fusion] offentligt certifikat för verifiering. Detta gör att webbtjänsten kan jämföra det certifikat som anges i HTTP-begäran med det som finns tillgängligt, för att säkerställa att certifikatet finns på webbtjänstens tillåtelselista.

Instruktioner om hur du överför [!DNL Adobe Workfront Fusion] offentligt certifikat till en webbtjänst finns i webbtjänstens dokumentation.

>[!NOTE]
>
>Du kan behöva ange annan information utöver certifikatet. Information om vad en webbtjänst kräver finns i webbtjänstens API-dokumentation.

Du kan använda följande länkar för att hämta Workfront Fusion offentliga certifikat:

### Certifikat för 25 maj 2023-9 juni 2024

>[!IMPORTANT]
>
>* Dessa [!DNL Workfront Fusion] offentliga certifikat upphör att gälla den 9 juni 2024. När ditt certifikat har gått ut måste du överföra det till webbtjänsten. Vi rekommenderar att du:
   >
   >   * Notera förfallodatumet och ange en påminnelse för dig själv om att överföra certifikatet till din webbtjänst.
   >   * Bokmärk den här sidan för att enkelt hitta de nya certifikaten.
>
* Dessa är mTLS-certifikat som inte är jokertecken.
>

* [Hämta [!DNL Workfront Fusion] Certifikat 2023](assets/fusion-prod-us-mtls-certificate.pem)
* [Hämta [!DNL Workfront Fusion] EU-certifikat 2023](assets/fusion-prod-eu-mtls-certificate.pem)

   För användning i EU

### Certifikat för 14 november 2022 - 15 juli 2023

>[!IMPORTANT]
>
>* Dessa [!DNL Workfront Fusion] offentliga certifikat upphör att gälla den 15 juli 2023.
>* Dessa är mTLS-jokertecken.


* [Hämta [!DNL Workfront Fusion] Certifikat 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Hämta [!DNL Workfront Fusion] EU-certifikat 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   För användning i EU

## Aktivera Ömsesidig TLS i [!DNL Workfront Fusion] HTTP-moduler

Alla [!DNL Workfront Fusion] [!UICONTROL HTTP] begärandemoduler har möjlighet att aktivera ömsesidigt TLS.

Aktivera Ömsesidig TLS i en [!UICONTROL HTTP] begärandemodul:

1. Lägg till en [!UICONTROL HTTP] begär modul till ditt scenario.
1. Börja konfigurera modulen.

   Instruktioner om hur du konfigurerar en [!UICONTROL HTTP] modul för begäran, se lämplig artikel under [[!UICONTROL HTTP] moduler](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Aktivera **[!UICONTROL Show advanced settings]** nära modulens nederkant.
1. Aktivera **[!UICONTROL Use Mutual TLS]**.
