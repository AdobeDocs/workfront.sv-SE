---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server-moduler
description: Du kan använda [!DNL Adobe Workfront Fusion] för att ansluta till Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] moduler

Du kan använda [!DNL Adobe Workfront Fusion] för att ansluta till [!UICONTROL Microsoft SQL Server].

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



## Ansluta [!DNL Microsoft SQL Server] service till [!DNL Workfront Fusion]

Instruktioner om hur du ansluter [!DNL Microsoft SQL Server] konto till [!UICONTROL Workfront Fusion], se [Skapa en anslutning till [!UICONTROL Adobe Workfront Fusion] - Grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Vissa Microsoft-program använder samma anslutning, som är kopplad till individuella användarbehörigheter. När du skapar en anslutning visas därför alla behörigheter som tidigare har beviljats användarens anslutning, förutom de nya behörigheter som krävs för det aktuella programmet.
>
>Om en användare till exempel har behörighet att läsa tabell som beviljats via Excel-anslutningen och sedan skapar en anslutning i Outlook-anslutningen för att läsa e-post, visar tillståndsskärmen både den behörighet som redan har beviljats för att läsa tabell och den behörighet som nyligen har krävts för att skriva e-post.

## Använda [!DNL Microsoft SQL Server] moduler

Du kan köra din anpassade logik direkt på databasservern via lagrade procedurer. [!DNL Adobe Workfront Fusion] läser in gränssnitt för in-/utdataparametrar och postmängd dynamiskt så att varje parameter eller värde kan mappas individuellt. Innan du börjar konfigurera ditt scenario bör du kontrollera att kontot som du använder för att ansluta till databasen har läsåtkomst till `INFORMATION_SCHEMA.ROUTINES` och `INFORMATION_SCHEMA.PARAMETERS` vyer.

När [!DNL Fusion] upprättar anslutningen till [!DNL SQL server] mål, [!DNL Fusion] -användare identifierar värden (domännamnet eller IP-adressen där servern finns) och porten. [!DNL Fusion] kan ansluta till alla tillgängliga värdar och portar.

Mer information om specifika IP-adresser som används av [!DNL Workfront Fusion], se [IP-adresser för åtkomst [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Mer information om hur du skapar en lagrad procedur finns i [!DNL Microsoft SQL Server] dokumentation.

>[!NOTE]
>
>[!DNL Workfront Fusion] stöder inte flera postmängder. Endast den första bearbetas.

## Felsökning [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Lock wait timeout exceeded; try restarting transaction]

Det här felet inträffar när du ändrar samma data med flera moduler. Den orsakas av SQL-transaktioner.

När en SQL-modul körs startar den en transaktion. Transaktionen avslutas när scenariot har slutförts.

Om en annan modul försöker få åtkomst till samma data måste den vänta tills den föregående transaktionen är klar. Eftersom den första transaktionen slutförs efter att scenariot har slutförts kan den andra transaktionen aldrig påbörjas.

### Lösning:

Aktivera Automatisk implementering. Den automatiska implementeringen slutför (verkställer) alla transaktioner omedelbart efter att modulen har körts.

1. Klicka på [!UICONTROL Scenario settings] icon ![](assets/scenario-settings-icon.png)längst ned på skärmen.
1. Klicka på **[!UICONTROL Auto commit]** kryssrutan.
1. Klicka **[!UICONTROL OK]** för att spara scenarioinställningarna.
